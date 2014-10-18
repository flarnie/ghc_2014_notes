# Web Services: Grow, Refactor, Rebuild
*panelists*
 * Alysha Voigt (Microsoft) BA CS, a Project Manager
 * Barbara Raitz (Airbnb) Software Engineer
 * Ity Kaul (Twitter) Software Eng. (3 years) (started in Finance Industry)
 * Kelsey Stemmler (Pinterest) Software Engineer (back end infrastructure team)
 * Neha Karajgikan (Square) Software Engineer (6 months at Square)

They mention service oriented architecture several times

> "Web services are everywhere
> assumming that you're growing
> ...
> eventually you're going to reach a point that
> ... it gets very tangled
> ... it takes a lot longer
> it's much more frustrating to build things than it should be."

One challenge of being a service on the web is that your product is;
> "always on, 24/7
> if something isn't working quite right, ... everybody will notice right away ...

> [a challenge is] refactoring.... without disrupting the flow of traffic."

## Recognizing the Problem
**Q:** What was a project you worked on where you realized you needed to refactor?

**Barbara Raitz (Airbnb) Answered:**
>"Almost all code needs to be refactored.
> [This is the] natural lifecycle of code.
> You're going to see this throughout your careers.
>
>[You] start with something clean, small, suited perfectly for the task at hand
>
>...
> [then come] patches, crazyness, .. when does it go too far?
>
>I work at the calendar service at Airbnb.
> It's at the core of the product.
>It's really bad when any engineer touches this code.
> ... extremely fragile ...
> That's extremely unacceptable.
>
> There comes a time when you need to service it."

She outlined some signs that code should be refactored:
> - fragility
> - just can't grow at scale
> - frustration within the team; productivity declines
> - something that should have taken a week takes 3 months

In the example of the calendar feature:
>"With the calendar project, it needed features we just couldn't handle."

*What causes the problem?*
>"Usually the cause is tight coupling of unlike components."

*How to deal with that problem?*
>"Learn how to modularize your code.
>... Understand interfaces. ..."

**Ity Kaul (Twitter) answered:**

>"The world cup was on and Twitter was at the center...
>
> with every penalty kick ...
>
> every red card
>
> [every] yellow card
>
> twitter kept becoming unavailable for small periods of time.
>
> We realized this wasn't scaling.
> We couldn't scale to the growth that Twitter was seeing.
>
> People in the audience don't have to get up to that stage to recognize that problem in front of them."

##Solving the Problem

**Q:** We know there is a problem - how to get started?

**Ity Kaul (Twitter) Answered:**
She started out with the admission that "It seems daunting. What's the easiest way to approach this?"

She described their early "MonoRail (monolithic and in rails)" application, which was "one of the biggest Ruby installations in the world at the time".

>"Everything from presentation layer to logic to cache management was done
> in the monorail.
>
> How did we go about breaking this up
> into different pieces?
>
> When you log into twitter for the first time
> if you look at the homepage;
> timeline,
> trends,
> notifications,
>
>If you think about all of these as different components
>each one was serviced by a different API.
>
>  There are dependencies between components
>  ... you can come up with a timeline."

**Kelsey Stemmler (Pinterest) answered:**

>"My first project was to build an independent ... service in front of these
> back end servers."

Her first step was to "write a design doc, scope out the problem. ...  look at the existing code ... what API calls this would need to support."

She stressed the importance of metrics;

>"We have all these dashboards; we track, we measure ...
> measuring requests per second and latency ...
> requests per second is ... useful - [tells you] how much traffic your service is going to take
>
> If you don't have these metrics available today,
> you can add it.
>
> It's really helpful to estimate how much capacity your service will need, [and]
> how much time you're taking.
> You can compare that between the old service and the new service ...
> hopefully it's not slower than it used to be.
> Then you can go look at it.
> You know where you wanna be.
> You know that you can't get there in one day.
>
> Step 1: Break it down into manageable pieces.
>
> Don't build it from scratch.
> Launch it.
> Hope it goes well.
>
> One thing I learned;
>
> If you have a piece and you can break it down,
>
> Try to break it down further.
>
>For example;
>
> For returning contacts:
> We wanted to have intelligent ordering, deduping, ...
>it sounds like they started with the basic version (just the order they came in)."

**Q:** What if it [the refactor] takes longer - the deadline you set starts to slip?

**Neha Karajgikan (Square) answered:**
>"There are different ways to do your estimations.
> Different teams... have different ways to do this.

She says that they have changed repeatedly the agile practices (stand ups) that they use.

>"Deadline slipping; it happens. Often."

>"One really good way to estimate
> ...
> defining - estimating - ...
> not just [taking into account] writing the code,
> [but also]
> unit testing it,
> doing integration testing,
> letting it be on production,
> fixing bugs, ...
> it's that entire cycle.
> In your estimations that's a good practice,
> but still,
> communicating this with your team."

**Alysha Voigt (Microsoft) answered:**

