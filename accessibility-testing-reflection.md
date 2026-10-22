### Research & Learn

1. What is WCAG (Web Content Accessibility Guidelines), and what are its key principles?
WCAG stands for Web Content Accessibility Guidelines. These are guidelines that help developers make websites and apps easier for everyone to use, including people with disabilities.

WCAG has four main principles, known as POUR:
- Perceivable: Users must be able to see or hear the information. For example, images should have descriptions for people who cannot see them.
- Operable: Users must be able to operate the app. For example, someone should be able to navigate using a keyboard without a mouse.
- Understandable: The app should be easy to understand. For example, buttons and instructions should be clear.
- Robust: The app should work well with different assistive technologies, such as screen readers.

2. How do screen readers (e.g., NVDA, VoiceOver, TalkBack) work, and how can QA test with them?
A screen reader is a tool that reads what is on a screen aloud. It helps people who are blind or have difficulty seeing use apps and websites.

Examples include:
- NVDA: A free screen reader for Windows computers.
- VoiceOver: A built-in screen reader for Apple devices.
- TalkBack: A screen reader for Android phones.

How QA can test with them:
a. Turn on the screen reader.
b. Open the app or website.
c. Move through buttons, links, images, and text.
d. Check whether it reads the correct information and explains what each button does.
e. Check whether you can complete tasks, such as filling out a form or starting a focus session, without relying on sight.

For example, if a button only shows a picture of a clock, the screen reader should explain what the button does rather than simply saying “button.”

3. What are some common accessibility issues in apps and websites?
Common problems include:
- Missing image descriptions: A screen reader cannot explain what an important image shows.
- Poor colour contrast: Text is difficult to read because its colour is too similar to the background.
- Missing button labels: Users cannot tell what a button does.
- Keyboard problems: Some features only work when using a mouse.
- Small text: Users with poor eyesight struggle to read it.
- Confusing error messages: Users are not told what went wrong or how to fix it.
- Poor navigation: Users get lost or cannot tell which part of the page they are on.

For example, if a website displays an error in red but provides no explanation, some users may not understand the problem, especially if they cannot distinguish the colour.

4. How can you test keyboard navigation and focus management?
This means checking whether someone can use an app or website without a mouse, using only a keyboard.

You can test it by:
1. Pressing Tab to move from one button or link to the next.
2. Pressing Shift + Tab to move backwards.
3. Pressing Enter or Space to activate buttons.
4. Checking that you can see which item is currently selected. This is called keyboard focus.
5. Checking that the selection follows a sensible order.
6. Opening a pop-up window or form and checking that you can move through it and leave it without getting stuck.

Example: When testing Focus Bear, I would check whether I can use the keyboard to start, pause, and end a focus session without needing to click with a mouse.

5. What tools can help automate basic accessibility checks?
These tools automatically scan websites for common accessibility problems.
a. Lighthouse: Checks a website for common issues and produces an accessibility report.
b. axe DevTools: Finds common accessibility issues, such as missing form labels and certain contrast problems.
c. WAVE: Highlights common accessibility issues directly on a webpage, making them easier to spot.

These tools can find many common problems, but they cannot detect everything. QA testers must still check the app manually, use the keyboard, and test with screen readers.


### Reflection

1. How would you test if Focus Bear is usable with a screen reader?
I would turn on TalkBack on my Android phone, and try using Focus Bear without looking at the screen.
I would also check if it reads my to-do list correctly and whether I can navigate through reminders and routines without getting stuck.

2. What accessibility barriers could affect someone with ADHD or Autism using the app?
As a QA tester, I should check whether Focus Bear allows people with different needs to use the app comfortably. I would look for features that help users control distractions, understand what is happening on the screen, and customise the app to suit their preferences.

3. If a developer says "this doesn't impact most users", how would you advocate for fixing an accessibility issue?
I would explain that even if the problem affects only a small number of users, it can prevent those users from using the app properly. I would demonstrate the issue, provide evidence, and explain how it affects the user.

For example, if a screen reader cannot identify the button for ending a focus session, a blind user may struggle to end the session independently. I would explain the impact and suggest adding a clear button label.