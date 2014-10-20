#Consistency in a Fragmented World
*Developing for Web, iOS, and Android*

*Friday, Oct. 10, 2014*

**[Full Audio Recording of Consistency in a Fragmented World!][consist-frag-audio]**

![Opening Slide for Consistency in a Fragmented World Panel][consist-frag-slide-1]

[consist-frag-slide-1]: ./consistency_frag_image.jpg
[consist-frag-audio]: https://soundcloud.com/paradasia/14-10-10-consistency-in-a-fragmented-world

**WORK IN PROGRESS: I still haven't formatted and edited the notes in this file.**

Building across desktop, mobile, and all the delight and difficulty that entails

 * Nishita Agarwal (@nishagarwal06) Facebook
   London office
   content creation
 * Tracy Chou (@triketora) Pinterest
   An eng. and tech. lead
   ads team
   building a sustainable business around Pinterest
 * Madelin Woods (@madw) Square
   tools for small business
   software eng.
   work on the front end
   receipts team
 * Brina Lee (@leebrina) Instagram
   Android eng.
   currently on growth team
   helping new new ways to follow
 * Sophia Westwood (@sophiawestwood) Quip
   collaborative app
   like google docs

Q: What platform did eac. co. start w and why

 - Nishita
 what were the plat. the ppl were using at that time
 wasn't until 2010 we started thinking about mobile
 a lot more users were accessing the internet on mobile devices

 mobile web around 2011
 we weren't completely utilizing the platform
 needed separate teams
 around 2012 rewrite of both android and iOS apps
 ours was a compl. product
 that wasn't scalable
 ea. product team has iOS android and web resources
 scale ourselves
 hire specialized ppl to build apps across all platroms

 - Pinterest
 web first
 mobile was not as prevalent at the time
 first app we built was for iphone
 tacking on an API
 added as an afterthought
 went until 2012 utnil co. wide effort
 launched ipad app
 android apps
 redid our iphone app

 .. later we started working on a desktop rewrite to consume the API as well
 mobile web rewrite until
 protip we are seated in order our co. were founded
 first was iphone
 often times first mobile platform
 a lot of users in the US
 as time went on we found it was very imp to build out for all other platforms as well

 - Square
 launched initially with iPhone app
 we needed to take online payments
 shortly after dev. an android app
 interst thing w square
 our iphone and android products are compl. diff. than web prod.
 use the web mostly for managing your accts and info.
 still con. to use it today
 but we have a ton of webapps today
 giving merc. ... tools
 doing the kind of bus. management they aren't doint while running their business

 now we have 3 apps
 sq order
 sq cash
 sq register

 we try to release on iphone and android simultan.
 try to keep web features consistent
 that feature is constent across web products as well

 - Instragram
 is 4 years old as of this week
 we launched web and iOS together
 mostly for viewing gal. and people togther
 did it purposefully to stress that it would be mobile only
 authenticity of taking a photo and sending it to your friends

 moved to -- in 2012
 building it on a windows phone in march of 2014 of this year
 microsoft was saying a lot of users were asking for our app
 we only have 3 plats we run on
 plus web

 - Quip
 from the start we knew we were going to be cross platform
 a lot of eng. dec. were going to be cross platform
 web and iOS with a beta version of iOS
 as android is known for
 it got a little delayed
 one thing that is interesting about Quip
 we branded around being cross platofrm

 we didn't really mean any device
 we meant web, iOS, and android
 it's very expt. to start dev. across platforms
 bare bones version of mobile web
 for web we didn't mean all of web
   no need to support IE8
   or even really IE9 or 10
   mostly we supported chrome
   as well as Safari and FF to some extent
   clearly we all dev. cross platform to some extend
   why should we be cross platform at all

 - Nishita
 a bunch of benefits
 consistent UX across all plats
 ... we want every one.. to be able to access the same type of products
 we want them to have the same controls
 indepe. of what plat. you are on
 ...
 consistent vision for the product
 it's about having common design
 common vision

 it also depends a lot on features
 when we're launching privacy controls
 it would be weird if we only allowed ...
 you're on privacy disparity when not on web
 it's important to always provide those features on all plat
 as soon as we leave one platforms it's really easy for hackers
 to take adv. of that vuln. for span

 it allows for better .. of your code

 it's .. more predictable to know what your code will do

 - quip
 is all about being able to collab. with your team
 online or offline
 as well as edit from the web
 given that we had to do it
 we saw it as a market oppurtunity

 were there any benefits to doing that?
 there's a lot of downsides
 you're slpitting up your eng. team 3 ways
 3 copies of the same code
 you have to test on 3 devices

 there are a couple of silver linings
 one of them is you can actually draw on the best of each platform in dev.
 it's much easier to do things like ab testing on web
 on iOS .. design tends to be very clean
 android  we haven't really figured out
 there is one
 bc it is so difficult
 there is some benefit to having done that already
 we can go see what iOS is doing
 translate the logic over

 - Square

 it's really important to question why you're doing it
 what is your product. .. who are your users
 we don't necc. have cross plat. consistency betwe mobile and web
 this isn't twitter or fb...
 its like, your mom or your dad or your grandma
 they aren't necc. as fam. w tech.
 we want to make it easy for them
 if they're running a bus. w mult. employees
   they may have mult. devices in their store

 that's a key aspect .. for us
 just making it really easy for them to use our products
 on the web side of things
 I think you just ... you don't want to have to think about it
 ..
 you want it to be fairly consistent with desktop web, iOS, android

