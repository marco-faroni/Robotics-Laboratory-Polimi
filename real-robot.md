---
title: Using the real robot
layout: default
nav_order: 7
---

# Using the real robot

## Start the robot cell

1. Turn on the main switch on the robot cabinet.
2. Wait until the Teach Pendant is ready.
3. Acknowledge any errors or warnings after understanding their cause.
4. Select **AUTO** or **TEACH** mode on the TP.

{: .warning }
> Do not acknowledge alarms or enable motors unless you have checked that the cell is safe and understand the alarm.

## Connect Estun Editor

1. Connect the PC to **Ethernet 1**.
2. Configure a static IPv4 address: `192.168.6.XXX`, netmask `255.255.255.0`, where `XXX` is 1–254 and unused.
3. Verify that the controller at `192.168.6.63` responds to ping.
4. In Estun Editor, select **Real Controller** and enter the robot IP address.

Network settings on the TP are under **System → Settings → Network**.

## Use the virtual TP with the real robot


The virtual TP on Estun Editor can act as a surrogate of the real TP. 
However, the usage of the virtual must be consistent with the robot setting in order to work. 

Consider the following: 

1. If the real TP is ON, you can connect to the Estun Editor and start programs (by pressing Play), but you will not be able to open the virtual TP.
2. To use the virtual TP, exit the real TP through **System → Settings → SystemSet → Menu → System Settings → System Management → Exit**. 
3. It is possible to completely disconnect the physical TP and use only the virtual one. You need a special connector to do so.

{: .important }
> When Option 2 is used, manual jogging still requires pressing the deadman switch on the physical TP.

{: .important }
> Replacing the physical TP entirely requires disconnecting it and fitting a special connector. **Ask the instructor before attempting this**.

## Upload and download code

- Select **Upload from robot** to copy the controller content into Estun Editor.
- Select **Save All** to save editor changes to the controller.

Synchronise before editing an existing controller project to avoid overwriting recent controller-side work.

## Run a program

After loading the program, use one of these methods:

- **Real Teach Pendant:** select **Auto (A)**, then press **Start**.
- **External buttons:** select **Auto-External (AE)**, then press the green button.
- **Estun Editor:** select **Auto-External (AE)**, then press **Start** in the editor.

If **Safety door is not open** or **Start AutoRun failed** appears, see [FAQs](faq.html#safety-door-and-autorun-errors).
