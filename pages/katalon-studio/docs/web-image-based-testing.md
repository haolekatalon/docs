---
title: "Web Image-based Testing" 
sidebar: katalon_studio_docs_sidebar
permalink: katalon-studio/docs/web-image-based-testing.html 
redirect_from: 
    - "/katalon-studio/docs/web-image-based-object-recognition.html"
---

## Requirements

* Your Katalon Studio version must be 7.2.2 or later.
* You need an active Katalon Studio Enterprise license.

Katalon Studio provides Image locator method to associate Test objects with images. This method allows users to perform image-based testing when elements of the web application under test retain their appearance even though the underlying structures have changed.

This guide shows you how to configure image-based object recognition, capture screenshots, and reduce the chance of failures in image-based testing.

## Enable Image-based object recognition

**From 7.6 onwards**

Image-based object recognition is enabled by default for web test execution in **Project > Settings > Self-Healing > Web UI > Test Execution** ([See Self-healing Tests](https://docs.katalon.com/katalon-studio/docs/self-healing.html)).

<img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/image-based-web-elements-recognition/image-enabled.png" width="" height="">

<details>
<summary><strong>Before 7.6</strong></summary>

By default, image-based object recognition is disabled in Project Settings. Please go to <strong>Project > Settings > Execution</strong> and check <strong>Enable Image Recognition</strong> to turn on this fallback strategy.
<br>
<img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/image-based-web-elements-recognition/enable.png" width="" height="">
</details>

## Capture screenshots for object recognition

### Using built-in tools 

In order to produce images associated with captured Test objects, Katalon Studio includes the **Add Screenshot** button in both Web Recorder and Spy Tool.

To capture an image of a Test object:

1. Open your AUT with Web Recorder/Spy Tool.
2. In **Captured Objects** view, select a captured object and click **Add Screenshot** button on the bottom right corner.

   <img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/image-based-web-elements-recognition/recorder.png" width="" height="">


### Using other tools

If you capture object images using other tools, you have to resize them to the display sizes of the corresponding web elements.


## Add image locator to objects

**From 7.6 onwards**

After you capture a screenshot using Web Recorder/Spy Tool, Katalon Studio automatically adds an image locator to the associated object.

To use image locator of an object:
1. Open the object in Object's view.
2. Select **Image** as the **Selection Method**.

   <img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/image-based-web-elements-recognition/image-locator.png">

<details>
<summary><strong>Before 7.6</strong></summary>

After you capture a screenshot using Web Recorder/Spy Tool, Katalon Studio adds a property called <strong>screenshot</strong> to the associated Test object. This property contains the absolute path to the captured screenshot.
<br>
To enable image locator of an object:
1. Open the object in Object's view. 
<br>
2. Select <strong>Attributes</strong> as the <strong>Selection Method</strong>.
3. In the <strong>Object's Properties</strong> table, tick the <strong>screenshot</strong> property. 
<br>
<img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/image-based-web-elements-recognition/property.png" width="" height="">
</details>

> **Note**
>
> For a screenshot captured using other tools, you must provide the absolute path to the screenshot in the **Path** property when enabling the image locator.

## Reduce the chance of failures

Since reliable image-based testing depends on image comparison, you can reduce the chance of failures in two ways:

* **Screen Resolution**: The screen resolutions of screenshot capturing machines and test executing machines can affect the accuracy of image comparison. We recommend capturing screenshots and executing tests on the same machine for the best results.

* **Capture tool**: We recommend using built-in capture tools in Web Recorder and Spy Tool since they automatically resize the captured images.

**See also**:

* [Sample Project](https://github.com/katalon-studio-samples/image-recognition-web)
* [Self-Healing Tests](https://docs.katalon.com/katalon-studio/docs/self-healing.html)
