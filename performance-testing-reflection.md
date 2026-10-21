### Research & Learn

1. What are the key factors that impact app performance (CPU, memory, network, database queries, etc.)?
- CPU: The phone or computer's processing power. If the app requires too much processing, it may become slow.
- Memory (RAM): The space the app uses to run. If memory is low, the app may freeze or crash.
- Network: A slow or unstable internet connection can make pages load slowly or prevent data from loading.
- Database queries: These are requests the app makes to retrieve or save information. If they take too long, the app may respond slowly.
- Images and other files: Large files can take longer to load and may slow down the app.
- Background activities: Other apps or processes running at the same time can affect performance

2. How can QA testers measure app speed and responsiveness?
QA testers can measure performance by:
- Checking how long the app takes to open
- How quickly pages load
- How fast buttons respond
- How long it takes to complete an action. 
They can also observe whether the app freezes, crashes, or becomes slow when performing several tasks.

3. What tools can be used for basic performance testing (e.g., Chrome DevTools, Lighthouse, mobile profiling tools)?
- Chrome DevTools: Helps testers check page loading times, network requests, and how the browser uses resources.
- Lighthouse: Checks website performance and provides suggestions for improvement.
- Android Studio Profiler: Helps testers examine an Android app's CPU, memory, and network usage.
- Xcode Instruments: Helps examine the performance and resource usage of iOS apps.

4. What common performance issues appear in web apps vs. mobile apps?
Web apps:
- Pages take too long to load.
- Buttons or links respond slowly.
- Pages become unresponsive when too much data is loaded.
- Websites perform differently across browsers.

Mobile apps:
- The app freezes or crashes.
- The battery drains quickly.
- The app uses too much memory.
- The app becomes slow on older phones.
- Features stop working properly when the network is weak.

5. How can QA test app behavior under high load or low resources (low RAM, slow CPU, unstable network)?
QA testers can simulate situations where the app has limited resources or many users are using it at once.
- Low RAM: Run the app on a device with limited available memory and check whether it freezes or crashes.
- Slow CPU: Test on an older or less powerful device to see whether the app remains responsive.
- Unstable network: Use network throttling or disconnect and reconnect the internet to see how the app behaves.
- High user load: Use load-testing tools to simulate many users accessing the app simultaneously.


### Reflection

1. How would you test Focus Bear’s performance on an older device or a slow internet connection?
I would install Focus Bear on an older device and check how quickly it opens, how smoothly its features work, and whether it freezes or crashes. I would also test it with a slow or unstable internet connection to see how long it takes to load data and whether its features continue to work properly.

2. If a user reports that the app feels slow, what steps would you take to investigate?
I would ask the user when the app becomes slow and what they are doing at the time. I would check their device, operating system, app version, and internet connection. Then, I would try to reproduce the problem under similar conditions, record any delays or errors, and share my findings with the developers.

3. What performance optimizations could help Focus Bear run smoothly on low-end devices?
- Stop unnecessary activities running in the background.
- Make sure the app doesn't use too much of the phone's memory or processing power.
- Make images and files smaller so they load faster.
- Make it easier and faster for the app to load and save information.
- Reduce how often the app needs to connect to the internet.
- Ensure the app can still respond properly when the internet is slow, without freezing or crashing.