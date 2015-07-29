--- How To: Build and Sign an App to Install via iTunes ---
1. In the root directory of the project, type the following to build the app:
```xcodebuild -target MyTestApp -sdk iphoneos8.4 -configuration Release```
2.Then, to package the app, type:
```/usr/bin/xcrun -sdk iphoneos PackageApplication -v MyTestApp/build/Release-iphoneos/MyTestApp.app -o MyTestApp.ipa```
3. ```MyTestApp.ipa``` is now ready to be dragged into the iTunes' App section and installed on a connected device.



--- Xcode Concepts ---
- An Project contains all the resources required to build one or more products.
- A Target contains the instructions needed to build a product from a set of files in the project.
- A Scheme specifies which targets, build configurations (e.g. Debug or Release) and executable configurations is active at a given time.
  A Scheme also defines which tests to perform.


