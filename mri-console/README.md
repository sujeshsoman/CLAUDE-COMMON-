# Mallu Radiographer · Virtual MRI Console

A practice MRI scanner console that runs in any web browser. Everything is in one file, `index.html`. It needs no internet connection, no images and no installation.

## Known limitations

- **The images are computer-made, not real scans.** Every picture is calculated in the browser from a simple 3D model of a head (and a much simpler knee) using textbook MRI formulas. They behave like MRI (CSF is bright on T2, dark on FLAIR, and so on) but they are less detailed than real images. No real patient images are used anywhere.
- **The anatomy is simplified.** The brain looks convincing but slightly artificial. The face, neck and knee are made of simple shapes, and the knee looks much less realistic than the brain.
- **Lumbar spine is not built yet.** It shows as "coming soon".
- **High matrix settings don't add detail.** Pictures are drawn at up to 320 pixels across. Choosing a 384 or 512 matrix changes the scan time, SNR and voxel size numbers, but not the sharpness of the picture.
- **The numbers are approximations.** Scan time, SNR, maximum slices and SAR are calculated to teach the right trade-offs (for example: longer TR gives more slices but a longer scan). They will not match any real scanner exactly. SAR is a rule of thumb, not a safety calculation.
- **Artifacts are imitated, not fully simulated.** Wrap-around, fat shift, motion ghosts, blurring and susceptibility loss appear in the right places and directions, but they are painted onto the image rather than produced from simulated raw (k-space) data.
- **Some features are basic:**
  - 3D scanning is only available for gradient echo.
  - Contrast is simply "given" or "not given", with no change over time.
  - Fat suppression never fails.
  - Patient position (head first, feet first, prone) only changes the labels, not the images.
- **Slow phones need a few seconds after each scan.** On a slower phone the remaining slices of a series appear over several seconds after the scan finishes, and show "Reconstructing…" until they're ready.
- **Nothing is saved.** Reloading the page starts again from the beginning. There are no logins or accounts.
- **Testing so far is limited.** It was tested in a Chromium browser on a desktop screen and on an emulated 360-pixel-wide Android phone with its processor slowed down 4×. It has not yet been tried on a real phone, an iPhone (Safari) or Firefox.
- **It is for teaching only.** It is not for clinical use, is not a medical device, and does not connect to any real scanner.

## What you can do with it

1. **Register a patient**: name, age, weight (used for SAR), position and coil, or tap **Demo patient**. You can also pick a teaching case: MS-like plaques, tumour with oedema, acute infarct or microbleeds for the brain, or bone bruise, effusion or meniscal tear for the knee.
2. **Load a protocol**: the brain routine or the knee routine.
3. **Run the 3-plane localizer**, then **plan** on it:
   - drag the slice stack to move it
   - drag the yellow circle to angle it, or press **Align AC–PC**
   - add a saturation band
4. **Change parameters** and watch the live preview update as you move each slider. You can change TR, TE, TI, flip angle, echo train, b-value, fat saturation, FOV, matrix, slice thickness, gap, number of slices, orientation, phase direction, averages, bandwidth, 1.5 T or 3 T, and 2D or 3D.
   - **Calculated for you:** scan time, voxel size, SNR, maximum slices, minimum TE, fat shift and SAR.
   - **If a setting is impossible** (for example TE too short, or too many slices for the TR), the console warns you and offers a one-tap fix.
5. **Scan**: the queue runs with a progress bar, at 40× or 15× speed or in real time, with optional scanner noise and a "patient moving" switch.
6. **View the images**: scroll through slices, set window and level, zoom, pan, measure an ROI, invert, and compare series side by side in 1×2 or 2×2 layouts.
7. **Learn and test yourself**: a Learn panel explains each parameter, 7 challenges are checked automatically (for example "null CSF with FLAIR" or "remove the wrap-around"), and an exam report summarises the session.

## How to open it

**On a computer:** download `index.html` and double-click it. It opens in your browser and works offline.

**On your phone**, choose one:

1. **Put it on your website.** Upload `index.html` to malluradiographer.com, for example into a folder called `mri-console`, using your hosting's File Manager or FTP. Then open `https://malluradiographer.com/mri-console/` on your phone. To show it inside a blog post or page, paste this into a "Custom HTML" block:

   ```html
   <iframe src="https://malluradiographer.com/mri-console/" title="Virtual MRI Console"
           style="width:100%;height:900px;border:0" allow="autoplay"></iframe>
   ```

2. **Free instant link with Netlify Drop.** On a computer, go to `app.netlify.com/drop` and drag the `mri-console` folder onto the page. You get a public web address straight away, and you can open it on any phone.
3. **GitHub Pages.** In this repository's settings, open **Pages**, choose "Deploy from a branch", then pick this branch and the `/ (root)` folder. The console will then be at `https://sujeshsoman.github.io/CLAUDE-COMMON-/mri-console/`. Free GitHub accounts can only do this for public repositories.

Opening the downloaded file directly on a phone often doesn't work well, because phone browsers restrict local files. Use one of the web options above instead.

## Measured performance

Measured in Chromium with a frame counter running while dragging. The phone was emulated at 360×800 with touch and a CPU slowed down 4×, to stand in for a mid-range Android phone.

| | Desktop | 360px phone, 4× slower CPU |
|---|---|---|
| Dragging the slice stack on a localizer | 60 fps | 47 fps |
| Scrolling slices in the viewer | 60 fps | 59 fps |
| Preview update after changing TR, TE or flip angle | under 10 ms | about 8–33 ms |
| Preview after a geometry change (position, angle, FOV) | about 50–80 ms | about 220–250 ms (a quick rough preview shows while dragging) |
| One full image slice | about 150 ms | about 650 ms (drawn in the background) |

## How it works (short version)

- **Phantom:** the head is described in millimetres as overlapping shapes, with folded cortex added using smooth noise. For each pixel of the slice you plan, the program works out which tissue sits at that point in 3D, so slice position, angle and FOV genuinely change the picture.
- **Tissue values:** each tissue has T1, T2, T2*, proton density and ADC values, with separate values at 1.5 T and 3 T.
- **Signal equations:**
  - spin echo / TSE: `PD·(1−e^(−TR/T1))·e^(−TE/T2)`
  - inversion recovery (FLAIR/STIR): `PD·|1−2e^(−TI/T1)+e^(−TR/T1)|·e^(−TE/T2)`
  - spoiled gradient echo: `PD·sinα·(1−E1)/(1−cosα·E1)·e^(−TE/T2*)`
  - diffusion: multiplied by `e^(−b·ADC)`
- **Noise:** added according to the SNR model, which uses voxel size, averages, bandwidth, field strength and coil.
- **Speed:** contrast changes only recalculate one number per tissue, so they are instant. Geometry changes recalculate the tissue map, which takes longer.

The console design, icons and wording are original. They are not copied from any scanner manufacturer.
