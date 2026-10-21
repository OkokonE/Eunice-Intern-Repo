### Research & Learn

1. What are the key differences between testing on real devices vs. emulators/simulators?
Real devices are actual phones, tablets, or computers. Testing on them helps you see how the app works in real life.
Emulators and simulators are programs that imitate phones or other devices on a computer. They help testers check how an app works without needing to own every device.

Real devices give more realistic results, while emulators and simulators are useful for testing different devices quickly and at a lower cost.

2. How does OS version fragmentation impact testing?
An app might work properly on a newer version but have problems on an older one. Testers need to check different OS versions to make sure the app works for as many users as possible.

3. What tools can help with cross-device and cross-browser testing?
- BrowserStack: Allows testers to check websites and apps on different devices and browsers online.
- Sauce Labs: Provides access to different devices and browsers for testing.
- Chrome DevTools: Helps testers check how a website looks and behaves on different screen sizes.
- Android Studio Emulator: Allows testers to test Android apps on virtual Android devices.
- Xcode Simulator: Allows testers to test iPhone and iPad apps on a Mac without needing every physical device.

4. What are common device-specific issues that testers should watch for?
- An app works on one phone but crashes on another.
- Text or buttons appear too large, too small, or out of place.
- Some features do not work properly on older operating systems.
- The app drains the battery quickly or makes the phone heat up.
- The app becomes slow or freezes on phones with limited memory.
- Notifications, permissions, or other features behave differently across devices.

5. How can QA handle testing on a variety of devices without access to all of them?
I would test on the devices available to me and use emulators or simulators to check other device types. 
I would also use online services such as BrowserStack to access different devices and browsers remotely. 
I would prioritise popular devices, older operating systems, and devices with different screen sizes.


### Reflection

1. What unique bugs could occur on Android vs. iOS, or Windows vs. macOS?
Some bugs occur because devices and operating systems work differently.

Android vs. iOS: An app might have notification problems on Android but work properly on iOS. Permissions, screen layouts, and background activities may also behave differently.

Windows vs. macOS: An app might work properly on Windows but have display issues, keyboard shortcut problems, or compatibility issues on macOS.

As a QA tester, I would test the app on different operating systems to identify these differences.

2. If a bug is reported only on an older OS version, how would you approach testing it?
I would try to test the app on a device running the affected OS version. I would follow the reported steps to see if I could reproduce the bug and compare the results with a newer OS version. I would record my findings and share them with the developer to help identify the cause.

3. What strategies can you use if you don’t have direct access to a specific device for testing?
I would use an emulator or simulator to imitate the device.