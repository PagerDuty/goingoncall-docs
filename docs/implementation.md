![Implementation Suggestions](/assets/images/headers/OnCall-Implementation.png)

If you and your team are completely new to on-call, here are some suggestions of tasks to help guide you in the process.

## Take Stock of Your Alerts

- Manage Alert Fatigue!
	- [8 Ways to Reduce Alert Fatigue](https://www.pagerduty.com/blog/reduce-alert-fatigue/)
	- [Cutting Alert Fatigue in Modern Ops](https://www.pagerduty.com/blog/cutting-alert-fatigue-modern-ops/)
- Make sure all of your alerts are actionable.
- Verify that all alerts have documentation.
- If any alerts indicate issues with external dependencies, liaise with your peers on those teams for shared responsibility.
- Clear noisy alerts as much as possible. Prioritize permanent fixes for troublesome issues.
- Disable alerts for issues that can’t be fixed and don’t have customer impact.

!!! tip
		Ideally, every alert that comes through to your team should be something they can fix

## Prioritize Projects

- Start your on-call journey with your most stable services.
- Prioritize customer-facing services.
- Decide which services require what level of response, and don’t over-assign high priorities to services that don’t require them.

!!! tip
		When the pager goes off at 3am, it better be worth it.

## Leverage Traditional NOCs

If your organization already relies on a 24x7 NOC for monitoring status and responding to alerts, you might migrate to your team on-call in phases. There are two major methods for doing this:

- Assign your team as escalation or “Level 2” for your services and allow the NOC to respond as “Level 1.”
- Divide common alerts into tasks that the NOC can easily manage and those which require your team’s access and expertise. You might make use of [PagerDuty Rundeck](https://rundeck.com), for example, to give the NOC team access to certain tasks in your environments.

Over time, your team can then pick up more of the alerts as they get acclimated to being on call.

## Be Flexible

- There’s no rule that on-call shifts need to be a full calendar week. Split things up in ways that make sense for your team.
- If you have folks in different timezones, consider using a model that puts team members on-call most of their day time and limit their sleep-time duties.
- If you don’t need coverage on weekends or evenings for certain services, don’t notify responders for those alerts. Leave them until work hours, and make it a practice for the primary on-call to clear the queue every morning.
- Try to lengthen the time between shifts for any individual. If you have a small team, work with peers with similar services to determine if there is enough shared knowledge to share a rotation.

## Establish Good Behaviors

Give your team members just a few guidelines to help them adjust to being on-call. This could include things like:

- Setting standards for alert response times and work with your team to meet them. Using [MTTA and MTTR](/people/#responsibilities) will help.
- Committing to being responsive, and communicate when assistance is needed.
- Don’t hesitate to escalate.
- Sober on-call.

