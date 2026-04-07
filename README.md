# EDAcation Example Project

This example project for EDAcation walks you through the full FPGA workflow in VSCode, step by step, from synthesis to programming your board.
It can be used in your local VSCode instance as well as the web version.

The project is based on the [ULX3S Blink](https://github.com/ulx3s/blink) example.

## Setting up

Open this repository in VSCode. You can either clone it to your local PC, or click [this link](https://vscode.dev/github/EDAcation/example-project) to open it in vscode.dev.

VSCode should ask you to install the recommended extensions for this repository, which includes EDAcation. Click yes and install the extensions. If you don't see the notification, you can also manually install EDAcation [from the VSCode Marketplace](https://marketplace.visualstudio.com/items?itemName=edacation.edacation).

You should now see the 'EDA' icon in the left sidebar. If it doesn't show up, make sure that your [workspace is trusted](https://code.visualstudio.com/docs/editing/workspaces/workspace-trust#_trusting-a-workspace). EDAcation does not support untrusted workspaces.

You may receive another notification asking you to install more recommended extensions. We recommend installing these, because they enable various useful features of the extension.

## Opening the project

EDAcation is now installed and you have the project files, but the project has not been opened in EDAcation yet. Open the EDAcation menu
in the left sidebar and click the 'Open Project' button, then open the `blinky.edaproject` file in the root of the workspace. All settings
should be automatically imported.

## Have fun!

That's it! You now have a fully functional FPGA development environment. Feel free to click around to see what EDAcation can do. If you don't know where to start, we have some suggestions:

- Click the 'RTL' button to inspect the Blinky circuit
- Click the 'Synthesize' button to synthesize the design, then click 'Place & Route' to open the FPGA viewer
- If you have an ULX3S with an ECP5-12k FPGA on board, click the 'Flash to FPGA' button to run the Blinky circuit on your FPGA
    - Note: this may require driver installation on Windows or udev rules on Linux
- Play around with the project settings! You can open it by clicking the cogwheel in the 'Configuration' menu.

If you only have access to other FPGAs, you can try to configure EDAcation to work with your board by modifying the following settings in the project configuration:
- Set the correct vendor, family, device and package settings in the 'General' tab
- Modify the 'Target board to flash' option in the 'Flashing' tab
- Update the `pins.lpf` pin constraints file to point to the correct I/O pins, or add your own file and mark it as 'active'

## Further resources

Consult the [EDAcation docs](https://edacation.github.io/) for more information.
