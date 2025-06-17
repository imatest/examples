Stray Light Source Example Images
Imatest, LLC
--

This folder contains example images of a small, bright white light source. The light source was collimated, with an angular diameter of 0.11 degrees. The camera was focused at infinity and operated in linear, single-exposure mode. The images were deliberately overexposed to reveal stray light (flare). The original 12-bit RAW image data were demosaiced and converted to 16-bit RGB format by applying a 4-bit left shift.

The ensemble of images can be used as an example to calculate the IEEE 2020-2024 (formerly P2020) normalized flare and flare intensity metrics.

Each image filename includes the field angle of the light source with respect to the camera (e.g., -24_degrees_1.png).

For each source angle, three images were captured at different camera exposure times to show stray light of different magnitude:
1) 0.00124006 seconds
2) 0.0419914 seconds
3) 0.333319 seconds

For all test images, the illuminance at the front of the camera was measured to be 251.132 lux. 

Two additional on-axis reference images are included: 
 - The "direct" reference image shows the direct image of the source without saturation, revealing its actual size to be a small point. To capture this image, a neutral density (ND) filter with optical density 2.5 was placed in the path of the collimated beam, and the camera exposure time was set to 0.00000380682 seconds. 
 - The "diffuse" reference image shows a diffuse image of the source without saturation, showing the relative spatial uniformity of the beam (though blurred due to diffusion and the camera being focused at infinity). To capture this image, an opal diffuser filter was placed in the path of the collimated beam and the camera exposure time was set to 0.0249985 seconds. The luminance of the diffuser surface facing the camera was measured to be 32.988 nits. 

Notes for analysis in Imatest:
- Dark level = 648 DN
- Saturation level = 65520 DN
- Analyze each exposure level separately. Do not mix test images that were captured with different exposure times in a single analysis run.
- To label the outputs with the correct field angles, use the following for the filename regular expression setting: (?<field>-?\d+(?:\.\d*)?)_degrees_\d+\.png$

--
For more information on how to analyze stray light in Imatest, see Imatest's documentation:
https://www.imatest.com/docs/stray-light-flare/standards/
https://www.imatest.com/docs/stray-light-flare/normalized-stray-light-instructions/