> "When we were going our refactoring of the web front end ...
> sky drive was rebranding to one drive ...
> we were kind of stopped like a deer in headlights ...
> trying to do too many things at once.
> [The] deadline kept going later and later. ...
> We had to do all the changes in two places. ...
> Once in a while, ...
> It can really get away from you.
> Deal with it the best way that you can.
> As long as you have good communication
> amongst your team;
> weekly emails,
> monitors up in your lobby at work;
> whatever works for you.
> Sticking with it,
> making the communication really clear,
> anything that your team may impact on other teams,
> there will be consequences,
> your responsibility to make sure it doesn't affect others."

**Q:**We're in the middle of coding;
 We need to make sure we're not missing any features.

 Strategies to really validate every piece as you go?

**Ity Kaul (Twitter) answered:**

> "Testing can range on several sides of the spectrum. ...
> junit, ...
> scala test, ...
> whatever it is you're testing a unit of work.
> From there ... integration testing.
> Make sure whether you're writing a new service
> or refactoring a service.
> ...
> Integration testing - deploy your services.
> ...
> Refactoring is a little special;
> Whatever was there should function the same way.
> ...
> We have a terminology
> "dark read";
>
> Take production traffic [and]
> funnel part of it to your new service.
> You have your old monolithic application, [and]
> at the same time the user also gets funneled to your new service.
> Compare your old response to the new response.
> Make sure that it's exactly the same.
> Also load testing that can come from this;
> Your production traffic can be dialed up or down.
>
> [You are] doing two things there.
> Dark reads slowly become "light reads".
>
> By the time you're confident
> ...
> now start channeling user input to the new service
> that can be dialed down or up
> so there is flexibility."

**Kelsey Stemmler (Pinterest) answered:**

> "Right now i'm working on a project
> moving python core code into java.
> We still wanna make sure that everything's [the same];
> No added information.
> What we're doing right now
> is the shadow table;
> basically the original table copied ...
> [an] offline process does the same write on the shadow table.
> Then a process [happens] to make sure that the data is equivalent.
>
> In the case of a larger data set
> we have a sharded database.
> We choose individual shards to do testing on.
>
> How do we actually do this? Control the dark reads and dark writes;
> [We have] controls that we call deciders.
> [They] can be used to turn features on and off.
> ...
> You create a decider with a name
> ... [it] has a value 0-100.
> We have this dashboard ... [with]
> scrollbars.
>
> To me it was really cool;
> At my last job we had no way of doing that.
> most places you have to deploy code,
> and if it doesn't go well you have to roll it back.
> We use that a lot at Pinterest.
> We run experiments
> on different user segments.
> We also have triggers;
> When a certain condition is met, an experiment is done."

**Barbara Raitz (Airbnb) answered:**
> "I love testing, in terms of code quality.
> This is what we do at AirBnb as well.
>
> I have a friend who was starting a company,
> [and wanted to know how to hire good engineers.]
> Find an engineer who knows how to test.
> If they don't know how to test, then in the first week
>   of bootcamp, teach them that.
>
> On controls;
> Kelsey described something I used every day.
> Example:
> I work with calendar code.
> I made a change that was supposed to act exactly the same way,
> but instead of just going live,
> I put an if/else switch.
> Inside that switch;
> a try/catch that protects you.
> In there
> you compare;
> you get the real result
> and then you chart it
> and you see how many are succeeding and how many failed.
> You really test it until you know.
>
> [One bug that surprised me was finding that because]
> there are different currencies in the world,
> ...
> There are other countries in the world, and they have rounding errors.
>
> I'm very proud of my code quality.
> ###I learned; measure everything.
> ###When you deploy,
> ###you have visible feedback that everything is working.
> ###If there is anything that is scary you should be notified."

**Q:** Now it's actually time to put it into production.
 This is kind of risky.
 Nobody should notice.
 What strategies do your teams do?

**Neha Karajgikan (Square) answered:**

> If we mess something up, customer impact is very large.
>
> Rolling to production ...
> If your feature is something significant
> then ... divert a percentage of the traffic.
>
> What if your changes are small?
> You're still going to deploy often.
>
> Any time you have a ... change that we know could have some impact,
> which is typically the case in my team,
> my biggest reccomendation is to have a document.
> Document everything.
>
> We got burned by this a couple of weeks ago actually;
> We thought our change was insignificant,
> not too risky.
>
> So what we did was
> changed the way we read from the database.
> Unfortunately we realized we introduced a bunch of bugs that were showing up
> across a bunch of services that depended on our services.
> We kept fixing the bugs that kept cropping up.
>
> When it becomes about money, everybody freaks out.
> ... But at that point in time it was really hard -
> We had this ugly commit history
> It was so hard to just revert the change back.
> [If we had] properly assessed the risk and impact of our change,
> talked to all the teams that were impacted,
> sent multiple emails out,
> reach[ed] out to team managers...
> "If your team is going to be affected, let us know immediately."
>
> A good example that happened:
> The app I work on
> was on Rails 2
> until about 6 months ago.
> It was a big shock.
> we made this ... move to mobile.
> The roll out of that was amazing.
> We got the team excited about it.
> The day we actually did do the deploy,
> the entire team gathered.
> As we were going to deploy,
> we watched our metrics;
> Watched new tracking,
> Just looked at exception tracking,
> made sure that everything is working as normal.
>
> [We] kept a really close eye on what was happening,
> notified the different teams,
> made ourselves available for any questions, ...
> It went seamlessly.
> We celebrated after that.
>
> That's because we had a really great roadmap."

