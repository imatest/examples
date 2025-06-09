Stray Light Source Example Images
Imatest, LLC
--

This folder contains example images of a small, bright light source. The source was collimated, with an angular diameter of 0.11 degrees. The camera was deliberately overexposed to reveal stray light (flare) in the image. The original 12-bit RAW image were demosaiced and converted to linear 16-bit RGB format by applying a 4-bit left shift.

Each image filename includes the field angle of the light source with respect to the camera (e.g., -24_degrees_1.png).

For each source angle, three images were captured at different camera exposure times to show stray light of different magnitude:

1) 0.00124006 seconds

2) 0.0419914 seconds

3) 0.333319 seconds

An additional on-axis reference image is included, showing the source without saturation and revealing its actual size to be a small point. To capture this image, a neutral density (ND) filter with optical density 2.5 was placed in the path of the collimated beam, and the camera exposure time was reduced to 0.00000380682 seconds.

These images can be used as an example to calculate the IEEE 2020-2024 (formerly P2020) normalized flare metric.

Notes for analysis in Imatest:
- Dark level = 648 DN
- Saturation level = 65520 DN
- Analyze each exposure level separately. Do not mix test images that were captured with different exposure times in a single analysis run.
- To label the outputs with the correct field angles, use the following for the filename regular expression setting: (?<field>-?\d+(?:\.\d*)?)_degrees_\d+\.png$

--
For more information on how to analyze stray light in Imatest, see Imatest's documentation:
https://www.imatest.com/docs/stray-light-flare/standards/
https://www.imatest.com/docs/stray-light-flare/normalized-stray-light-instructions/
 
