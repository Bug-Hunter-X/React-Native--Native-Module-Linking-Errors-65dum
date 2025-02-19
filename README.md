# React Native Native Module Linking Issues

This repository demonstrates a common React Native error related to missing or incorrectly linked native modules.  The `BuggyComponent.js` file shows the problematic code, while `FixedComponent.js` provides the solution.

The error typically manifests as `Unable to resolve module` or `Invariant Violation: requireNativeComponent: ... was not found`. This happens when a library requiring native code (e.g., a camera library, geolocation library) isn't properly configured in the native Android/iOS projects.

**Steps to reproduce the bug (BuggyComponent.js):**
1. Run the app.
2. Observe the error related to the missing native module.

**Solution (FixedComponent.js):**
The solution involves ensuring correct installation and linking of the native module for your specific environment (Android and iOS).  See the `FixedComponent.js` file for example implementation and code comments indicating crucial steps.  This may involve using tools like `react-native link` or manually configuring the native project files.  Consult the documentation for the specific native module you're using for detailed instructions.