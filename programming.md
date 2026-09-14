---
title: Robot programming
layout: default
nav_order: 6
---

# Robot programming

## Create a project

Right-click the controller, select **New Project**, and enter a project name. Estun Editor creates a main program automatically. Save with **Ctrl+S** or by right-clicking the controller and choosing **Save All**.

## A minimal example

A minimal program normally contains a safe starting pose, one or more motion instructions such as `MovJ` or `MovL`, and an `End` instruction. First validate each motion in simulation and at reduced speed.

{: .warning }
> Do not reuse taught positions blindly on the physical cell. Confirm the active tool, frame, payload, and surrounding workspace first.

## Variable scope and naming

Use the narrowest useful scope:

| Scope | Prefix | Intended use |
|:--|:--|:--|
| System | `S` | Default speeds and precision zones |
| Global | `G` | System-wide I/O, for example a gripper |
| Project | `P` | Values shared by project programs; avoid when local scope is sufficient |
| Local | `L` | Values used by one script; preferred for most variables |

Because the editor has limited autocomplete, start a variable name with its type, for example `I_counter` for an integer.

## Good practice: start a project from scratch

1. When connected to a real controller, first select **Upload from robot**.
2. Create the project, then save the workspace. By default, workspaces are stored in `C:\Estun\Editor\Workspaces`.
3. Define system defaults, then global/project variables only when shared access is genuinely needed.
4. Prefer local variables for values used by one program.

## Run a program

1. Load the program with the icon to its right.
2. Enable the robot motors.
3. Set the robot mode to **Auto**.
4. Press **Play**.

If **Safety door is not open** or **Start AutoRun failed** appears, see [the troubleshooting section](faq.html#safety-door-and-autorun-errors).
