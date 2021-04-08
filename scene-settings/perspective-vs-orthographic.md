---
description: What are the two main camera types and which one should I use?
---

# Perspective vs Orthographic

Perspective and Orthographic are two camera types that define the perspective of objects within the frame.

**TLDR: Use perspective for all isometric renders, use orthographic for orthographically positioned renders.**

![Switching between orthographic and perspective in the scene settings tab](../.gitbook/assets/ee6cdd70304e61dc6e51e359d9f151d9.gif)

{% tabs %}
{% tab title="Perspective" %}
Perspective view displays object with realistic depth, making closer objects appear larger, and farther away objects appear smaller. While this gives the correct depth perception of the objects, it strips away any geometric squareness and scaling.

![A perspective render, scaling objects based on depth](../.gitbook/assets/perspective.png)
{% endtab %}

{% tab title="Orthographic" %}
Orthographic preserves 2D geometric properties, keeping angles and relative dimensions instead of distorting parts of the model based on depth. While these is highly undesired for isometric renders of the robot, for orthographic renders of the robot such as the one below, keeping the squares of the robot makes it easier to see the powertrain and odometry in the drivetrain.

![An orthographic render of the robot, preserving 90 degree angles](../.gitbook/assets/orthographic.png)
{% endtab %}
{% endtabs %}

Lastly, _Perspective with Ortho Faces_ is a combination of the two; most of the camera angles will result in perspective renders. When the camera is pointed directly at a face \(e.g. front and top\), it becomes orthographic. 

