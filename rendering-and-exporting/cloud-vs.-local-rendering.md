---
description: Comparing the three rendering options in Fusion 360.
---

# In-Canvas vs. Cloud vs. Local Rendering

In-Canvas, Cloud, and Local are three rendering options within Fusion 360.

TLDR: In-Canvas should be used to get a quick sense of what your render is looking like and adjust camera position/angle, scene setttings, and appearances. Cloud should be used for final renders.

{% tabs %}
{% tab title="In-Canvas Rendering" %}
**In Canvas**

In-Canvas creates a low fidelity, real-time render of your model within the Fusion rendering environment. While this does produce lower quality results than Local or Cloud renders as it does not utilize ray tracing and can simplify the lighting based on the settings, it is an extremely useful tool for checking lighting, appearances, scene settings, and camera angles.

1. Select "Fast" or "Advanced" from the In-Canvas settings menu.

{% hint style="info" %}
Fast reduces the material and lighting data, allowing the render to be executed faster, but at a much lower quality than what would be outputted in the advanced setting.
{% endhint %}

![Selecting the options for In-Canvas render](../.gitbook/assets/6f1d480d5dcfbb477ccd5738f0e89b14.gif)

  2. Start the render by clicking the icon with the sphere and the green arrow.

![Starting an In-Canvas Render](../.gitbook/assets/72acd1aa5a16e4449087e89244020782.gif)

{% hint style="info" %}
The In-Canvas Render can be paused by pressing the pause button at the lower right and can be stopped by clicking the icon with the sphere and the red stop button.
{% endhint %}
{% endtab %}

{% tab title="Cloud Rendering" %}
**Cloud Rendering**

Cloud rendering is one of two options for creating final renders that are high resolution and high quality. While local rendering can be utilized to achieve a virtually exact output as cloud rendering, cloud renders are done on the Autodesk servers, allowing you to run multiple renders in parallel with no load on your computer. 

1. Click on the teapot icon to open the rendering menu, selecting "cloud render".

![Opening the cloud/local render menu](../.gitbook/assets/06f7906a58e862602ff4b65439091431.gif)

2. Select the aspect ratio, render quality, and resolution of the render.

{% hint style="info" %}
Final render quality should always be selected during cloud renders, with a resolution above 1080p being used.
{% endhint %}

![Selecting the cloud render settings](../.gitbook/assets/d9e88044a698d350dfb39e34c219bab3.gif)

3. Hit render!
{% endtab %}

{% tab title="Local Rendering" %}
**Local Rendering**

Local rendering is one of two options for creating final renders that are high resolution and high quality. Cloud renders are prefered over local renders in almost every situation as local renders will take longer, load your local machine, and cannot be run in parallel. If for some reason, the Autodesk rendering servers are failing, this would be the rendering option to use for creating a final render.

{% hint style="warning" %}
Local rendering is generally not recommended in most cases unless you have a high-end computer and 
{% endhint %}

In addition to local renders being generally much less convenient, the post-processing features of cloud renders are unavailable in local renders.

#### How to Render Locally

1. Click on the teapot icon to open the rendering menu, selecting "local render".

![Opening the cloud/local render menu](../.gitbook/assets/fd6f65db6bb7e04329aea3aeeaaa7799.gif)

2. Select the render quality setting, aspect ratio, file format, and resolution.

![Selecting the local render settings](../.gitbook/assets/938f609edcca3385c3e27db01b73d4ae.gif)

3. Hit render!
{% endtab %}
{% endtabs %}

\*\*\*\*