Q: Biggest challenges we've all faced with cross platform consistency
 - Pinterest
 the biggest thing is ... you have a lot of surface area of your product
 there are a lot of challenges
 for diff. design paradigms
   iOS has very strong
   android has it's own
   web is all over the place

   ...
the eng. side - you just have to .. build a lot more
it's harder for an ind. eng. to build everything
mobile vs. desk. vs. tablet
diff. paradigms of interaction
a lot more to think about
you might be able to start off w/ 1-2 eng.
rapidly have to start specializing
at Pinterest
we have a web team
an iOS team
and android team
exp. w/ moving some devs on feature teams
puts a pretty big burden on your eng. team
...
a lot of coordination effort
figure out prioritization
do we insist that everything ... launch at the same time
  what are the drawbacks or benefits to doing things on diff. platforms
  for some things you don't really have a choice
it would be silly to say you could only msg somebody on iOS
a lot more eng. and design cost to all of this

for instagram we're a bit more lucky
  we only care... (about iOS and android)
  coordination between teams
  we have to make sure launch dates are the same

  iOS takes a little bit of time
  communicate that to our PR team
  our marketing team
  if android is still lagging behind
    (in most cases if not all cases)
 we can use their (FB) testing framework
 you also have to make tradeoffs
 which iOS or android are you developing for
 which featureset are you willing to build for
 on top of that
 if you start to cut our features on android vs. iOS
   our users will complain
 we end up having a lot of tech. debt
 when android is already behind
 sometimes when we go about dogfooding
 sometimes iOS finds the bug first
 it's all about communication
 when it comes to cross plat consistency

