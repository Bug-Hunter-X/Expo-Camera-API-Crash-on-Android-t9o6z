# Expo Camera Crash on Android

This repository demonstrates a bug in the Expo Camera API where the camera preview may freeze or crash on certain Android devices. The issue appears to be related to camera switching and multiple picture capture. This example includes a solution to mitigate this problem.

## Bug Reproduction

1. Run the `bug.js` file (requires Expo Go).
2. Observe the camera preview.
3. Rapidly switch between the front and rear cameras several times, or take multiple pictures.
4. Note that the preview may freeze or crash on some Android devices.

## Solution

The `bugSolution.js` file demonstrates a solution involving using `Camera.takePictureAsync` with a delay before switching to the next operation. This delay may prevent the sudden changes that trigger the crash in some devices. This is not a perfect solution and more robust approaches might be needed for critical applications.

## Contributing

Contributions are welcome!