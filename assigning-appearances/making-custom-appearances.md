---
description: Sometimes the default appearances just don't cut it.
---

# Making Custom Appearances

## Editing Existing Appearances

In the _Appearances_ tab, we can right-click on an appearance and hit _Edit_ to alter its properties, including color, roughness, and reflectance.

![Opening the &quot;Edit&quot; menu for &quot;Aluminum - Satin&quot;](../.gitbook/assets/957ccecf89eeca52c7a9926838348a7e.gif)

![Using the color map and slider to change the color of the mecanum wheel plate](../.gitbook/assets/culurz.gif)

![Using the sliders to change the roughness and reflectance of the appearance](../.gitbook/assets/slidurr.gif)

### Changing Roughness

For certain appearances, we can change the roughness to make the part look smoother or rougher \(a higher value means rougher\).

![goBILDA channel set to &quot;Aluminum - Anodized \(Red\)&quot; with roughness decreasing from left to right \(0.75, 0.35, and 0.122 \(default\) respectively\)](../.gitbook/assets/roughness.png)

### Changing Reflectance

For certain appearances, we can change the reflectance, which affects the amount of light reflected by the part. The higher the value, the more reflective and shiny it becomes, and vice versa.

![Timing belt pulley set to &quot;Plastic - Glossy \(Blue\)&quot; with reflectance increasing from left to right \(0.015, 0.053 \(default\), and 0.08 respectively\)](../.gitbook/assets/pull.png)

### Editing the Scale and Rotation

Many appearances have textures linked with them, that is source images that define part of the look of the appearance. When these appearances are applied, the scale of the source image is often much too large or small to look proper on the object.

In the example below, a granite appearance is edited from the stock scale to a much more reasonable level. In addition, the rotation was changed slightly to slightly change the look of the granite.

![Changing the scale and rotation of the granite texture from stock settings](../.gitbook/assets/123187422eecc9520066f1c2469663ab.gif)

### Editing Wood Settings

Unlike many of the other appearances, the solid wood appearances contain a few unique parameters relating to the earlywood, latewood, and rings of the wood appearance.

* Earlywood roughness: controls the roughness of the earlywood \(the lighter wood\)
* Latewood roughness: controls the roughness of the latewood \(the darker rings\)
* Ring thickness: controls the thickness and spacing of rings
* Ring bump: controls the bump of the rings
* Pores/rays: toggles that add extra imperfections to the wood \(recommended to keep on\)

In the example below, these sliders are adjusted to improve upon the current settings and create a wood appearance that more closely matches the desired look.

![Adjusting the parameters of 3D Maple - Glossy](../.gitbook/assets/6e73d80746bf3c9ac5bde2b5028104c4.gif)

## Creating New Appearances

While often adjusting existing appearances works well for creating the desired look, there are often times where a completely new appearance would achieve a much better result.

There are 3 main ways to create a custom appearance: importing the texture source image, importing the bump map source image, and importing the cutout source image. These 3 aspects will be covered in two examples below.

### Texture Source Image

The texture source image defines how the appearance looks at the base level, much like how the carbon fiber appearance adds the recognizable weave. To achieve the same effect but on a custom appearance, a new source image needs to be added.

In the example below, an FTC field tile image is being used as the texture source image. While this one is provided, taking your own tile source images is encouraged as it will make your tile appearance unique to your team.

![Source image used in the tile example below](../.gitbook/assets/fieldtiles-editednoedge-contrast_brightness.png)

To create a custom appearance any appearance can be used, but in this example, the "Base Material - Opaque" appearance will be used as a starting point. To add the field tile image navigate to the advanced editing menu of the appearance and change the color input to an image input.

![Changing the base material appearance  to use the field tile image](../.gitbook/assets/8b3778cd3dd3e9fdf35db60e133d5d16.gif)

Already the appearance should be looking pretty close to a tile, but the patterning of the source image looks strange. To fix this, 1 tile of the source image must cover 1 tile, meaning that there is only 1 instance of the image per tile. This is accomplished by clicking on the image in the advanced edit menu and changing the scale to be 25 inches x 25 inches.

![Changing the size of the source image](../.gitbook/assets/f1abd2162bc0465a5ebf39badca17c8b.gif)

While the size of the source image tiles looks correct now, the image tile may not match up with the actual tile body properly. Fixing this issue by manipulating the position of the tiling is covered in [Texture Map Controls](texture-map-controls.md).

### Bump Map

Bump maps are a way of generating a fake normal displacement, that is a displacement of the surface to create dips and bumps. While bump maps do not actually change the geometry of the model \(hence the "fake normal displacement"\), they can give the sensation of displaced geometry.

There are many different and better ways to generate bump maps, for the field tile example, the bump map source image will be exactly the same as the texture image. The same process is followed for importing the image and resizing, only in the bump section of the advanced edit settings.

![Applying and scaling a bump map](../.gitbook/assets/243d2f19086397ecfe96ff320f3be245.gif)

After applying the bump map, the depth of the bump map can be adjusted to create the desired displacement.

![Adjusting the depth of the bump map](../.gitbook/assets/b7448dd913654b27ab3698fbb41ddb04.gif)

{% hint style="info" %}
After adding a bump map, and especially for the field tiles, always check and adjust the reflectance and roughness settings.

Field tiles can become oddly shiny after adding a bump map.
{% endhint %}

![Adjusting the roughness and reflectance of the field tiles](../.gitbook/assets/c0fdf4f8d3ca87397adc7b8552635977.gif)

### Cutout

Cutout, much like a bump map, creates a fake effect, this time making it appear as if there are holes in the model when in actuality some parts of the model are becoming transparent.

In the example below an appearance that mimics the netting of the FTC Ultimate Goal field will be created using a custom cutout map. Starting with the "Plastic - Glossy \(Black\)" appearance, the cutout image is added and scaled in the advanced section of the appearance edit menu.

![Cutout source image used the example below](../.gitbook/assets/untitled-drawing-26-.png)

![Adding the cutout source image](../.gitbook/assets/59810a0ac88f6522598127779b598a99.gif)

The cutout is both much too large and inverted, but these issues can be easily fixed in the cutout image settings menu.

![Inverting the cutout and scaling it](../.gitbook/assets/8c7fe13c8eb85715b056bb2e1ba7becc.gif)

{% hint style="info" %}
A similar process as the one demonstrated in this example can be used to achieve a wire sleeve appearance.
{% endhint %}

