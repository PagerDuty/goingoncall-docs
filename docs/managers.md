![Recommendations for Managers](../assets/img/headers/OnCall-Managers.png)

## Etiquette and Setting Expectations

### Humane On-Call
Your team will probably have concerns about starting an on-call rotation. When we look at on-call behaviors in more traditional organizations, the expectations and implementations often leave the team members in a bad place—lots of alerts, low context, and alerts for services they can’t access or work on. 

When establishing on-call for a new team, set the expectations and some ground rules for your team. You might consider things like:

- Rescheduling around planned events at least a week in advance. No one wants to miss a child’s birthday party for on-call.
- Letting the backup know if you will be temporarily unavailable during a shift for things like subway commutes.
- Setting guidelines for folks to delay their workday if the responders were up overnight responding to alerts.
- Thinking about a process for rolling folks off the primary if an on-call shift has been especially stressful. For example, if a large issue lasts for several days, or if there are a lot of overnight issues.
- Erring on the side of creating more shifts of a shorter duration if your services are very noisy.

Preserving the health and well being of your team should be high on your list. 

!!! tip
		The PagerDuty platform can help you monitor the number of alerts your responders are getting, including alerts during “sleeping” hours in the [Operational Reviews](https://support.pagerduty.com/docs/operational-reviews) feature. 

### Team Participation

Part of avoiding burnout on your team and making on-call duties feel equitable is ensuring that all team members are participating equally. As a manager, you’ll want to keep an eye on how your team is managing things like shift swapping and schedule overrides. No one person should be taking a disproportionate amount of the on-call duties for any given team. 

It is also important to manage coverage for major holidays, and ensure that the same team members aren’t working every holiday or the same holiday year after year.

Your on-call platform provider probably provides some reports and other insights into how many hours your team has been on call, how many incidents they have responded to, and how many times they have been paged during sleep hours to help you manage team health. 

You also might want to talk to your team about expectations for their off time behavior when they are on call. Team members should be sober enough to work when they receive alerts. It probably feels like an awkward conversation to have, but it’s common enough it’s been a topic on [Ask a Manager](https://www.askamanager.org/2016/08/i-think-my-on-call-coworker-was-high-when-i-contacted-him.html). 

### Attrition
It is absolutely possible that a new on-call team might lose some members. Changing responsibilities for any job will cause some employees to reevaluate whether the position is still something they want to be doing. Attrition has an impact on morale, and will also impact the workload of an on-call team as rotations are adjusted to cover the vacancies left. 

While you can’t prevent all attrition, setting your team up for success will help alleviate doubts. Following up on action items, prioritizing the fixing of repeated issues, and championing your team’s requests to other groups will also demonstrate that you support them.

Ensuring that all team members understand the goals of the on-call effort, the metrics that will be measured, and the positive outcomes that are expected will go a long way. You’re likely to have detractors on your team, and vocal detractors can really have a negative effect on other team members. Firing folks who are destructive or refuse to participate should be a last resort; you can also look for methods like delaying a full on-call roll out, or setting a competition for improving key metrics with another team to motivate folks. Listen to people’s concerns with empathy. Many of the suggestions in this guide will help you build a supportive team.

## Time Management
When application developers are part of an on-call rotation, there will be periods where they won’t be as productive in their normal planned workload. When working with your team on an on-call plan, include guidance around how to reduce planned work during on-call shifts.

This will likely be easier for teams that work in short sprints, or with well-defined and well-groomed task backlogs. Teams that don’t have those types of methods in place can also be flexible about expectations during on-call shifts. For example, the primary on-call might work on bug fixing. They might also dedicate their time explicitly to making sure all issues that caused alerts have fixes created. 

## Burnout
Managing burnout on your team is a key to successfully handling on-call duties as well as normal feature work. Dealing with attrition due to burnout is one thing, but it can also be difficult to deal with a team member who is burning out but not yet willing to acknowledge the problem. 

### Monitoring Team Health
Replacing folks is expensive. Keep tabs on your team and how they’re doing. New on-call duties can also cause strife with family members who weren’t expecting to share their homes with noisy alerts in the middle of the night, so managing a humane on-call schedule and prioritizing permanent fixes for alerting issues is important. Maintaining the team you have in a healthy way is less disruptive and will be less expensive than hiring to replace team members.

Knowing what to keep tabs on with your team can vary, but PagerDuty’s Agile Leadership Team has posted their system [on our blog](https://www.pagerduty.com/blog/best-practices-health-checks/). This is a simple method that you can modify for your team’s needs. 

### Working on Systematic Improvement with Peers
As we mentioned earlier, maintaining a humane on-call culture will go far to help with team health. Actively managing the issues and alerts, as well as setting appropriate priorities for incidents can reduce alert volumes for existing services over time. Maintaining appropriate, actionable alerts should become part of your development practice for all new services as well.

When services managed by your team depend on other services that aren’t providing necessary reliability, your team may need to do more defensive coding to protect their services and their sanity during on-call. Planning for things like dependencies becoming slow or unavailable, and adding functionality to deal with them, might take more time to implement initially, but will help your service metrics over time in addition to saving your team alerts. 



