---
layout: shared/narrow
title: "Accessibility Codelab"
description: "Accessibility Codelab"
published_on: 2016-03-01
updated_on: 2016-03-01
order: 41
translation_priority: 0
authors:
  - megginkearney
  - dgash
key-takeaways:
  tldr: 
    - "Learn what accessibility means and how it applies to web development."
    - "Learn how to make web sites accessible and usable for everyone."
    - "Learn how to include basic accessibility with minimal development impace."
    - "Learn what HTML features are available and how to use them to improve accessibility."
    - "Learn about advanced accessibility techniques for creating polished accessibility experiences."
notes:
  efficiency:
    - "Understanding the accessibility issue, its scope, and its impact can make you a better web developer."
  problem-solving:
    - "Catching, identifying, and removing potential accessibility roadblocks before they happen can improve your development process and reduce maintenance requirements."
---

# Don't Convey Information with Color Alone

There are roughly 320 million users with color vision deficiency. About 1 in 12 men and 1 in 200 women have some form of "color blindness"; this translates to around 1/20th, or 5%, of your users who will not experience your site the way you intend. When we rely on conveying information using color alone, we effectively push that number to unacceptable levels.

For example, in an input form, a telephone number might be underlined in red to show that it is invalid. But to a color deficient or screen reader user, that information is not conveyed well, if at all. Thus, you should always try to provide multiple avenues for the user to access critical information.

The WebAIM checklist states in section 1.4.1 that "color should not be used as the sole method of conveying content or distinguishing visual elements." It also notes that "color alone should not be used to distinguish links from surrounding text" unless they meet certain contrast requirements, which we'll cover in a bit. Instead, the checklist recommends adding an additional indicator such as an underscore (the CSS `text-decoration` property) to indicate when the link is active.

An easy way to fix the previous example is to add an additional message to the field, announcing that it is invalid and why. When you're building an app, keep these sorts of things in mind and watch out for areas where you may be relying too heavily on color to convey important information.

If you're curious about how your site looks to different people, or if you rely heavily on the use of color in your UI, you can use the [NoCoffee Chrome extension](https://chrome.google.com/webstore/detail/nocoffee/jjeeggmbnhckmgdhmgdckeigabjfbddl?hl=en-US) to simulate various forms of visual impairment, including different types of color blindness. 
