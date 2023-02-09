# sokol_app.h Sample App (macOS and iOS)
This is an example of using `sokol_app.h` on macOS and iOS. Also uses `sokol_gfx.h` with Metal enabled. Just open the Xcode project, pick a target, and run. Works on any architecture.

The files in here are the bare minimum required for each platform. You can run this code on macOS in a fresh Command Line App with no changes, but iOS will need an `Info.plist` with a scene manifest key to prevent warnings.

If you have created an iOS App project through Xcode, you will need to remove all files except for the `Info.plist` with the required changes. You also need to remove the link to `Main.storyboard` by going to Build Settings and removing the string value from `UIKit Main Storyboard File Base Name`. You can optionally do this with `Launch Screen Interface File Base Name` too, but leaving it in doesn't throw an error.