**Barbara Raitz (Airbnb) answered:**

> ###"Stop and think:
> ###how will I test this feature?
> ###You need to know before you go to production:
> ### * what are you testing
> ### * how will you test it on staging
> ### * how will you test it on production
> ### * how will you roll it back
>
> The big example:
> Airbnb about 6 months ago went through a big rebrand.
> That was kind of a gutsy move for us.
> On the engineering team,
> it was all legacy code. ...
> A complete sweep with new brand ...
> and all of this was done under the covers with out the presses seeing.
> At the highest load we roll over the boxes...
> Kind of gutsy.
> [It was the] most beautiful rollout I've ever seen.
> Everybody had a name of what their task was,
> verify that, and say 'done', ...
> We had a mock roll-out the day before.
> I need to go find some of the engineers and ask them to write a blog post.
> All of you could benefit from that.
> Estimate capacity;
> What are all the places it can go wrong,
> [and] what do you do if it goes wrong."

**Q:**Benefits your company has seen as a direct result of doing this?

**Ity Kaul (Twitter) answered:**

> "Our monorail .. is being blogged about, talked about...
>
> Before coming there I wanted to check where we were at;
> currently 134k tweets per second.
> ###It's so much easier to roll up a few more boxes. ...
> ###In terms of performance,
> ###in terms of actual engineering efficiency,
> they can write their code in isolation and then integrate at the end.
> ###It's making changes so much easier."

**Barbara Raitz (Airbnb) answered:**

> "Testing is only getting better ...
> codebase is evolving ...
> everything we talked about is becoming part of the standard practice ...
> the site has gotten more stable than it has been
> ... the calendar service ...
> i'm starting to see some shiny spots ...
> hoping to roll out some new features ...
> that will be my reward."

**Kelsey Stemmler (Pinterest) answered:**
 She shared a personal success story from her work at Pinterest:

> "One of the projects I was working on this summer; ...
> Rebuilding user typeahead.
> We wanted it to be really fast.
> You can have millions of followers.
> Very big scaling task. ...
> Built a new back end to help store that more efficiently. ...
> 99% [of] requests were [within] 28 ms ...
> the slower requests were at 28ms ...
> the data itself was more reliable ...
> [before] if you had a lot of followers sometimes they wouldn't show up ...
>   but now it's a lot better ...
> the previous project I worked on ... gave me more confidence ...
> Working on a bigger piece of the code ...
> You don't take your codebase
> and decide to split and go for it.
> Start with little pieces.
> Gain some confidence and iteratively work and break pieces out of it."

**Neha Karajgikan (Square) answered:**
She described their move from Rails 2 to Rails 4.1:

> We're one of the only services that is on the most modern version of Rails.
> Our success stories ...
> When it comes to refactoring;
> If you have code, ...
> you're always going to have to come back and revisit it.
> There will be mistakes,
> because of demands, time, ...
> You will always have to come back; it's part of the process."

## Questions from the Audience

**Q:** For Kelsey Stemmler (Pinterest) - you talked about how you have that bar, dynamically push things into production.

**Kelsey Stemmler (Pinterest) answered:**
They use zookeeper to host the config files.
Then they run daemons that constantly check the configs;
Like a config watcher to update the configs.

**Q:** How often when you try to rewrite your services do you look for new technologies
to use?

Related to that;
we had to find techniques to figure out ramp-up
we kind of write half of it in the old technology, half of it in the new

**Ity Kaul (Twitter) answered:**

> "We were on Ruby on Rails and went to the new stack. ...
> Rewriting in Java and Scala, ...
> You get the statically typed language;
> You can sleep better at night.
> You have your compile time check.
> Half of that code was still running on the codebase until it was moved to the new codebase."

**Q:** Did you have any ecosystem for balancing traffic between the old stack and the new stack?

**Ity Kaul (Twitter) answered:**

> "You can take production traffic and funnel it to the old and new services.
> Once you roll to production and make it return responses to the users.
> You can dial the traffic up and down; [For example,]
> I only want .9% of the production to go to the new services.""

**Q:** How do you guys prioritize doing this
because it's such a huge effort?
It's a full time job;
How do you guys do that?

> "It depends on what the priorities are for your company at the time.
> We *had* to rewrite;
> There was almost a code freeze.
> You had to move them out to the new services;
> All hands on deck and make that happen before we add new."

---

All images and quotes fall under [fair use][fair-use] and are intended for purely educational purposes.

This document is licensed under a [Creative Commons Attribution 3.0 United States (CC By 3.0 US) License][cc-by-3].
[fair-use]: http://en.wikipedia.org/wiki/Fair_use
[cc-by-3]: https://creativecommons.org/licenses/by/3.0/us/

---
[Official Notes on the Systers Wiki][web-services-wiki]

[web-services-wiki]: http://systers.org/wiki/communities/doku.php?id=wiki:ghc:ghc14:web_services_-_grow_refactor_rebuild_panel
