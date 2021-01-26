![Introduction](../assets/img/headers/OnCall-Intro.png)

With the right approach, being on call doesn’t have to be a painful experience for your team. When you have a culture of collaboration, infrastructure insight, and the right tools in place, deploying an on-call workflow will create some predictability around your production systems. A good on-call program will create some containment for disruptions, provide predictable paths for escalation and resolution of incidents, and encourage application teams to take on work to fix chronic issues in your ecosystem. 

We often think about on-call the way it is dramatized in television shows—doctors with beepers getting paged into Operating Theater 3 for emergency surgery, STAT. For technical teams, the reality is less life-threatening, but can still be a stressful experience, full of uncertainty. 

When something unexpected happens to a system, the people who know that system best are needed to investigate and fix whatever the problem is. Sometimes an individual can accomplish this by themselves. In other situations, more help is needed—maybe from the same team, maybe from another team. There could be some additional organizing or coordination, letting responders know to join a conference call. 

During work hours, these interruptions might pull folks away from work tasks or meetings. Outside of work hours, though, they could be eating dinner, or commuting, or sleeping. This disruption of personal time is a big concern for folks going on call for the first time. In this guide, we’ll go through some of the steps your team can take to alleviate these concerns and set your team up for success.

## Why Have On-Call?
If your team is responsible for consumer-facing services, you probably know how unpredictable users can be. Did we really expect someone to be doing their banking or ordering groceries at 3 a.m. on a Wednesday, or using your service in a way it wasn’t intended? Your goal as a manager isn’t to punish teams for writing bad code; it’s to improve the overall reliability of your teams services and systems. Unfortunately, for many complex distributed systems, the best way to do that is in a production environment, exposed to whatever interesting things users might get up to. 

Customers now assume most services will be up and running all the time—not just during limited business hours. In addition to customer expectations, the increasing complexity of modern services makes it more and more difficult for general-purpose operations centers to effectively respond to all the idiosyncratic alerts that might be generated. So teams that would have traditionally been spared an on-call responsibility are increasingly expected to have some responsibility for their services during their off hours.

Having a predictable on-call schedule can be beneficial for your team. For individuals, being on call creates a scheduled time when they know you will be the first person contacted if something happens. For teams with unstructured incident response, implementing a regular on-call rotation can decrease the amount of unplanned interruptions some team members receive. Instead of always being the person to be contacted for an issue, team members will have primary responsibility on a regular schedule. When someone is on-call, they can take fewer regular tasks during a sprint plan, knowing they will need some hours to deal with unplanned work. 

It’s possible that not every service your team works on needs to have a full-coverage, on-call schedule. You may have different uptime and reliability goals for different types of services. It’s common to need 24x7 response for customer-facing services, or those with strict SLO’s, but for internal applications, it might not be needed, especially for services that run periodically. If your team has some offline data processing that runs in the middle of the night, you might have some flexibility to say that the on-call doesn’t need to be alerted during off hours, but should be alerted at 9am.  


!!! tip
		For more on SLA, SLO, and SLI, check out [this blog post](https://www.pagerduty.com/blog/best-practices-service-monitoring/).

!!! tip
		For an example, PagerDuty’s SLA is published [here](https://www.pagerduty.com/standard-service-level-agreement/).

When you think about the services your team owns, be pragmatic, but also be ferocious about taking on responsibility for the things you are responsible for and the things that matter—you don’t have to be on-call for absolutely everything. 

## Who Goes On Call?
Prior to the emergence of cultural-technical philosophical shifts, like DevOps and SRE, on-call responsibilities were generally limited to teams considered “Operations” or “Systems Engineering.” This practice didn’t prevent developers from being contacted during their off hours, but it made that contact unpredictable, and the response times for those alerts longer than it needed to be, leading to  unnecessarily extending service outages.

With more teams exploring DevOps and SRE models, a wider range of individual contributors who would not have been on-call just a few years ago are finding themselves with on-call responsibilities. The most impactful change is that more application development teams are playing a larger role in taking care of the code they write when it reaches production. When organizations need to reduce the amount of time it takes to respond to and remedy a problem, having the folks who know the code best in the responder list is a huge benefit.

One thing to keep in mind is that responders will have on-call responsibility for the areas of their expertise. We talk a lot about the concept of [full-service ownership (FSO)](https://ownership.pagerduty.com/), and the role application developers play in incident response for modern organizations. We have an entire ops guide dedicated to this [method](https://response.pagerduty.com). Translating full-service ownership for your organization can look very different from another organization, and success with the FSO model may depend on how robust or sophisticated your service modeling and monitoring systems are. Adopting full-service ownership and an appropriate on-call rotation should focus your teams on the aspects of the production systems that they know, and applying the appropriate expertise to the response process. Different teams can be on call for different components of an application stack based on where their knowledge and strengths lie.

Having an on-call rotation should ideally mean better on-call experiences for your team. Team members will know exactly when they need to be available to respond to incidents on a regular schedule. Explicit rotations and schedules take some of the unexpectedness out of unplanned work for responder teams. The best part is, team members know when they are not on call, when they can take a vacation, or when they can just put their phones in a drawer and run away. For managers, there is greater visibility into the health of the team; who is getting paged a lot, who is being woken up at 3am consistently?

An on-call shift doesn’t necessarily need to be 24x7. Teams using platforms like PagerDuty can customize their rotations to best suit their requirements. Teams can limit the hours they support certain services. Internal applications might only require a 24x5 or even a 9-5x5 schedule for user support.

Global teams have a particular advantage in that their schedules can use a “follow the sun” method. When teams are widely distributed, teams with 8-, 10-, or 12-hour time differences can be responsible for response during their daytime hours, with no one required to have an overnight shift.  

!!! tip 
		For tips on follow-the-sun on-call schedules, check out PagerDuty’s recommendations [here](https://support.pagerduty.com/docs/schedule-examples#example-6-follow-the-sun-schedule)

Organizations new to FSO, DevOps, and [SRE](https://www.pagerduty.com/blog/building-scaling-sre-team/) models might also take advantage of a hybrid model with a Network Operations Center (NOC). An established NOC can serve as first-level responders in any of these models. NOC responders can also take advantage of automated processes and [runbooks](https://www.pagerduty.com/resources/learn/what-is-a-runbook/)  to alleviate the number of alerts that escalate to other teams.

Overall, teams have a lot of flexibility for how on-call can be incorporated into their workflows. Choosing appropriate scheduling, assigning the services and alert types, and establishing best practices for escalations will all benefit the teams and individuals being asked to take on-call responsibilities. The rest of this guide will feature some recommendations around the mechanics of on-call as well as some guidance for building a supportive on-call culture for your team.
