---
description: CONCEPTS
---

import ControlTreesLogicalScreenshot from '/img/gitbook-import/assets/image (61).png';
import ControlTreesVisualScreenshot from '/img/gitbook-import/assets/image (15) (2).png';
import ControlTreesEventScreenshot from '/img/gitbook-import/assets/image (1) (1) (2).png';

# Control Trees

_Avalonia UI_ creates control trees from the XAML files in an application so that it can render the UI presentation and manage the application functionality.  &#x20;

## Logical Tree

The logical control tree represents the application controls (including the main window) in the hierarchy in which they are defined in the XAML. For example: and control (button) inside another control (stack panel) in a window will have the 3-layer logical tree shown here:

<img src={ControlTreesLogicalScreenshot} alt=""/>

While your application is running, you can show the _Avalonia Dev Tools_ window (hit F12). This displays the logical tree on its **Logical Tree** tab.

## Visual Tree&#x20;

The visual control tree contains everything that is actually being run by _Avalonia UI_. It shows all the properties set on the controls, and all the additional parts that have been added by _Avalonia UI_ in order to present the UI and manage the application functionality. &#x20;

<img src={ControlTreesVisualScreenshot} alt=""/>

You can see the visual control tree on the **Visual Tree** tab of the _Avalonia Dev Tools_ window.

## Events&#x20;

An essential part of application functionality management performed by _Avalonia UI_, is the generation and propagation of events. The **Events** tab logs the source and propagation of events as you move around, and otherwise interact with the running application.

<img src={ControlTreesEventScreenshot} alt=""/>
