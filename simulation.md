---
title: Robot simulation
layout: default
nav_order: 4
---

# Robot simulation

Use the virtual controller and simulator to learn the workflow before using the physical robot.

## Connect to a virtual controller

1. Click **Disconnected**.
2. Select **Virtual Controller**.
3. Select the **ER4-550-MI** model.
4. Click **Connect**.

## Open the 3D simulator

Estun Editor includes two simulators:

- **Open 3D**: use this for routine jogging and movement.
- **Full-function Simulation**: use this for advanced tasks, such as importing CAD models and building 3D scenes.

## Open the simulated Teach Pendant

The simulated Teach Pendant (TP) mirrors the physical pendant. It can jog the simulated robot, teach poses, and create programs and variables.

Open it from **Tool → Teach Pendant**.

For the recommended interface, set **SystemSet → Menu → System Settings → Personalization → New Style**, then close and reopen the TP.

## Jog the robot from the Teach Pendant

1. Open **Open 3D** and the simulated TP.
2. Select **Teaching** mode on the TP.
3. Enable the motors with **Mot**.
4. Use **A1** through **A6** to jog individual axes.
5. Press **Jog** to choose joint, world-Cartesian, or tool-Cartesian jogging.

{: .important }
> Check the selected frame and jog mode before moving the robot. A Cartesian command behaves differently in world and tool coordinates.
