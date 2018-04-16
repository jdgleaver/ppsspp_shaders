# ppsspp_shaders

A small collection of shaders for [PPSSPP](https://www.ppsspp.org/) standalone, ported from various sources.

- All shaders include a '(Mobile)' variant which forces 'highp' variable precision for compatibility with Android devices

- All shaders include a '+ PSP Color' variant, which applies colour correction to replicate the LCD dynamics of the PSP 1000 and PSP 2000 displays

## Bead

A port of the 'bead' shader from RetroArch, which turns each pixel into a round bead. The native PSP resolution is too high for this to work entirely as it should (unless used with a 4k+ display), but it still produces quite a nice clean, crisp result.

- REQUIRES a rendering resolution of 1xPSP

- REQUIRES a display resolution of at least 1080p

- Runs at full speed on mid-range Android devices

## Dot

A port of the 'dot' shader from RetroArch, which produces an LCD effect with a cosy sort of glow.

- REQUIRES a rendering resolution of 1xPSP

- REQUIRES a display resolution of at least 1080p

- This is quite a 'heavy' shader, intended for Desktop use. The '(Mobile)' version will only run at full speed on high end Android devices.

## LCD3x

A port of the LCD3x shader from RetroArch.

- REQUIRES a rendering resolution of 1xPSP

- Runs at full speed on mid-range Android devices

- Does *not* require a 1080p display. This shader produces decent results (i.e. no unbearable aliasing effects) at 1360x768, and so is appropriate for potato laptops

## LCD1x

A 'tweaked' version of LCD3x that is 'sharp' and which omits the 3-band LCD colour effect.

- REQUIRES a rendering resolution of 1xPSP

- Runs at full speed on mid-range Android devices

- Does *not* require a 1080p display. This shader produces decent results (i.e. no unbearable aliasing effects) at 1360x768, and so is appropriate for potato laptops

## PSP Color

Simply applies PSP colour correction.

- Works with any rendering resolution

- Runs at full speed on mid-range Android devices

- Has no display resolution requirements

## zfast LCD

A port of the zfast_lcd shader from RetroArch. This creates an LCD effect by performing nearest neighbour scaling and adding a subtle grid lattice.

- REQUIRES a rendering resolution of 1xPSP

- REQUIRES a display resolution of at least 1080p

- Runs at full speed on mid-range Android devices

## zfast LCD HD

A tweaked version of 'zfast LCD' which supports arbitrary rendering resolutions. Applies the same grid effect, but omits the nearest neighbour scaling.

- Works with any rendering resolution

- REQUIRES a display resolution of at least 1080p

- Runs at full speed on mid-range Android devices
