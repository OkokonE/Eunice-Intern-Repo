### Research & Learn

1. What steps should QA take when a customer reports a bug that can’t be easily reproduced?
I would first gather as much information as possible about the reported issue, including the steps the customer took, and how frequently the problem occurs. I would check the device, operating system, app version, browser, and network conditions. Next, I would try to reproduce the issue using the same conditions and investigate any available logs or error messages. If I still could not reproduce it, I would document my investigation, request additional evidence, and collaborate with the developer and customer support team. I would not dismiss the report simply because I could not reproduce it immediately.

2. What information should QA request from customer support to help diagnose an issue?
I would ask customer support for:
- A clear description of the problem and the steps the customer took.
- The expected result and what actually happened.
- The date and approximate time the issue occurred.
- The device model, operating system, app version, and browser version, where applicable.
- How frequently the issue occurs and whether it affects other users.
- Screenshots, screen recordings, error messages, or available logs.

3. How can logs, screenshots, and error messages help with bug reproduction?
Logs, screenshots, and error messages help identify what went wrong and provide evidence that can help reproduce a bug, even when the person who reported it is unavailable.

4. When should QA recommend adding more logging to capture hard-to-reproduce issues?
I would recommend adding more logging when I cannot reproduce a reported bug or when the available information is insufficient to identify its cause.

During an internship in 2023, another tester logged a bug that I was asked to verify, but I couldn't reproduce it because the issue occurred on the web application while I was testing the mobile app. This experience taught me the importance of confirming the affected platform and gathering sufficient information before drawing conclusions. If the issue remained difficult to reproduce after checking the correct platform, I would recommend additional logging to help identify its cause.

5. How do other teams handle "Cannot Reproduce" customer bugs effectively?
Other teams handle "Cannot Reproduce" customer bugs by reviewing the bug report, gathering more information from customer support, and checking whether the issue was tested on the correct platform and environment. 


### Reflection

1. How would you report a bug that only happens occasionally?
I would clearly describe the bug and include the steps I took, the device details, the operating system version, and any available screenshots or screen recordings.
I would also mention how often the bug occurs and under what conditions I observed it. I would also add timestamp.

2. If a customer reports a crash but you can't reproduce it, what are your next steps?
I would ask for more information from the customer, including their device details, operating system version, app version, steps taken before the crash, and any error messages or screenshots. I would check the available crash logs and try to reproduce the issue under similar conditions. If necessary, I would work with the developer to investigate further.

3. If a developer marks a bug as "Not reproducible", what's your next step?
I would review the bug report to ensure that the reproduction steps and environment details are clear and complete.
I would then try to reproduce the bug again and provide additional evidence, such as a screen recording or logs. 
If the developer still cannot reproduce it, I would request a meeting to share my screen and demonstrate the issue.

4. When should you ask developers to add more logging, and what kind of logs would help?
I would ask developers to add more logging when a bug occurs intermittently, cannot be reproduced consistently, or lacks enough evidence to identify its cause. 
Useful logs include error messages, timestamps, API request and response details, and information about the user's actions before the issue occurred. 
These logs can help identify what happened and where the problem originated.

5. What are some common patterns in bugs that only occur for some users but not others?
- Device differences
- Operating system differences
- Network conditions
- Browser differences
- User-specific data
- Timing and sequence of actions