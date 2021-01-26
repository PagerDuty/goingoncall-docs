![Team Norms](../assets/img/headers/OnCall-People.png)

## Responsibilities
While being available during an on-call schedule is one of the first responsibilities of being on-call, there are more obligations beyond just acknowledging the alert. When an alert comes in, it will notify the on-call responder who will then acknowledge the incident (to stop any further escalation). One of the goals with having SMEs on call is to reduce [mean time to acknowledge](https://support.pagerduty.com/docs/glossary)  (MTTA) and [mean time to resolution](https://support.pagerduty.com/docs/glossary) (MTTR). Driving down MTTA through quick acknowledgement of alerts is one of the behaviors on-call schedules reinforce.  

Once an incident is acknowledged, the on-call engineer has the responsibility of triaging the incident; is this something they can fix on their own? Do additional responders need to be notified? Do they need to reassign to another team? Is the severity increasing and does a major incident need to be kicked off? 

At PagerDuty we have a saying: “Never hesitate to escalate!”. Part of the triaging process is determining if you have the ability to fix the problem yourself. If the issue is not time sensitive, create a ticket, assign it to the right team, and work on it during business hours. However, for high [severity](https://response.pagerduty.com/before/severity_levels/) or incidents that are rapidly increasing, hesitating to escalate only increases the overall opportunity for related damage. Engineers should always feel empowered to involve other teams and team members as necessary. You will rarely know all of the contributing factors or *gasp* root cause at the beginning of an incident. As a first responder, the goal is to have a basic enough understanding to be able to determine what the causes might be, and who to bring into the response.

Additionally, on-call engineers should look for ways to improve existing systems and processes. Take the time to tune alerting if there are alerts that aren’t actionable. Also, look for ways to improve on the system and ask questions like: 

- Was there enough context in the alert to make it meaningful? 
- Was the documentation up to date? 
- What can I do so that the next person who may deal with this will have an easier time? 

## Not Responsibilities
Every problem that arises across your platforms may not be your responsibility, even during an on-call shift. A single team within a larger organization should be able to escalate to other teams or to ask for additional support when the incident requires it. 

!!! tip
		“Never Hesitate to Escalate”

It’s important to help responders manage their time well during their on-call shift in order to avoid burnout and maintain employee morale. A few other things to consider include:

- Encourage responders to lighten their regular workload during an on-call shift
- Remind responders that if they are not adding value to an incident, they should disengage from the incident or set their status to stakeholder for later announcements
- When a responder is already engaged with an incident, additional and/or unrelated incidents should fall to other members of the team
- If a responder has burned out during a shift, have a process for someone else on the team to help them pick up the part of, or the entire shift so they can sleep, eat, etc.

It’s easy for some responders—especially if they are new to being on call—to feel obligated to solve all problems at any cost to themselves. This behavior won’t help your team in the long run.Folks can easily experience burn out and resentment. Additionally, it is important to remember that people are human, while there is the expectation an on-call responder be available to answer pages, life happens. Cell phones fall in pools, the internet goes out, dinners happen. Sometimes an alert gets missed, which is why there are escalation policies, because there is no expectation that a responder will be the first to answer every single page, every single time. 


## Handoffs
At the end of an on-call shift, it’s a good practice to have some kind of formal handoff. This can take the form of a team meeting, where the outgoing on-call responder summarizes the incidents for their shift. It can also take the form of an email, shared document, or saved query in your incident response platform that highlights the current and recent alerts and how they were handled, if they are closed, or the current status for those ongoing into the next shift.

The purpose of the handoff is to make sure the incoming on-call responder has all of the information and context for the current state of the environment. 

Other items that might be helpful in your handoffs:

- Recent deployments on key systems, including upstream dependencies and downstream consumers.
- Any queued remediation work requests created after a postmortem meeting.
- Any TODO action items to make documentation, context, alerting, or anything for the next person on call better.
- Staff changes on other key teams. For example, if your team regularly reaches out to Ed in database engineering, but Ed is leaving your organization.

Your team will likely find other key areas that are useful to share in shift handoffs. At PagerDuty we recommend the second layer of your escalation policy be the person from the prior week as they should still have context from any previous incidents.  You can learn more about PagerDuty recommendations on escalation policies [here] (https://support.pagerduty.com/docs/escalation-policies-and-schedules).

## On-Call and Life
For teams and individuals new to going on call, the mentality shift can be hard. One of the critical considerations is work-life balance when going on call. As previously mentioned, remembering that people are human is key to avoiding burnout and maintaining a people-centric culture. Things to consider with on-call life are:

- Vacations and emergencies. When life happens, use the override function on schedules when you have something planned or unplanned occur (to learn more about how to user PagerDuty overrides [see this page](https://support.pagerduty.com/docs/editing-schedules)).
- Keep on-call schedules consistent. Think through how long the on-call rotation is; 3 days, 5 days, 7 days or 8, 12, or 24 hours? At PagerDuty, we recommend handing shifts off on Mondays to recap the week with minimal confusion and ensure shifts aren’t switched over the weekend. 
- Teams should work to find what is best for them and their applications. For best practices on shift lengths on effective shift scheduling, check out this [article](https://community.pagerduty.com/forum/t/scheduling-effective-start-end-practices-for-on-call-scheduling/1677). 


