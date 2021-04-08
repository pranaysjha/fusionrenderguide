---
description: >-
  Different from standard appearances, they emit light instead of simply
  reflecting.
---

# Emissive Appearances

While not commonly used, emissive appearances can provide additional lighting to the scene and highlight certain parts of the render. Emissive appearances can be accessed through the "Miscellaneous" and then "Emissive" folders of the appearance menu.

### Changing the Emission Color

1. While changing the emission color is not as straight forwards as changing the color of a standard appearance, it is still fairly simple. The color should be changed in all 3 places shown below to have the proper coloring.

![Changing the base color](../.gitbook/assets/19b170edaa38fe7d62e739d2c1fb239c.gif)

![Changing the emissitivity color](../.gitbook/assets/206dfa1a83c6669bb02e1c9efe686de9.gif)

![Changing the highlight control color](../.gitbook/assets/984eba59813f15c0b84788a3f1891116.gif)

### Adjusting the Luminance

Much like the brightness of the scene can be adjusted, the brightness of emissive materials can be adjusted. Adjusting the brightness to a proper level can be hard without running ****[**In-Canvas Renders** ](../rendering-and-exporting/cloud-vs.-local-rendering.md)to check the current look of the render in real time.

![Adjusting the luminance of the emmisive appearance](../.gitbook/assets/259bb55f78638aa38362227cb3509c8b.gif)

### Post-Processing

Unlike renders without emissive materials, the rendered output often looks off, with additional work needed to achieve the desired look. The [**post-processing**](../rendering-and-exporting/post-processing.md) page covers this in detail, but consider adding some bloom, decreasing exposure, and increasing the prominence of shadows.

![Raw render output \(left\); post-processed render \(right\)](../.gitbook/assets/untitled-drawing-25-.png)



