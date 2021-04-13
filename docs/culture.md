![On Call Culture](/assets/images/headers/OnCall-Culture.png)

Successfully implementing on-call for a new team requires team members and managers to think about team dynamics, trust, and communication. We see these same characteristics in teams that successfully run [postmortems](https://postmortems.pagerduty.com).

Telling your team that they will have on-call responsibilities when they haven’t had them before can be difficult. On-call has an established reputation for being exhausting, wasteful, and even abusive in many organizations. Your team may have heard horror stories for their colleagues of missed events, wasted weekends, or ruined family holidays. For a while there was even a [podcast](https://podcasts.apple.com/us/podcast/on-call-nightmares-podcast/id1447430839) focusing on on-call “nightmares” in tech.

Building a supportive culture and maintaining that culture long-term is a key responsibility for managers of on-call teams. It is worth noting that the goal of going on-call is to lower stress, bring the right people in at the beginning, spread the work across the team, and allow folks to know when they are OFF call.

## Empathy and Psychological Safety
A key element of team dynamics in successful on-call teams is empathy. Teams and individuals need to feel empowered to make decisions quickly to remediate incidents without fear of reprisal. During an incident there is a mentality shift from “peacetime or OK” to “wartime or not OK,” this mentality shift changes the normal operating behaviors. From hierarchies to decision making, teams that have a high level of psychological safety will spend less time debating courses of action (which leads to decision paralysis) and more time working towards resolution. Additionally, empathy needs to extend beyond the incident to the day-to-day ways in which teammates interact. It is important to remember that a teammate may have been woken up at 4 a.m., and could use a little extra time to sleep in. Maybe a teammate has been having a rough week on call with a lot of incidents, would it make sense for someone on the team to take the rest of their shift?

Psychological safety and creating a blameless culture is a key indicator of high-performing teams according to a study done by [Google](https://rework.withgoogle.com/blog/five-keys-to-a-successful-google-team/) . One of the most important actions that a business can have is to support learning. Supporting learning is action-based, and it is important that it’s modeled from leadership down the hierarchy so that all employees are psychologically safe to try new things. This is important to clarify as "do as I say, not as I do" can quickly become a stressful— even toxic—culture for people to grow in. In regard to on-call teams, teammates need to feel safe making decisions to resolve incidents, and that they can depend on each other to “answer the page.”

![Psychological Safety](/assets/images/psychological-safety.png)

## Onboarding
Successful on-call teams spend the necessary time onboarding new team members. Give folks the time to learn the new systems, understand the dynamics of the team, and know who to call before throwing them in an on-call rotation. Shadow on-call rotations are an easy way to get new team members spun up on services they will be on call for. These rotations allow for people to listen into incident calls without having the responsibility of being the subject matter expert. Shadow responders receive the alerts and join the calls in a listen only mode. Once the new member has shadowed a few calls, they will be more confident in acting as a responder. The shadowee should then schedule time with the responder they shadowed after the incident call to answer any questions.

Creating a shadow schedule is a fairly simple process for more information check out this [How To](https://community.pagerduty.com/forum/t/creating-a-shadow-schedule-to-onboard-new-employees/1647).

Beyond shadowing, make sure new users have contact methods (SMS, email, push, and call notifications) set up and staggered so they don’t miss alerts. For more information on how to set these up in PagerDuty, check out this [knowledge base information](https://support.pagerduty.com/docs/quick-start-guide).

## Iteration and Improvement
For many teams that have incident response duties, some kind of metric like MTTA (mean time to acknowledge) or MTTR (mean time to resolve) is tracked to determine how fast the team is handling incidents.

MTTA and MTTR are blunt instruments when taken at face value, and may not reflect exactly what is most important in your response plan. Neither metric differentiates among incidents of differing priority or importance. Your team may want to break down metrics based on priority, severity, or other categories. For a more detailed discussion of working with these metrics, see [this How To](https://community.pagerduty.com/forum/t/reporting-making-your-metrics-meaningful/1549) and [this Knowledge Base article](https://support.pagerduty.com/docs/reporting).

!!! tip
		MTTA and MTTR are also discussed in the [Full Service Ownership Ops Guide]( https://ownership.pagerduty.com/digital_transformation/)

!!! tip
		*Critical Incident Response Time*, or CIRT, is another emerging metric that might be interesting for your team. Learn more about it in [this article](https://opensource.com/article/19/7/measure-operational-performance).

Other potential metrics relate to how fast fixes for incidents make their way into production. The longer a permanent fix takes to be deployed, the more likely it is that additional incidents will happen. When we think about getting new features into production, we might measure *mean time to market*. This is also a useful metric to keep an eye on when prioritizing fixes. When a bug or other error causes an incident, fixing it permanently increases the reliability of the system overall and decreases or eliminates the incidents arising from the original issue.

## Escalating Beyond Your Team
Knowing who you're going to call is crucial to streamlining increasingly complicated communications. To ensure that you're reaching out to the correct group(s), you'll need to check that you have defined which areas need assistance. For example, did something start out looking like a network outage but turned out to be a database outage? In that case, you'd pull the on-call database administrators into the incident and allow the on-call NOC to drop off as needed.

Cross team communication is also why it's very important to have as many common tools as possible. In the above example, the NOC will likely have their own network monitoring tools, but if they don't have a tool in common with the database admins, then the NOC won't be able to point to issues in a way the database admins can see. Relevantly, all teams should be in the incident management platform for hand-offs and reviewing what has been done thus far.

When you are pulling in new teams, it's possible that people might be pinged who are not needed. To keep everyone focused on the active incident, make sure to only keep those on the call that have an active role. Before someone drops off, they should clear with the incident commander to ensure 1) that there's nothing left for them to do and 2) to keep communications and decisions centralized.

For those who remain on the call, it is especially important to avoid the use of industry jargon, acronyms, or other short-hand references that could be confusing in the heat of the moment. Remember: not all disciplines use the same "shorthand," and it's better to be clear and up front. This will also help when doing the incident review and postmortem as there will be different skills present for those meetings and write ups as well.

