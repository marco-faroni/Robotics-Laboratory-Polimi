---
title: FAQs, hints, and pointers
layout: default
nav_order: 9
---

# FAQs, hints, and pointers

## Back up and restore a workspace

To make a backup:

- Insert a USB drive into the TP or controller, open **Project → Loader**, and copy the project to the drive; or
- In Estun Editor, right-click the workspace, select **Save locally**, and choose a PC folder.

Restore with **File → Open Workspace** and select the backup.

{: .important }
> Before backing up a real controller, use **Upload from robot** so the editor includes the controller's current content. After restoring a backup, use **Download to robot** to place it on the controller.

## Switch between Auto and Auto-External

**Auto (A)** runs programs from the TP. **Auto-External (AE)** allows execution from Estun Editor or external buttons. Select the appropriate mode on the TP before attempting to start a program.

## Safety-door and AutoRun errors

The messages **Safety door is not open** and **Start AutoRun failed** can prevent automatic execution. Usually, a digital input configured as a safety-door signal is not at its expected state (normally `1`, meaning door closed).

Open the **I/O** tab and check the configured safety-door inputs—typically `DI4` and `DI13` in this cell.

{: .warning }
> Never bypass, force, or reconfigure safety I/O to clear an error. Check the physical cell and ask the instructor if the expected state is unclear.

## Create safety areas

Estun provides two area types:

- **Polyhedron:** safety-certified area; up to four can be created through **User App → Polyhedron**.
- **Area:** available to program logic but not safety-certified; create it as a global variable of type `Area` on the TP.

## Import an external CAD model

1. Open **Full-function Simulation** and select **Scene Tree**.
2. Right-click **Models → New Scene**, then save the new scene.
3. Right-click **Models → Import model**.
4. Save the scene again after importing.

## Move to a default pose

On the TP, go to **ROB → GoPoints**. Define the home positions there and move the robot to the selected one after checking that the path is safe.

## Create a user frame

In Estun Editor, select **Function → User Coordinate Calibration** and follow the calibration procedure.

## Tool calibration

Tool calibration defines the tool centre point and orientation relative to the robot flange. Use the dedicated course procedure and verify the result at low speed.

## Object calibration

Object calibration defines a coordinate frame for a workpiece or fixture. Establish it only after the object is fixed in its final position.

## Camera calibration

Camera-to-robot calibration determines the transformation between camera and robot coordinates. This procedure is course-specific; use the dedicated lab instructions and obtain instructor approval before changing calibration data.

## Robot APIs

API access and supported interfaces depend on the controller configuration. Use only the course-provided API instructions and test commands in simulation or at a safe reduced speed.

## Recalibrate robot encoders

Encoder recalibration changes the robot's reference information. Do not perform it without explicit instructor authorisation and the official procedure.
