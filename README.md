# AlignIt

AlignIt is a Chrome extension that solves a bug found on Canvas LMS. It could just be some weird error produced when using Cidilabs, although I am not exactly sure why the bug occurs.

## The Bug
There are some "alignment issues" that happen involving accordions/tabs/expanders. From time to time, a specific tab may not have its expected content. Sometimes, the content could be found in another tab or even outside the group of tabs.

## Cause
What I've found so far is that whenever this happens, usually, the id for the title of the tab and the id for its content doesn't match up. For example, the tab could have an id of "kl_panel_0", but the content has an id of "kl_panel_1_content".

## Current Solution
Parse through HTML code and make sure the numbers in the id match up.

## TODO
* Build UI
* Parse through HTML code using Javascript
* Run tests using previous code that resulted in the bug
* Publish extension