Q: What are the strat. for miitig. these chall.

 - Pinterest
 Trying to coordinate between desktop and mobile
 we wanted to make sure the webapp was treated as a client of the API just like .. iOS and Android
 built a framework in house
 different than a lot of trad. web dev.
 pushing a lot of that logic behind an API layer allows you to keep a lot of consist.
 we have ways of optionally including things that can be shared
 in some cases the mobile views will be a lot lighter
 we can still share a lot of it w/desktop
 we have SASS mixins we can include for diff. styles
 JS is a little more straightforward
 for mobile web
   there are some cases where we will build things for mobile web
   and have native web wrappers around those features
   it enables us to get something out there
   get it out into the apps without all the native costs

 - With Quip
 being in a pos. to know from teh start
 i'm sure in 3 years we'll have to deal with other challenges
 we knew that building for web, iOS and android,
 3x as much problems
 everything gets magnified
 build tools to make everything easier
 if you're doing something 3 times manually
 we wrote some shared syncer code in C++
 in order to have the same code to keep the local SQLite db in sync
 with AWS
 so that when you got access again it would sync to the web

 another thing we did
 quip has an editor
 we put in a ton of initial eng. time
 to make it so you could share that editor between iOS
 web and android
 web is has to be JS
 on android unfort. you have many diff. versions
 so it's kind of awful
 we made it so we can ship
 chrome
 inside of quip
 when you download it from the app store (on android)
 ... you can develop for that version for the web view
 the downside is a ton of hacks
 i was a little bit sad - it's a lot of time, a lot of effort
 it was kind of neccessary
 you're either gonna have problems later on, or problems early on
 you can decide when you wanna deal with those problems

 I think ideally
 ... we could tell you we're all doing the same thing
 and we could tell you what's the secret sauce
 but it's not the reality
 it's about knowing what trade-offs you're making

 can you afford ... etc.
 it's really a series of tradeoffs and underst. those tradoffs at the end

 - Square
 any time you approach a challenge you build a toolset around it
 we only had one web repos.
 as we'v egrown we have mult. web services
 for all the tooling we've built
   we had various style guides
   CSS frameowrks
   JS tools
   how do we share these?
  We began collecting these
  makings ure our code was really abstractable
  style gems we can include
  just import that style gem
  for a quick way to get started
    we have a handful of JS libraries we share around the company
    making sure that everything is really well tested
    we use rspec
    unit testing
    on each of our web services
    we use protobuffers
    helps us share APIs across all the different services
    on web there's a handful of challenges we have to face
    it gets expo. more compl. once you have to deal with iOS Android

Once you say 'code freeze' you actually have to freeze it
we have this concept called a release train
we have a conductor for the release train
that's a PM
mapping out what version of the app will we be releasing
up to all teams to coordinate with the conductor

if you aren't able to hit that ship date
  it's going to get pulled
you have to be able to commun.
as your company grows
communication is the biggest thing
all of our companies started out super small
communicate commun. commun.
that's the only way you can get over any of these challenges

 - Do you guys exp. w/ or launch on all platforms or just start with one, test one out, and see what happens?

 - At Facebook
 it really depends what the feat. is
 ideally we want all of it to go out at the same time
 a lot of times it's not possible

 the other things is the release cycle
 at FB we push code twice every single day
 for desktop and mobile web
   it's possible that our mobile users get it way delayed

 it's faster and easier to dev. on web
 we use it to experiment
 it's faster to get it out
 it's easier to iterate on it
 instead of waiting 2 weeks every time you make a single change

 if it's a mobile web
   we experiment on mobile web
it's a comb. of what the feature is
with videos
we started with testing on web

we gauge the user's interest
at the same time, if it's someth like priv contr or msgs
you want to ens. it's avil. on all plats at the same time

 - Instagram
 still again lucky in this case
 we put so much effort on putting things on both platforms
 a lot of times we launch on both platforms
 for dogfooding we usually start on iOS
 android's always lagging behind
 we need that extra dev. time

 it's a great challenge to dev. on android
 android has diff. APIs
 all the diff. manuf. have diff. ways of encoding and decoding video

 we really care about reliability and perf.
 we were not willing to sacrifice that to launch on android

 - Quip
 at quip we try to launch on everything
 bc it's intended to be consistent on everything

 ...
 ideally we would say we need to have a lot of disc.
 shipping feat. cross plat. all the time

 if you say 'android can come later'
 sometimes later never comes

 one mentally that has helped
 is to think about the most important actions first
 if it has to be cut bc of release time
   try to get that in later
   that's ok

 Quip has not had to deal with any eng. overhauls
 we certainly will

 - What are some eng. overhauls you had to do
 to deal with the landscape is constantly changing?

 At FB
 we've been around for 10 years
 we moved into this mobile first mindset
 a lot of the overhauls we've done

 A lot of the rewrites we've done have been pretty gradual

 for a really long time we had ... separate endpoints for mobile and web

