[Download these files as a ZIP file](http://github.com/cis1951/hw3-gpx/zipball/main)

GPX files for [HW3: Penn Dining Scavenger Hunt](https://www.seas.upenn.edu/~cis1951/24fa/assignments/hw/hw3/). You can use these to simulate a device's location using these steps:

> If you don't have access to a physical device or don't feel like making the trek to each of the dining halls, worry not! Xcode lets you simulate your device's location using a GPX file. To use it:
> 
> 1. [Download the GPX files from the link above.](https://github.com/cis1951/hw3-gpx)
> 2. Run your app in the simulator or on a device.
> 3. In Xcode's menu bar, go to **Debug > Simulate Location > Add GPX File to Project...** and select the GPX files for each of the dining halls. (You can shift-click to select multiple files at once.)
> 4. Once you've added the GPX files, you can select them from the **Simulate Location** menu to simulate your device's location.
> 
> Note that if you're running on a physical device, location simulation will only work while your app is actively being run from Xcode. Running your app from the home screen will use the device's actual location.
> 
> (You can also use the **Features > Location** menu in the Simulator, but doing it through Xcode will let you use our GPX files.)

We also provide a `Locations.swift` file, which will let you easily use the coordinates in your program's code. Once you copy it to your project, you can access a dining hall's coordinates like so:
```swift
let diningHall = DiningHall(name: "1920 Commons", coordinates: CLLocationCoordinate2D.commons, /* etc. */)
```