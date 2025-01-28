# Uncommon Expo CLI Errors: File System Access and Native Modules

This repository demonstrates and provides solutions for uncommon errors encountered when using the Expo CLI, specifically those related to file system access and native module integration within the Expo managed workflow.

## Common Scenarios:

* **Permission Errors:** Accessing files or directories outside the project's allowed sandboxed environment.
* **Incorrect File Paths:** Using incorrect relative or absolute paths when working with assets or native modules.
* **Native Module Integration Issues:** Problems linking or configuring native modules correctly.

## Solutions:

* **Verify File Paths:** Ensure that you're using the correct paths when accessing files.  Use the `expo-file-system` API for reliable file system operations within Expo.
* **Check Permissions:** Understand the limitations of the Expo managed workflow and its sandbox environment. Avoid accessing system files or directories directly.
* **Configure Native Modules:** Follow the specific instructions and configuration steps for the native modules you're using. Properly link and integrate them into your Expo project.
* **Use Expo's APIs:**  Whenever possible, favor Expo's built-in APIs (like `expo-file-system`, `expo-image-picker`, etc.) for tasks that involve external resources or file system interactions. These APIs provide a safer and more consistent way to interact with those resources within the Expo environment.

## Reproducing the Bug

The `expoBug.js` file contains code that intentionally provokes these uncommon errors.  Follow the instructions in the comments within the file to trigger the specific error scenarios.