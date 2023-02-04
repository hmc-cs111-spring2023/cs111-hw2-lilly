_Fill in each this file with your responses, placing each response after its
corresponding question._

---

**Question**

Pick three quotes from the readings about language design. Good candidates
are:

- Something you agreed with / resonates with your own experience
- Something you disagree with
- Something that is interesting, a new idea or perspective you'd like to remember
- Something you didn't understand

For each quote, describe what it was about the quote that led you pick it.

**Response**

*We should now think of a language design as a pattern for language designs, a
tool for making more tools of the same kind.* [Steele, 1998]

This stood out to me because in hindsight, it seems obvious but I haven't
thought of this before. Many people, when asked why they like coding, respond
that it's because of the sheer expressiveness it has, and this can only be
possible due to the open room that the languages have for growth. Suppose we had
Java but no ability to define our own custom classes; the use cases for it would
then drop significantly. 

I also want to bring in the interview I had with Amy Yuan during class, where
she was talking about how everything is streaming nowadays, how she misses the
simplicity of having a hard copy she could always own. I feel like coding also
feeds into this because no one can regulate what you do with the programming
language (aside from illegal activities I suppose), so it appears like you have
full control (though if progamming languages ever decide to start a subscription
model, I might quit being a CS major).

*Why shouldn’t those “interfaces” be as humanely designed as the ones we tap and
swipe?* [Pavlus, 2012]

This reminded me of a CS colloqium talk we had last semester, "Stop Writing Dead
Code." The idea is that programming languages can be much less opaque than they
currently are, it's just that people cling onto past traditions such that they
are anachronistic. An example that the speaker brings up is how we have the
standard of 80 columns of code before a linebreak (which I'm also adhering to
right now) because that's how long punchcards for code used to be.

I also wonder if there's also a factor of "gate-keeping" that was brought up in the
previous reading, "C is Manly, Python is for 'n00bs'". Once people get ahold of
a language, some snobs -- for the lack of a better term -- like to think that
they're one of the few who are 'smart' enough to get the language. This also may
contribute to some areas of language design staying fairly stagnant.

*The plan will change in real time to meet hte needs of those who work on it and
use it.* [Steele 1998]

This is a good reminder that ultimately, the language we will be desigining is
not just for us, but for everyone in the audience. I think this is what the
inclass exercises were trying to show when we're given random constraints such
as "only include things that would work on a rollercoaster." It may seem
nonsensical to us, but it's something that's necessary for others and thus must
be considered seriously when implementing a solution. 


---

**Question**

How would you know a well-designed language? What are the symptoms? How would
you know a poorly designed language? What are the symptoms?

**Response**

A well-designed language should be vaguely comprehendable to someone who has
read the very basic documentation. If, after doing a cursory tutorial, they are
still totally lost on how something works, the language designer has messed
up. There should be fluency and symmetrical vocabulary, as described by both
Fowler and Bloch. This promotes the idea of a language rather than a mishmash of
symbols thrown together (the likes of which aren't very well-received by
novices, as shown by Pavlus' experiment). 

In essence, it should have clarity. Thus, the opposite -- a poorly designed
language -- will obfuscate what it's doing and have unclear vocabulary. It will
require a close eye on the documentation at all times because otherwise, you
have no chance of understanding what it means.

---

**Question**

How might the themes of _Growing a Language_ relate to notions of fluency from last week's
class?

**Response**

In the previous reading, we discussed how DSLs should have limited
expressiveness, but still be able to showcase fluency by stringing together
expressions in a meaningful way. The same can be said for languages in general,
as we have seen in the Pavlus reading. However, I will note that there are some
discrepancies between the Fowler and Pavlus reading. Pavlus seems to advocate
for a more "English" language, as shown by his fake language Quorum. Fowler
disagrees, though, and states that oversimplifying things will introduce a lot
of synatic sugar that may even take away the clarity that it was trying to
introduce. Thus, there must be a balance between having an understandable
language and a concise one.

There is also a notion of "extending fluency." If we keep the base language
simple, it is easier to learn and look at, as befitting of the description that
Fowler provided. If there are more complicated tasks that a programmer might
want to accomplish, then they can grow the vocabulary of the language by
introducing their own custom code. By doing this, they give a name to some task
they want to do, and thus increase the expressiveness of the program they're
working with. This has the added benefit of having more comprehendable code.
You can parallel this with how in the Steele reading, Steele kept defining new
words and grammar structures so that he could express himself better.

---



**Question**

In what way is an API a language?

**Response**

An API has its own unique vocabulary (usually through specific function calls,
sometimes also has their own objects). They are not just variable assignments;
you can manipulate things using the API, and also make an expression by
stringing together vocabulary from the API. For instance, you might have
apiObject.getId() which clearly gets the ID of the api object. 

---

**Question**

What does the post on grayscale tell us about the process of API design?

**Response**

It shows me that there is a surprising amount of thought involved in introducing
a new function. There is also more "audience participation" than I thought, as
they are polling users what their preferred naming scheme is. The comments were
interesting to read as well. I already thought 3 ways to name the same function
was a stretch, but there are even more perspectives than I thought. Some things
that are clear to me are not clear to them, and the opposite is also true. One
user suggested tint which seemed unintuitive to me because a) it's not specific
to gray scale b) tint is usually explictly for making things lighter, at least
in the painting world.

---

**Question**

The Pavlus article mentions the researchers' comments that people preferred
"natural-language replacements for some of the more abstruse syntax". In other
words, people found it easier to work with code that looks more like a human language (e.g.,
English). Consider the following quote by William R. Cook, one of the creators
of AppleScript:

> The experiment in designing a language that resembled natural languages (English
> and Japanese) was not successful. It was assumed that scripts should be
> presented in “natural language” so that average people could read and write
> them. … In the end the syntactic variations and flexibility did more to confuse
> programmers than to help them out. It is not clear whether it is easier for
> novice users to work with a scripting language that resembles natural language,
> with all its special cases and idiosyncrasies. The main problem is that
> AppleScript only appears to be a natural language: in fact, it is an artificial
> language, like any other programming language. … even small changes to the
> script may introduce subtle syntactic errors that baffle users. It is easy to
> read AppleScript, but quite hard to write it.
> [[Cook 2007, page 1-20]](https://dl.acm.org/citation.cfm?doid=1238844.1238845)

Are these two experiences of natural languages at odds with one another? Would
you choose to include natural language in the design of a DSL? If so, how might
you do so? If not, why not?

**Response**

I don't think these experiences are necessarily at odds with each other. Pavlus'
article was catered towards the average person who did not know much about
programming. However, it seems like the problems people found with AppleScript
were programmers themselves. So one could infer that languages that resemble
natural ones are more easily comprehendable by regular people, but they
frustrate programmers because it isn't as concise and clear cut. Think of
Scratch, for example. It's great for people starting to learn how to code, but
programmers will feel annoyed because they have to use blocks instead of just
typing it out. 

I think I would include natural language to a certain extent, but not more than
Python does. For example, I feel like the 'in' keyword in Python is very clear,
and is preferable to some of the way other languages do it. So I think having
small fragments would be good, but not full sentences which might introduce a
 syntatic sugar and confusion.

---
