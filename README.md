# Hot Wheels Unleashed Mod Kit

A Set of Mod Development Tools for Hot Wheels Unleashed

## Prerequisites

These need to be installed in order to use the tools:

- [Python 3.8+](https://www.microsoft.com/en-us/p/python-38/9mssztt1n39l)
- Unreal Engine 4.22

You can download Unreal Engine for free through the Epic Games Store app, just **make sure to select version 4.22.x**. Using a different version of UE4 will cause all sorts of strange issues.

## Setup

Edit the text files in the `Tools/user_settings` folder to configure the tools:

| File                    | Description   |
| ----------------------- | ------------- |
| editor_directory.txt    | This contains the path to the folder where the Unreal Editor executables are. |
| package_output.txt      | This contains the path to the .pak file that the package.bat tool creates. |

Setting the package_output path to a file in your `~mods` folder is recommended to make testing the mod easy.

### Packaging

To test your mod, you can run the `package.bat` tool to create a .pak file. If the tool is configured to place the .pak file in your `~mods` folder, you can start the game as soon as it finishes.

To package your mod for release, use the `Tools/pack_compressed.bat` tool instead. This tool will create a `compressed_pack.pak` file in your `Tools` folder. This .pak file usually takes slightly longer to create, but the file size should be much smaller. You can rename the .pak file to whatever you want.
