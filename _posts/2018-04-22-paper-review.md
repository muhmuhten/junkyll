---
layout: post
title: Paper review
---

### Paper
Schildbach, B., Rukzio, E., 2010. Investigating selection and reading performance on a mobile phone while walking. In: Proceedings of the 12th International Conference on Human Computer Interaction with Mobile Devices and Services. MobileHCI ׳10. ACM, New York, NY, USA, pp. 93–102. URL 〈http://doi.acm.org/10.1145/1851600.1851619〉.


## Commentary

I read Schildbach and Rukzio's "Investigating Selection and Reading Performance on a Mobile Phone while Walking”, in which the authors, noting that people often walk and operate their phones, investigate how much worse people are at using their devices when they’re also simultaneously using their legs.

The authors found negative effects on both target acquisition, i.e. pressing within a box, and reading comprehension, when using a phone while walking a designated path vs. while standing. They further assessed whether increasing size of the targets could mitigate the negative effects, finding that increasing target size increased success rate for the target acquisition task, but not the reading comprehension task. The authors found very large, disproportionate increases in scrolling when text size was increased and attribute the lack of improvement with increased text size to the increase need for scrolling. This doesn’t really seem like the most plausible explanation to me, since it doesn’t seem plausible that, among all of the tested text sizes, the relationship between scrolling behaviour and increased legibility is such an exact tradeoff that there is, the figures suggest, almost no difference whatsoever between reading speeds and text size; all of the walking conditions have visually approximately the same mean and variance for reading speed, which suggests to me that it actually just didn’t make any difference at all, which seems most likely to indicate that no reading per se happened at all. The procedure itself for the reading comprehension assessment is a bit suspect, since generally the sort of things people read on a walk are, I would expect, less likely to be read “for comprehension” and more likely for some reason like feeling like one is keeping up with the news, where actual comprehension is a low priority. Otherwise plausible; it’s actually pretty obvious, at least anecdotally, that it’s hard to get reading done while walking.

I do think that, with this paper’s results in mind, it may have been a good idea to design our mobile app to make it easier for the user to read through information not *right now*. As it is, our interface effectively invites the user to read through an analysis of a charity as they encounter it and decide there, or else have to find it again after leaving. This would be less of a hassle for something like a web page, where say, the page for one charity can be left loaded in one tab while the user looks at another, but for an app, it may actually be useful to expose some kind of bookmarking functionality orthogonal to actually donating to a charity for returning to easily it at a later point.
