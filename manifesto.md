---
layout: page
title: Design Manifesto
---

In the course of studying design, it often felt like we were reading about little-related techniques which had little to do with each other, except that they could all be inserted at some point in the design process. And if we had left it at reading about techniques, it wouldn't much surprise me if it never would have come together, and remained a jumble of half-memorized trivia.

Making the attempt at putting theory into practice makes a huge difference to understanding the problem space. Of course, this generalizes beyond simply learning about design; it's actually quite widely applicable. But the process is particularly necessary when everything builds on top of everything else, and a lot of feedback is needed to make sure nothing is going terribly wrong.

Having come out of that, it's hard to make any kind of satisfyingly resolute pronouncements. But there are few particular noteworthy insights that, I feel, distinctly impact the priorities I would set when working on new designs in the future.

## Accessibility above all

[One of our accessibility readings](http://redish.net/images/stories/PDF/InteractionsPaperAuthorsVer.pdf) made the point I found insightful that improving accesibility for users working with assistive technology also tends to improve usability for users in general. I think this is a point that can be flipped on its head to make a stronger, an not less true, claim though: the same factors that make accessibility worse for users working with accessibility tend to degrade usability for usability in general.

I think this is a better framing for thinking about accessibility, at least on the technical side, in that it sets acccesibility up as a default, rather than an extra to be considered as an afterthought. When working with computers, after all, the default state of being (unstyled plain text, more or less, modulo encoding hassles) is fairly accessible as things go, being a format which is simultaneously readable without special tools, but also a source format that almost all assistive technology is already well-equipped to deal with, if only because it's so common. Moreover, nothing gets in the way of the user restyling or enlarging or voice-to-texting it as they see fit.

From here, in the direction of more accessible, we can add headings, semantic annotations, and so on, which are just as useful to present organization structure to general users as to those using assistive technology.

But what I think is key is to consider *additional requirements* to be factors that make accessibility *worse* unless mitigated. For example, adding images imposes a requirement that the reader be able to see; it should be mitigated if possible by presenting the content in an alternative format that doesn't require vision, e.g. good alt-text or a caption. Styling that affects layout makes accessibility worse by imposing a requirement that the viewer's renderer be able to correctly reorder contents; it should be mitigated by ensuring that, when ignoring the styling, the relevant content is at the top of the page. Links make accesibility worse, by requiring the user follow them in order to see what they lead to; this should be mitigated by making them descriptive enough to understand their purpose in context without necessary following them immediately.

As for the actual execution of making designs accessible, it seems that the important element is just ensure that all information in reasonably parseable form for assistive aids to be able to retrieve. That requires the information to be input in such a form in the first place, so accessibility essentially must be one of the first things considered for when presenting any content, since accounting for it impacts the content itself.

## Ethics is a design choice, not an afterthought

The design process has no particular place for ethics. I don't mean that in the sense that ethics isn't something to consider in the process; but I don't think it makes any sense at all to consider as a separate entity, since it's not possible to simply insert an ethics checkin step at some point in the design process. There are at least three ways I've identified that things can go wrong, ethically, that have to be addressed throughout the design process:

- Sometimes poor implementations lead to tragedy. To be frank, I can only consider these sorts of incidents to be an ethical matter in the case where the scope of the problem was known in advance, and the implementors did not perform diligence due to the gravity of those goals. Beyond that, unfortunately, there are limits to what we can expect humans to do.

  For my own standards, I consider it the responsible thing to do to ensure that whatever products I deliver operate as specified, and to fix them if they don't. Sometimes, this means fixing the specification, because the limits of the media in which the product is built make the specified behaviour infeasible or too easy to get wrong; as such, there needs to be close attention from the design phase through implementation to ensure that everything worse as intended. To power through implementing things poorly, and separately designate a testing/QA phase, as some are wont to do, unavoidably means leaving poor design choices baked in once they're too entrenched to be fixed.

  In the end, ultimate responsibility falls on whoever delivers a product and declares its purpose, and it would be poor form to chide those who disclaim all representations and warranties when their parts break, rather than whoever willingly chose to integrate those parts. But it would be nice to have have _some_ guarantees.

- Other times, products are misrepresented, or else they do some particular thing, and it's not at all what people really want. To this category, I submit all types of data-based learning, whose true function is to faithfully regurgitate whatever biases then were trained with, regardless of whether they're true, useful, or desirable; when really, all anyone ever wanted was a reliable source of objective truth.

  I think those products and components are valuable in their own right, and if used with full knowledge of how to interpret them and understanding of their limitations can only be better than not having information from them at all. But that knowledge has to be present at every point where they are incorporated, wchich for different components means different points in the design.

- Finally there are designs that are, per se, inherently unethical. Implementing them exactly as conceived would be a terrible thing in its own right. The right place to catch these is really at the ideation phase, but in a sense these are also the easiest types of ethical violations to put an end to, since at any point before the product reaches wide distribution, if someone convincingly point out that it's really a terrible idea, it can be scrapped.

  However, my impression is that such clear-cut cases are quite rare. More often, what seems clearly bad to one person, is really a product which benefits some users at the expense of others in the general public. After all, there aren't that many reasons to build products of benefit to nobody at all. But then the category of things that benefit some groups at the expense of others is huge, and includes pretty much all advertising, social networks built by extroverts with no sense of personal privacy, any usage of subsidized resources, filesharing, &c., along with less contentious examples, like glass staircases that people can look up through, or robbery and premeditated murder as a service.

  There should be a line somewhere, and it's not totally clear whether it belongs somewhere among the first category, or even further left from all of the above. I'd like to say that we should consider the good of all mankind when assessing whether a product is too unethical to make, but almost everyone is actually pretty bad at thinking on behalf of all humanity, so what I really mean is I'll take into account the preferences of people close to me and/or are like-minded to me, but that gets us nowhere in terms of avoiding ideas that are mostly bad to people who are not like me, which requires taking more, different, people's preferences into account.

## Being up-front with the product

It's nice, if ideally invisible, when a product functions as intended and also has a well-polished, intuitive design.

It can be a bit tedious when a product actually does do exactly what you need, but it takes a bit of wrangling to get it to comply.

It is _immensely_ frustrating, to come across a design that purports to accomplish something, seems to do so on cursory examination, but on closer examination can't manage to do so reliably.

Put another way, it is far worse to do a job wrong, but "well", than to do the right thing, but overtly poorly. Part of it is a perception thing which crops up in all sorts of places, like how in testing, participants will focus more on details than general design when shown higher-fidelity prototypes. When it comes to delivering product, a more polished product leads users to consider it more deeply, independent of whether it actually solves their problem. But by the same token, a polished, poor product leads users to _waste_ more time evaluating it.

Except for very limited classes of product, I don't think it is a right and proper goal to maximize the _number_ of users for a product; rather, we should work at increasing the amount of value delivered to users, factoring in costs; making a product look good when it doesn't do its job provides users _negative_ value.

Meanwhile, accurately labelling the product, making it behave as its affordances suggest, and making its behaviour compositional enough for potential users to infer its possible uses without needing them to be explicitly enumerated, in basically a matter of responsible representation.

Actionably, this means that the polish goes on _after_ the functionality is complete; false affordances are worse than no affordances.

## Better to do too little than too much

In the same vein, a design that incorporates too many tasks to handle them all properly, on the whole, worse than one that doesn't quite solve every problem that might come up, but is reasonably forthcoming about its limitations and doesn't get in the way of using a different tool to work around them. I think there's a temptation to add features to the requirements for a design, just in case, even if it's only tangentially related, before we've fully thought out what we're going to do with it and how it's going to work. For example, in our project, our initial design was full of ideas to enable people to communicate directly through our platform, but none of this made it through because it was actually rather hard to take them from half-baked to something that could be integrated in with the rest of the design.

The biggest danger of scope creep is winding up with a product that does a zillion things, none of them well enough to be worth using, and not well integrated enough to provide a cohesive environment. That's a waste of users' time, and, as I've said, provides negative value, which is bad. Anything going into the design should be done well; this, too, is as much as anything about being honest and responsible with what the product is and what problems it addresses.

## The inside must be beautiful, too

A good design needs to build on solid foundations. A set of incremental updates to bring an organically grown codebase with vastly different previous requirements up to a new specifications or the like is a recipe for broken assumptions leading to subtle bugs that add up to achieve murder. Most cases are not *quite* as extreme, but changing requirements makes it easy to break assumptions for about the same reasons that mutable global state is a bad idea: constraints that were previously true aren't accounted for by new additions, and old components that relied on those constraints holding start behaving wrong.

For that reason, whenever requirements change, it's useful to reexamine the entire design for places where those requirements imposed constraints or provided guarantees, leading to cruft or incorrectness in the general case, repsectively, though how visible their effects are may vary depending on how well-organized the rest of the design process is.

Conversely, the benefit to having an elegant design in the first place is that it obviates the need for requirements to change; it was already general enough to accommodate the requirements.

## Do the right thing by default

More of an aphorism than a statement of an actionable principle, I strongly feel that it is fruitless to try enumerating the things that are right and should be done, and equally pointless to enumerate the things that are wrong and to be avoid. In other words, I have a rather low opinion of "Dos and Don'ts" lists.

Design is in no small part about things that are hard to explicitly state, because they're subtle enough that the vocabulary for them doesn't really exist, but feel more or less right or wrong. The defining element of good design is not that it does anthing in particular, but that it subtly provides correct information and doesn't get in the way. It's not something that's easy to get get right by starting with something subtly wrong in various way and correcting some of them from a checklist. You'll just end up with a design that's subtly wrong in different, maybe slightly fewer, ways.

Trying to achieve good design by following principles explicitly seems like trying to achieve good reading comprehension by using a dictionary, or trying to achieve good writing by using a thesaurus, or trying to achieve good cooking using a recipe, or trying to achieve insightful synthesis by quoting prior art. On the face of it everything you do may be _literally correct_, but it lacks nuance, contextual understanding, and general je ne sais quoi.

Principles need to be understood and internalized and fully generalized, not applied by rote. I don't know any alternative to lots of experience for this, so I'll have to work on that.
