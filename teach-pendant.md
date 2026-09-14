---
title: Teach Pendant
layout: default
nav_order: 5
---

# Teach Pendant

The Teach Pendant (TP) is used to set robot modes, jog the robot, teach positions, inspect status, and edit programs.

## Main functions

Become familiar with the TP before operating a real robot:

- The **status bar** shows the controller state, mode, and active messages.
- The physical **vertical buttons** include motion and enable controls.
- The physical **horizontal buttons** provide execution and navigation controls.

{: .note }
> Screenshots of the TP layout should be added here when the course reference images are available.

## Create and teach a program

1. Go to **Home → Programme → Project → New → New project**.
2. Enter a project name and select **OK**.
3. In the programming window, select the final `End` line.
4. Insert a motion primitive, for example `MovL`.
5. Jog the robot to the desired pose and press **Teach** to record it.

## Execute in teach mode

1. Press **Start**.
2. Press **PC** to set the program pointer to the selected line.
3. Hold the physical **Start** button while the program runs.

The robot movement is visible in the simulation window.

Watch: [create a program](doc/video_estun_editor/create_program.mkv) and [teach points with the TP](doc/video_estun_editor/teach_points_TP.mkv).

## Synchronise the TP and Estun Editor

Programs created on the TP are not automatically visible in Estun Editor. In the editor, right-click the controller and choose **Upload from robot**.

Conversely, after editing code in Estun Editor, choose **Save All**, then refresh the TP to see the changes there.

{: .important }
> Treat the controller/TP and Estun Editor as separate copies until you explicitly synchronise them.
