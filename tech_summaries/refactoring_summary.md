##Refactoring Web Services
*Based on notes from "Web Services: Grow, Refactor, Reguild"*

*presented by: Alysha Voigt (Microsoft), Barbara Raitz (Airbnb), Ity Kaul (Twitter)
 Kelsey Stemmler (Pinterest), Neha Karajgikan (Square)*

*at the 2014 GHC*

##When to refactor?
 * It's time to refactor if:
   - code is fragile
   - productivity declines
   - performance suffers (can't scale)

##How to refactor?
 * Take measurements, metrics from before the refactor.
 * Break down and simplify the problem.

> "For returning contacts:
> We wanted to have intelligent ordering, deduping, ...
>it sounds like they started with the basic version (just the order they came in)."

 - Kelsey Stemmler (Pinterest)

> "You don't take your codebase
> and decide to split and go for it.
> Start with little pieces.
> Gain some confidence and iteratively work and break pieces out of it."

*- Kelsey Stemmler (Pinterest)*

##How to launch a refactor?
 * Slowly test your new service on a subset of live traffic.
 * Measure and test everything.
 * Document and communicate everything you are going to do.

> "Rolling to production ...
> If your feature is something significant
> then ... divert a percentage of the traffic."

*- Barbara Raitz (Airbnb)*

> "I learned; measure everything.
> When you deploy,
> you have visible feedback that everything is working.
> If there is anything that is scary you should be notified.
> ...
> Stop and think:
> how will I test this feature?
> You need to know before you go to production:
>  * what are you testing
>  * how will you test it on staging
>  * how will you test it on production
>  * how will you roll it back"

*- Barbara Raitz (Airbnb)*

> "Any time you have a ... change that we know could have some impact,
> which is typically the case in my team,
> my biggest reccomendation is to have a document.
> Document everything."

*- Neha Karajgikan (Square)*

##Dealing with Missed Deadlines
 * Overcommunicate.

> "As long as you have good communication
> amongst your team;
> weekly emails,
> monitors up in your lobby at work;
> whatever works for you.
> Sticking with it,
> making the communication really clear,
> anything that your team may impact on other teams..."

 - Alysha Voigt (Microsoft)

##Benefits of Refactoring
 * Performance improvements
 * Increased site stability
 * Engineering efficiency improvements

> "It's so much easier to roll up a few more boxes. ...
> In terms of performance,
> in terms of actual engineering efficiency, ...
> It's making changes so much easier."

*- Ity Kaul (Twitter)*

[Full Notes from this Presentation](https://github.com/flarnie/ghc_2014_notes/blob/master/thurs/web_services_grow_refactor_rebuild.md#web-services-grow-refactor-rebuild)
