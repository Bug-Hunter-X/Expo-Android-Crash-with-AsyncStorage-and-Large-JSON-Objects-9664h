# Expo Android Crash with AsyncStorage and Large JSON Objects

This repository demonstrates a bug encountered in an Expo project where the app crashes unexpectedly on certain Android devices when using AsyncStorage with large JSON objects. The crashes were inconsistent and difficult to debug due to unhelpful error messages.

## Bug Description

The app crashes on some Android devices when using AsyncStorage.setItem() with large JSON objects. The issue seems to be related to memory management or limitations within AsyncStorage on specific Android versions or devices.

## Reproduction Steps

1. Clone this repository.
2. Run the app on an Android emulator or device.
3. Attempt to store a large JSON object using AsyncStorage.setItem().
4. Observe the app crashing on some devices.

## Solution

The solution involves splitting large JSON objects into smaller chunks before storing them in AsyncStorage. This reduces the memory footprint and prevents the app from crashing. The bugSolution.js file shows the improved implementation.

## Contributing

Contributions are welcome! If you have any suggestions or improvements, please feel free to open an issue or pull request.