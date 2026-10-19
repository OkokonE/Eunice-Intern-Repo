### Research & Learn

1. What are the best practices for communicating bugs to developers?
- Use a clear title for the bug report.
- Provide a detailed description of the bug.
- Include steps to reproduce the bug.
- State the expected result.
- State the actual result.
- Provide evidence, such as a screen recording or screenshot.
- Include device details.
- Specify the operating system version.

2. How can QA provide useful feedback without overwhelming developers?
- Report bugs with clearly stated severity and priority levels. This helps developers determine which issues to address first.
- Keep bug reports clear and concise, avoiding irrelevant information.

3. What are common misunderstandings between testers and developers, and how can they be avoided?
- Different expectations about a feature's behaviour: This can be avoided by referring to the acceptance criteria, user stories, and other documentation related to the feature.
- Different priorities: Something a tester considers a major issue may be considered minor by the developer. This can be avoided by politely and professionally explaining the severity and impact of the bug to the developer.

4. How does a good vs. bad bug report conversation look like?
**Bad Conversation**
QA: The app is not working.
Developer: What exactly is the problem?
QA: I can't use the app.

Why it is bad: The QA tester is not specific about what is wrong with the app, making it difficult for the developer to understand and investigate the issue.

**Good Conversation**
QA: While testing the Focus Bear app on my Samsung mobile phone running Android 14, I observed that whenever I started a focus session, it automatically stopped whenever I left the focus session page. The expected behaviour is for the focus session to continue even when I leave the focus session page.
I have attached a screen recording showing the exact steps I took.
Developer: Thanks for the details. I'll check the expected behaviour and investigate.
QA: Thank you. I'll also test the behaviour again after the change and confirm whether the issue is resolved.

Why it is good: The tester provides evidence, clearly explains the observed and expected behaviour, and agrees to verify the fix.

5. When should QA escalate an issue if it’s not being addressed?
QA should escalate when an issue presents a significant risk and is not receiving appropriate attention through the normal process.
Examples include:
- A critical defect affecting login, core functionality, data integrity, privacy, or security.
- A bug that blocks users from completing an essential task.
- A serious issue that remains unresolved close to a release deadline.
- A defect repeatedly postponed without an agreed decision or mitigation.
- A disagreement about expected behaviour or severity that the immediate team cannot resolve.

### Reflection

1. If a developer says they can’t reproduce a bug, how would you respond?
Assuming the bug report is detailed and clear, with screen recordings, device details, and the operating system version, I would ask the developer for a meeting where I could share my screen and reproduce the bug. This would help the developer observe the issue firsthand and investigate it further.

2. How can testers avoid blaming developers while still pushing for bug fixes?
- Maintain the mindset that the developer is a team member, not an enemy.
- Communicate politely and professionally.
- Make bug reports clear and detailed, providing enough information to help developers understand and fix the issues.

3. What are some techniques for keeping bug discussions constructive and professional?
- Use clear, respectful, and factual language.
- Provide evidence and specific steps to reproduce the bug.
- Listen to the developer's perspective and remain open to feedback.
- Ask questions and clarify misunderstandings instead of making assumptions.
- Focus on finding a solution rather than assigning blame.
- Follow up on unresolved issues professionally.
- Acknowledge the developer's efforts and retest the fix to confirm that the issue has been resolved.