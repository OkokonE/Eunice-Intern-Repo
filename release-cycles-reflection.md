### Research & Learn

1. What are the typical stages in a software release cycle (development, testing, staging, production)?
- Development: Developers write the code and implement new features or fix existing issues.
- Testing: QA testers check the software to identify bugs and confirm that the changes work as expected.
- Staging: The software is deployed to a testing environment that closely resembles production. QA performs final checks before release.
- Production: The software is released to real users. QA performs smoke tests and monitors for issues after deployment.

2. How does QA work differ between a feature release and a hotfix?
A feature release introduces a new feature; functionality or improvement. QA performs functional testing, regression testing, integration and end-to-end testing, and other relevant checks to ensure the new feature works correctly without affecting existing functionality.

A hotfix is an urgent fix for a serious issue affecting users in production. QA focuses on testing the specific fix, checking the affected functionality, and performing targeted regression testing to ensure the fix does not introduce new problems. Because hotfixes are urgent, testing is usually more focused and time-sensitive.

3. What is version control (Git), and how does it impact testing?
Version control is a way of keeping track of changes made to software code. Git allows developers to save their work, compare changes, work on the same project, and return to an earlier version if something goes wrong.

How Git affects testing:
Git helps QA testers know which version of the software they are testing. It also helps them identify changes that may have caused a bug and check whether a developer's fix works correctly. This makes it easier to track problems and confirm that the right changes have been made.

4. What are Git branches, and why do testers need to be aware of them?
Git branches are separate lines of development that allow developers to work on features or fixes without directly changing the main codebase.
Imagine developers are working on Focus Bear. One developer wants to add a new feature, while another wants to fix a bug.Instead of making changes directly to the main version of the app, they can create separate branches to work on their tasks. When the changes are ready and approved, they can be added to the main version.

Why should QA testers know about branches?
- To test the correct version: You need to know which branch contains the feature or bug fix you are testing.
- To avoid reporting old bugs: A bug might already be fixed in one branch but still exist in another.
- To verify fixes: You can test the branch containing the fix to confirm that it works before the changes are added to the main version.

5. How does QA handle rollbacks if a release causes major issues?
If a release causes major issues, QA helps assess the impact and provides evidence to support the decision to roll back to the previous stable version. After the rollback, QA performs smoke tests to confirm that essential functionality is working again.

QA also verifies that the original issue is no longer present, checks for any side effects, and documents the incident. Once the underlying problem is fixed, QA tests the corrected version before it is released again.



### Reflection

1. How would you adjust your testing strategy for a major feature release vs. a small bug fix?
For a major feature release, I would test the new feature thoroughly and check that the existing features still work properly i.e function testing, regression testing, integration testing.
For a small bug fix, I would focus on checking whether the specific bug has been fixed. I would also test the related features to make sure the fix has not caused another problem.

2. If a developer says, “This bug only happens on an older branch,” how would you handle it?
I would ask the developer which version of the app has the problem. Then, I would check if the problem also happens in the latest version. If it only happens in the older version, I would inform the team and confirm whether that version still needs to be fixed.

3. Why is it important for testers to know which version of the app they are testing?
Knowing the version helps testers reproduce issues accurately, avoid reporting bugs that have already been fixed, and confirm that the correct changes are working as expected.