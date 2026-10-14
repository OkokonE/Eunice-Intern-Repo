### Research & Learn

1. What is the difference between a scheduled release, a rollback, and a hotfix?
- Scheduled release: This is a planned deployment of new features, improvements, or bug fixes at an agreed time. QA tests the changes before release and verifies the application is functional after deployment.
- Rollback: This reverts to a previous stable version when a deployment causes serious problems. QA checks that the previous version works correctly and that important data or functionality has not been affected.
- Hotfix: An urgent change released to fix a critical problem in a live application, such as a login failure or a security vulnerability. QA performs focused testing to confirm the fix works and does not introduce other serious issues.

The main difference is that a scheduled release is planned, a rollback restores an earlier version, and a hotfix addresses an urgent issue in the live app.

2. What should QA test immediately after a deployment?
I would perform smoke testing to confirm that the application is available, stable and its core funcionalities still work.
Key checks include:
- Availability: Can users open the application and sign in?
- Critical workflows: Can users complete essential actions without errors?
- API health: Are key requests returning expected status codes and responses?
- UI checks: Are pages, buttons, forms, and navigation working correctly?
- Data integrity: Are user data and saved settings still present and correct?
- Compatibility: Does the application work on supported browsers and devices?
- Monitoring: Are there unusual increases in crashes, failed requests, or response times?

QA should also verify that the intended version was deployed.  

3. How does QA handle hotfix testing when a critical bug is found after release?
When a critical bug is discovered in production, QA needs to validate the urgent fix quickly without skipping essential checks.
1. Understand the impact: Confirm the affected feature, severity, affected users, and reproducible steps.
2. Verify the fix: Test the original failure scenario to confirm the problem is resolved.
3. Run targeted regression tests: Check nearby features and workflows that could be affected by the change.
4. Check critical functionality: Run smoke tests for essential functions such as login, navigation, and saving data, as relevant to the application.
5. Validate the deployed fix: Confirm the correct version is live and the bug no longer occurs in the production environment.
6. Monitor after release: Watch for recurring errors, crashes, and other unexpected behaviour.
The testing scope should be risk-based: test the most important scenarios first, while making the time constraints and any remaining risks clear to the team. 

4. What strategies help prevent new bugs from being introduced in urgent fixes?
- Keep the change small: Fix the specific problem instead of making unrelated changes.
- Review the code: Have another developer review the fix when feasible.
- Run automated tests: Execute relevant unit, integration, and regression tests.
- Test edge cases: Check unusual inputs and scenarios related to the original defect.
- Use version control: Track the changes and make it possible to identify or revert them.
- Deploy gradually: Where the infrastructure supports it, release to a small group of users first and expand after monitoring.
- Prepare a rollback plan: Know how to restore a stable version if the fix causes further problems.
Google's Site Reliability Engineering guidance recommends small, automated, reproducible releases and gradual rollouts to reduce the impact of defects. 

5. How do other teams approach post-release monitoring?
Teams commonly combine automated monitoring, user feedback, and targeted testing to check whether a release is behaving as expected.
- Error and crash monitoring: Track exceptions, failed requests, and application crashes.
- Performance monitoring: Watch response times, loading speed, and resource usage.
- Logs and alerts: Review application logs and configure alerts for unusual error rates.
- Canary releases: Expose a small percentage of users to a new release before expanding it.
- Health checks: Verify that essential services and workflows remain available.
- User feedback and support tickets: Look for problems users report after an update.
- Incident reviews: Investigate significant failures and identify improvements for future releases.
For example, a team might release a new version to 10% of users, monitor error rates and response times, and expand the rollout if the results are healthy. If serious problems appear, the team can pause the rollout or roll back. The exact percentages and monitoring period depend on the product and its risk profile.

### Reflection

1. If a release goes live and users immediately report issues, what should QA do?
QA should respond quickly, assess the severity and impact of the reported issues, and help the team determine the next steps.
- Gather information: Collect the affected feature, steps to reproduce, screenshots or recordings, device/browser details, and error logs.
- Assess severity: Determine whether the issue affects a critical function, many users, or a smaller part of the application.
- Reproduce the issue: Verify the reported behaviour in the production environment when safe to do so.
- Inform the team: Notify the developer, product manager, and relevant stakeholders, especially if the issue is critical.
- Support the response: Help validate a hotfix or recommend a rollback if the release causes serious disruption.
- Verify and monitor: After the fix or rollback, retest the affected functionality and check whether the problem has stopped occurring.
The priority is to protect users and restore stable functionality while gathering enough evidence to make informed decisions.

2. What’s the best way to prioritize testing when working under time pressure for a hotfix?
I would use a risk-based testing approach, focusing first on the application's most critical functions.
- Test the critical bug first: Confirm that the original issue is fixed.
- Test high-risk related areas: Check other features that may be affected by the code change.
- Run smoke tests: Verify that essential workflows still work.
- Check common edge cases: Test invalid inputs, error handling, and relevant boundary conditions.
- Automate where possible: Run existing automated tests to get quick feedback.
- Communicate remaining risks: Clearly tell the team which tests passed, failed, or could not be completed before release.
For example, if a hotfix addresses a login failure, I would test successful login, invalid credentials, and relevant authentication flows first, then check related functions such as logout and password reset.
The goal is to gain the highest possible confidence in the fix within the available time, rather than trying to test everything equally. 

3. How can QA help ensure stability in production while still allowing fast bug fixes?
QA can help by combining quick, focused testing with safeguards that reduce the risk of a faulty release reaching all users.
- Maintain automated regression tests for critical workflows so they can be checked quickly.
- Keep hotfixes small and focused to reduce unintended side effects.
- Use code reviews and CI checks to catch problems before deployment.
- Run smoke tests immediately after the fix is deployed.
- Use gradual rollouts or canary releases to expose the change to a small portion of users before expanding it.
- Monitor production metrics, including crashes, failed requests, and response times.
- Prepare a rollback plan so the team can restore a known stable version if the fix causes serious problems.
- Review incidents afterward and add regression tests to prevent the same issue from recurring.
