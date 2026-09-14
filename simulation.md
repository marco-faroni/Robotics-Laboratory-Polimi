---
title: Robot simulation
layout: default
nav_order: 4
---

# Robot simulation

Use the virtual controller and simulator to learn the workflow before using the physical robot.

## 1. Connect to a virtual controller

1. Click **Disconnected**.
2. Select **Virtual Controller**.
3. Select the **ER4-550-MI** model.
4. Click **Connect**.

![Virtual controller connection dialog](doc/img/connect_to_virtual_controller.png)


## 2. Open the 3D simulator

Estun Editor includes two simulators:

- **Open 3D**: use this for routine jogging and movement.
- **Full-function Simulation**: use this for advanced tasks, such as importing CAD models and building 3D scenes.

You can open the simulators from the **Simulation** panel (see image below).

<img src="doc/img/open_simulator.png" alt="Simulation panel" style="display: block; margin: 1rem auto;">


## 3. Open the simulated Teach Pendant

The simulated Teach Pendant (TP) mirrors the physical pendant. It can jog the simulated robot, teach poses, and create programs and variables.

Open it from **Tool → Teach Pendant**.

<img src="doc/img/tp.png" alt="Simulated Teach Pendant command" style="display: block; width: 70%; height: auto; margin: 1rem auto;">

{: .important }
> For the recommended interface, set **SystemSet → Menu → System Settings → Personalization → New Style**, then close and reopen the TP.

## 4. Jog the robot from the Teach Pendant

1. Open **Open 3D** and the simulated TP.
2. Select **Teaching** mode on the TP (see image below).

   <img src="doc/img/tp_mode_selector.png" alt="Teach mode selection" style="display: block; margin: 1rem auto;">

3. Enable the motors with **Mot**.
4. Use **A1** through **A6** to jog individual axes.
5. Press **Jog** to choose joint, world-Cartesian, or tool-Cartesian jogging according to the following graphics:

<img src="doc/img/tp_frames.png" alt="Jog mode selection" style="display: block; width: 40%; height: auto; margin: 1rem auto;">


{: .important }
> Check the selected frame and jog mode before moving the robot. A Cartesian command behaves differently in world and tool coordinates.

<!--
## Test a program in manual mode

### Video: test a program step-by-step in manual mode

<video controls preload="metadata" playsinline style="width: 100%; max-width: 960px">
  <source src="doc/video_estun_editor/run_program_manual.mp4" type="video/mp4">
  Your browser does not support embedded video. <a href="doc/video_estun_editor/run_program_manual.mp4">Open the video</a>.
</video>
-->
