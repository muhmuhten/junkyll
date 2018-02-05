---
layout: post
title: Reasonable design
---

On page load
![No selection](../img/Screen Shot 2018-02-05 at 00.49.36.png)

Click "Mission Park"
![Mission Park](../img/Screen Shot 2018-02-05 at 00.49.46.png)

Click "Williams' Bakeshop"
![Mission Park/Williams' Bakeshop](../img/Screen Shot 2018-02-05 at 00.45.58.png)

Click "Driscoll"
![Driscoll/Williams' Bakeshop](../img/Screen Shot 2018-02-05 at 00.46.04.png)

Click "Whitmans' Marketplace"
![Whitmans' Marketplace/Williams' Bakeshop](../img/Screen Shot 2018-02-05 at 00.46.13.png)

Notice that as the upper-level selection is changed, the lower-level selection
remains on "Williams' Bakeshop" without requiring reselection.

To put it another way, this fixes the really common issue where redoing a
higher-level selection requires redoing all lower-level selections, which makes
it tedious to compare the food being offered at multiple locations in the
common case: for deciding which dining hall one wants to walk to right now,
based on what food is being served.

With this relatively new design, switching the location selection keeps the
same meal selection, so it's possible to compare changing only the location.
