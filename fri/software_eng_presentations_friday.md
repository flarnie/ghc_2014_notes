#Software Engineering: Multiple Presentations
*Friday, Oct. 10, 2014*

**[Full Audio Recording of Software Engineering Presentations!][soft-eng-audio]**
*The first 10 minutes are really soft - It gets louder after about 13:00*

## A Case for Humanitarian Free and Open Source Software
**Chelsea H. Komlo; Software Developer, ThoughtWorks**

Discussed her involvement with the [Mifos Initiative][mifos-initiative];
"The one true open platform for financial inclusion"

[mifos-initiative]: http://mifos.org/

###Software Best Practices in Open Source Software
> "Software best practices improve code quality, not only in everday
> applications, but also most especially in [open source] applications.
> Managing a large open source project is really hard; with thousands of people
> around the world trying to make changes, ... some of the software best
> practices ...  such as continuous delivery, or test driven development, or
> refactoring, are really helpful in these types of projects.
>
> For example, I worked with some of my colleagues at Mithos to set up a build
> system ...  with TravisCI. ... That was really helpful to their team.
>
> We also helped with their testing, their test infrastructure."

###Getting Involved in Open Source
Her own story:
> "How did I get involved with this project?
> I was involved with the Mifos team for several months, joining them on
> development calls, ... testing, ... but really it started small.
>
> I heard a presentation much like this, and ... I was really inspired, so I
> went to their Github repo, and they had all of their issues listed, in great detail,
> and I picked up a couple of stories, and I added some fixes, and really the
> [barriar] to contributing is really small; ... so it's easy to get involved,
> and it's something that is easy for us because this is what we do every day."

How can you get involved?:
> "So how can all of you get involved?
>
> ... There are several ways:
> - Starting with documentation
> We added documentation talking about testing, and the test pyramid, and what
> kinds of tests do you write. ...
> - Become a core contributor
> Each of these projects have calls, maybe weekly or bi-monthly, to talk about
> new features that are coming out, ... doing some planning.. You can start
> getting involved at that level.
> - Apply your expertise
> If you're a data scientist, or if you do UX, or whatever kind of thing you do,
> I promise it will be helpful to [open source] applications ...
> ###Whatever you have to contribute, it will be helpful.
> - Recommend open source
> If you're working with a great ... organization that has really amazing
> tools, maybe talk to them about open sourcing their products, so that other
> organizations around the world might put this to use.
> Or if you're working with an organization that is just looking at building a
> tool, look and see if that tool exists elsewhere."

> "To wrap up ... I just want to return to the challenge to build technology for
> humanity. So, everybody in this room has had great opportunity. There have been
> tons of people who have helped us get where we are today. We're unbelievably
> blessed. ...
> ###I just want to challenge everyone to take what you have, and the skills and tools you have, and build technology for people who have much less."

## Beyond the Buzzwords: Test-Driven Development
**Sabrina B. Williams; Software Engineer, Google**

> I'm here to give you guys a practical knowledge of Test Driven Development.
> I'm not trying to sell you on it; I just think it's a fun thing to know.
> I don't neccesarily think it's good; I don't think it's bad; I do it sometimes,
> I don't do it other times.
>
> Unless you've actually tried doing it, you cannot explain it, because you're
> writing tests for code that doesn't exist.
>
> ![Writing tests for code that doesn't exist; I have no idea what I'm doing](./test_driven_development_meme.jpg)

> ###"What is Test Driven Development?
> ... It's just a highly iterative process by which tests are written before the
> production code is implemented. ...
> - Figure out what it is you want to test
> - Write a test for it
> - Run the test; the test should fail, because you have not yet implemented this feature
> - Implement the feature (in the simplest possible way)
> - Run the test again; the test will pass
> - Look at your code again ... clean it up a little bit. That's where the
>   refactoring part comes in."

> ###"What are some benefits of Test Driven Development?
> - You're only writing the code that's necessary to get the tests to pass
>   (So you're following KISS ... YAGNI ...)
> - You can't write your code without the tests ... high test coverage ...
>   making sure that you get that.
> - You end up with an extensive test suite
>   Then developers are responsible for writing their own tests, so you don't
>   have that throw-it-over-the-wall mentality that ... some have
> - Emphasis on testability that influences how you design your code.
>
> **This is not a typo (the next section has the same bullets)**
> ###Drawbacks of Test Driven Development
> - You're only writing the code that's necessary to get the tests to pass
>   If you're not careful, ... you can end up with some pretty funky, fragmented
>   stuff that doesn't fit together, so you have to pay attention ... keep the
>   overall architecture in mind.
> - You can't write your code without the tests
>   Depending on how ... you stick to this, you can get yourself stuck.
> - You end up with an extensive test suite
>   ... has to be maintained. If you start making a lot of changes ...
>   and it gives developers too high a confidence. You get very high unit test
>   coverage, but you still have to do your integration tests. You still have to
>   do your system tests. ... Sometimes, someone may not ... understand the
>   feature correctly. ... That's where code reviews come in really really handy.
> - Emphasis on testability that influences how you design your code.
>   Sometimes people get a little too happy with mocks, and fakes and stubs,
>    ... it can be hard to figure out what's going on in the code.
>   Sometimes folks may expose functionality that shouldn't be exposed, ... for testing.
>
> How do you reconcile those things?
>
> Use common sense.
> ###Don't go overboard trying to adhere to methodologies to strictly.
> ...
> Don't force everybody to do things exactly the way you do it, because everybody's
> different. What works for you may not work for them."

She addressed common questions that come up:
**Q:** What if you're working on legacy code?
> "It is difficult to try and do it when you're refactoring existing function.
> ... Just start off with the new things that you do ... "

**Q:** Writing tests when I'm prototyping is a waste of time, right?
> "If your prototype is likely to become production code, which a lot of [it]
> does, then maybe testing isn't bad. If you're sure that your prototype is
> never ever ever going to become production code, then maybe you don't have
> to spend a lot of time testing. This isn't even TDD specific, but in general."

**Q:** I'm in a start-up, I have all these deadlines; I don't have time for this!
> "Do you have time six months from now to deal with all the bugs, and crashing ...
> This one isn't even TDD either; just in general, testing. ..."

**Q:** We don't have automated testing set up, or any kind of testing culture.
How am I supposed to use TDD in this environment?
> "... First you have to get an environment where testing is important, and then
> you can go about figuring out how you wanna write your tests. ... Get your
> continuous integration system up, get some kind of test framework running,
> don't jump into TDD if you can't even write a test."

She also did a live coding demo of TDD using Go.

## Semantic-Based Code and Documentation Search Engine
**Reshma Thumma; Graduate Student and Teaching Assistant at the University of Missouri-Kansas City**

**WORK IN PROGRESS: I haven't transcribed this one yet.**

Check out the
[audio recording of the Semantic-Based Search Engine Presentation][soft-eng-audio]
(start at 15:00).

[soft-eng-audio]: https://soundcloud.com/paradasia/14-10-10-software-engineering
---

All images and quotes fall under [fair use][fair-use] and are intended for purely educational purposes.

This document is licensed under a [Creative Commons Attribution 3.0 United States (CC By 3.0 US) License][cc-by-3].
[fair-use]: http://en.wikipedia.org/wiki/Fair_use
[cc-by-3]: https://creativecommons.org/licenses/by/3.0/us/

---
[Official Notes on the Systers Wiki][softw-eng-fri-wiki]

[softw-eng-fri-wiki]: http://systers.org/wiki/communities/doku.php?id=wiki:ghc:ghc14:presentations_-_software_engineering