a lot of the data ... is the same on both mobile web and desktop web
centralized controller

it was a lot more gradual
deprecate a lot of the new endpoints
no new ...
no more legacy controllers in the system

have the product teams keep in mind
so they are always using up to date tech.

any time you want to take a break from your usual load
go and rewrite

decided to have a unified query lang.
it's called rofql
as long as your query is in that lang.
the server doesn't hav eto care if it's android or iOS

 - Pinterest
 has had one really big rewrite
 and that was for the website
 if we go back ...
   pinterest started with web
   ... over time we've had a lot more mobile traffic
   we're not 75% mobile

   there were inconsistencies between what you might see on web and mobile

you do a search on web
and it would be diff. than your search on mobile
it was bad in terms of fracturing of dev. attention

mobile dev.s would be blocked on API dev.
web dev.s would reach into the data layer and grab whatever they needed

we did this one really big overhaul so that the webapp would be treated as a client of the API
it forced us to do much more perf. testing on the API
before when we did perf. it was easier to do web
we would make web really fast

with web and how we set up our API
we ... were able to improve perf. across all the diff. plat.s

it ended up taking us 7 months to get the full roll-out
we felt like it was worth it

 we did a big design overhaul at the same time
 ... on web more consistent with our mobile clients

 - Have you had to do design overhauls?
 absolutely
 Square started out just taking payment
 we have grown to a point where we are a ful POS service
 we've added all kinds of features

 ...
 don't add features that ppl don't know how to use
 we tend to be a very design focused company
 if we get a point where it looks outdated
   we take into account
  how the design looks

 - Instagram
 started out as iOS
 we needed to move as fast as possible
 bit redesign was on android
 it was only to do with perf.
 pulling out gradient assets
 do the simplest thing first
   pulled down our assets from 28 to 8
   programmaly color all our assets

 Audience questions:
"How to have strong branding and also embrace the design conventions of that platform
I know that's something our team has struggled with"

 - At Square
  we have specialized designers for each of the platforms
  solely focused on android, ... iOS, .. web
  it's almost an organizational thing
  you have to push your organization to collaborate
  always be showing your work
  that's something that
  you really have to put in the effort to do that
  you think talking with your coworkers is easy to do
  it's not

  ppl think it falls to  .. a creative director
  it comes down even front end eng.
  we talk back and forth
  ...
  we really force our designers to .. talk to each other

 - Instagram

 we used to have designers for android and iOS separately
 we saw that as a problem
 we put android on all our desks and make that our main phone

 - Facebook
 has .. design guidelines
 we also have a team dedicated to f.e. eng.
 the job of that team is to build those components
 you don't have to think about ... specific platform
 you take that UI comp. as a black box

 - quip
 being a startup
 only one designer
 we also like to use the phrase
 "strongly inspired"
 as in "this feature is strongly inspired by the iOS design"
 often instead of having to do it from scratch

 "Have you looked into middleware? Like in the games industry, Unity"

 - Instagram
 you're going to have to sacr. perf.
 we use webviews
 but even webviews slwo down the perf. of mobile web

 - FB
 at fb we haven't used that
 our product is compl. enough that
 ... you lose a lot of control to ... make our app 10% faster
 a lot of this stuff has been gradual

 we need to support one more platform
 and this looks like the most nat. and straihhtf. way to do this

 push as much as possible to behind an API

 instead of interesting interactions

 "Do you use 'cortical buffers'" ?

 - Quip
 they're excellent across languages
 if you're trying to go from java
   to our C++
   to our JS web code
   etc.
   it's nice to be able to send around a bytestream
   that each client knows how to ....
   that we can pass around to all the different platforms

---

All images and quotes fall under [fair use][fair-use] and are intended for purely educational purposes.

This document is licensed under a [Creative Commons Attribution 3.0 United States (CC By 3.0 US) License][cc-by-3].
[fair-use]: http://en.wikipedia.org/wiki/Fair_use
[cc-by-3]: https://creativecommons.org/licenses/by/3.0/us/

---
