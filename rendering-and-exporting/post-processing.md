---
description: >-
  Often the render comes out slightly off, so there are built in post-processing
  features to adjust the render output.
---

# Post-Processing

If your render's exposure or saturation seems a bit high, or if there are other scene settings that you would like to tweak, Fusion provides an option to easily adjust these without having to redo the entire render.

The post-processing menu is accessed by first opening up the desired render, and then selecting the icon with a plus-sign and a minus-sign.

![Accessing the post-processing menu](../.gitbook/assets/8e0b6abd9171d2ad208ea6f7bfc76f4a.gif)

## Exposure

Exposure is essentially the amount of light in the image, or the relative darkness/lightness of the render. Often renders come out slightly dark, so **decreasing** the exposure value will increase the brightness of the image, and **increasing** the exposure value will decrease the brightness of the image.

![Adjusting the exposure of a render](../.gitbook/assets/cbdd1e232141c52b60faea5ec59c15f6.gif)

{% hint style="info" %}
Keep in mind that changing the exposure will alter colors \(e.g., the background color will no longer be what it was set to\).

Keep exposure values between 8.5 and 10.5, otherwise it gets extremely washed out out or dark.
{% endhint %}

## Color Preset

Color presets are built in settings that adjust the highlight compression, contrast, and shadow prominence. While these values can be adjusted manually, there are a few color presets that have fixed values for these settings. Changing these changes the look of the render, but vivid and linear are the best two, with vivid achieving a vibrant look that highlights colors, and linear achieving the most realistic look.

![Changing the color preset](../.gitbook/assets/95375488aca27788cad8ff7e82c18b5a.gif)

## Saturation

The saturation value controls the intensity of the colors in the render, with a value of 1 not changing anything, values closer to 0 approaching grayscale, and values above 1 increasing the intensity. While changing this is often unnecessary, it can help mute or highlight colors in the render.

![Adjusting the saturation of the render](../.gitbook/assets/700ffef3dabae838ea4e7d8a0aa98624.gif)

## Color Correction

The color correction slider can be used to adjust the white point of the render, or the color temperature of the main light source. Values below 6500 \(default\) will result in a colder-lit image with more blue hues, and values above 6500 will result in a warmer-lit image with more orange hues.

![Adjusting the white point of the render](../.gitbook/assets/8996796e5a366ddcee18efa7dbb7f6f8.gif)

## Bloom

Bloom is used in renders with emissive appearances to control the manifestation of bloom, a post-processing setting that mimics real-world photography of objects emitting a large amount of light.

{% hint style="info" %}
For there to be any bloom in the render, the bloom amount and bloom width multiplier must be a non-zero value.

For robot renders, a small bloom amount and bloom width will give a more photorealistic look to the emissive materials.
{% endhint %}

![Adjusting the bloom in a render with emissive materials](../.gitbook/assets/1787fd583c3ab5d415d8d953de493e8b.gif)

