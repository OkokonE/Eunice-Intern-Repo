### Research & Learn

1. What is boundary value analysis, and why is it useful for testing?
Boundary value analysis means testing the limits of what a system allows. For example, if a password must contain between 8 and 20 characters, I would test passwords with 7, 8, 20, and 21 characters to see whether the app accepts or rejects them correctly.
Bugs often occur when users enter values that are just below or above an allowed limit.

Example: While testing a fintech app, I tested a Tier 1 customer's transfer limit of ₦50,000. Transactions above this amount were supposed to trigger a hold on the account. I tested a transfer of ₦50,001 and discovered that the transaction went through successfully without the account being placed on hold. This revealed a bug in the system's transfer limit validation.

2. What are common edge cases that testers should check in forms, authentication, and app flows?
- Forms: Leaving fields empty, entering invalid information, or entering more characters than allowed.
- Login and authentication: Entering the wrong password repeatedly, using an expired password reset link, or trying to log in with an empty field.
- App flows: Clicking a button repeatedly, losing internet connection while performing an action, or leaving a page before a task finishes.

3. How should QA test network failures, offline mode, and slow connections?
I would turn off the internet, use a slow connection, or disconnect and reconnect the network while using the app. I would check whether the app displays an appropriate message, saves information where expected, and recovers when the connection returns. I would also check that the app does not freeze, crash, or lose important information.

4. What happens when an app encounters an unexpected input or invalid data?
The app should handle the information properly instead of crashing or behaving unexpectedly. For example, if a user enters letters into a field that accepts only numbers, the app should reject the input and explain what is required.

5. How can error messages be tested to ensure they are helpful and user-friendly?
I would check that error messages explain what went wrong and tell the user what to do next. The messages should be clear, easy to understand, and free from confusing technical language.

For example, instead of displaying "Error 400," a login page could say, "Incorrect username or password. Please try again."

I would also check that the message appears at the right time, is easy to notice, and disappears or updates when the problem is corrected.


### Reflection

1. What edge cases could break Focus Bear’s onboarding flow?
- Losing internet connection while creating an account.
- Leaving the onboarding page before completing all the steps.
- Entering invalid information or leaving required fields empty.

2. If the app fails midway through a critical action, how should it behave?
The app should display a clear error message and avoid losing the user's information. If possible, it should allow the user to continue from where they stopped or retry the action.

3. How would you test for network instability and ensure Focus Bear handles it gracefully?
I would test Focus Bear using a slow internet connection, disconnecting the internet during an action, and reconnecting it afterward. I would check whether the app displays a helpful message, saves information where expected, and allows the user to retry when the connection returns. I would also check that the app does not freeze, crash, or lose important information.