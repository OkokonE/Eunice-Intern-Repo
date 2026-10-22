### Research & Learn

1. What are logs, and how do they help with debugging?
Logs are records of what happens inside an app or website. They can show what the app was doing, when something happened, and whether an error occurred.

Logs can be likened to a diary that an app keeps about its activities.

Example: While testing Focus Bear, you click Start Focus Session, but nothing happens. The logs might show that the app tried to start the session but failed to connect to the server.

Logs help QA testers and developers understand what went wrong and investigate the cause instead of guessing.

Common types of logs include:
- Info: Records normal activities.
- Warning: Indicates something unusual that may cause a problem.
- Error: Shows that something failed.
- Debug: Provides detailed information to help investigate problems.

2. How can you capture logs from a web app (browser DevTools)?
- Open the website you want to test.
- Right-click the page and select Inspect.
- Click the Console tab to look for errors and warnings.
- Click the Network tab to check requests sent between the website and its server.
- Repeat the action that caused the problem.
- Take screenshots or save the relevant logs so you can share them with the developer.

3. How can you capture logs from a mobile app (Android/iOS debugging tools)?
**Android**
You can use Logcat in Android Studio.
1. Connect your Android phone to a computer, or use an Android emulator.
2. Open Android Studio and launch the app.
3. Open View → Tool Windows → Logcat.
4. Reproduce the problem on the phone.
5. Look for error messages around the time the problem occurred and save the relevant details.
Logcat shows app and system messages, including information that can help explain why an app crashed.

**iPhone (iOS)**
You can use Console on a Mac or the debugging tools in Xcode.
1. Connect the iPhone to the Mac.
2. Open the Console app or Xcode debugging tools.
3. Select the connected device, where applicable.
4. Open the app and reproduce the problem.
5. Look for relevant errors and save the details.
These tools help you investigate crashes and other problems that occur on Apple devices.

4. What are some common error messages and log patterns testers should recognize?
Error or pattern	            Simple meaning
404 Not Found	                The requested page or resource could not be found.
401 Unauthorized	        The user may need to log in or provide valid authentication.
403 Forbidden	                The user does not have permission to access something.
500 Internal Server Error	Something went wrong on the server.
Timeout	                        The app waited too long for a response.
NullPointerException	        The program tried to use something that had no value when it expected one.
Connection refused	        The connection to the intended service was rejected.
Crash or FATAL	                The app or a part of it encountered a serious failure.

5. How do network requests in browser DevTools help diagnose API failures?
A network request is when an app or website sends a message to a server to get information or perform an action.
An API allows the app and server to communicate. For example, Focus Bear may send a request to save a user's routine.

To investigate a failed action:
a. Open DevTools and select Network.
b. Reproduce the problem.
c. Find the request related to that action.
d. Check its status code, request details, response, and timing.
e. Use the information to help identify where the problem may have occurred.

The Network tab helps testers see whether a request was sent, what response came back, and how long it took.



### Reflection

1. If Focus Bear crashes on a user’s device but not on yours, how would you use logs to investigate?
I would ask the user for details about their device, operating system, app version, and the steps they took before the app crashed.

I would then ask for the error logs and check what happened just before the crash. I would try to reproduce the problem using the same device or a similar environment and compare the logs with mine to identify the difference.

2. What are some useful log messages that should be included when reporting a bug?
- Error messages: Show what went wrong.
- Timestamps: Show when the problem happened.
- Crash reports: Explain when and how the app crashed.
- Network errors: Show whether the app failed to communicate with the server.
- API responses: Show what the server returned.
- Device and app details: Help identify whether the problem is related to a particular device or app version

3. If an API call returns an unexpected response, what steps would you take to analyze the issue?
I would first open the browser's DevTools and go to the Network tab to find the API request that failed.

Then I would:
a. Check the status code to see whether the request succeeded or failed.
b. Check the request details to confirm that the app sent the correct information.
c. Check the response to see what the server returned and whether it matches what was expected.
d. Check the error logs for clues about what went wrong.
e. Repeat the test to see whether the problem happens consistently.
f. Document the findings with screenshots, relevant logs, and steps to reproduce the issue.

For example, if Focus Bear tries to save a routine but the API returns an error, I would check whether the request contained the correct data and whether the server returned a useful error message.