---
title: Vision
layout: default
nav_order: 8
---

# Vision

## Standard workflow with SCMVS

The standard HIKRobot-camera workflow uses **SCMVS**. Download SCMVS 3.3 from the [HIKRobot download page](https://www.hikrobotics.com/en/machinevision/service/download/).

{: .note }
> SCMVS requires a connection to the physical camera.

### Connect to the camera

1. Connect the PC to the camera Ethernet cable.
2. Configure a static IPv4 address: `192.168.100.XXX`, netmask `255.255.255.0`, where `XXX` is 1–254 and unused.
3. Open SCMVS and connect to the detected device.

The course camera password is provided separately by the instructor.

### Create a basic recipe

1. Click on create a new recipe.
2. Use **One Key Adjustment**: select the region of interest and apply the adjustment.
3. Set **Trigger Mode** to **External** and **Source** to **Software**.
4. In **Communication**, inspect the trigger string expected by the camera.
5. Under **Base**, select **Current Image**, then capture an image.
6. Add processing blocks under **Tools** and define the result under **Output**.

A basic step-by-step tutorial to create a recipe for object detection is available [here](doc/Tutorial_Camera.pdf).

Refer to the HIKRobot YouTube channel for tutorials on more advance tools.

## Camera SDK

You can use the camera Software Development Kit (SDK) to acquire raw images and implement custom algorithms (e.g., from OpenCV).

TODO: SDK tutorial

## Transfer images through FTP

As an alternative, you can send raw images from SCMVS to a PC via File Transfer Protocol (FTP) and then process the received images with a standard vision library such as OpenCV.

1. Set up an FTP server on the PC.
2. Configure SCMVS's FTP client with the server details.
3. Trigger image acquisition and verify that files arrive before automating processing.

See the [FTP setup video](https://www.youtube.com/watch?v=a-fWLcoLqcg) for an example.
