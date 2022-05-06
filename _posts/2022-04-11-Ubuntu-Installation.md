---
layout: post
title: Configuring Ubuntu LTS
categories: [Tech Tech Hooray]
usemathjax: true
comments: true
---

Purchasing a new laptop can be exciting, but reinstalling applications and programs from your former laptop is a pain. Recently, I retired my ASUS Zenbook and upgraded to the [Lenovo IdeaPad 5](https://www.bestbuy.ca/en-ca/product/lenovo-ideapad-5-15-6-laptop-abyss-blue-amd-ryzen-7-5700u-512gb-ssd-16gb-ram-windows-11/15701037?cmp=seo-15701037&cmp=knc-s-71700000068294177&gclid=EAIaIQobChMI943xidet9wIVj21vBB2HvgKEEAQYASABEgI1LfD_BwE&gclsrc=aw.ds). This new laptop ticked all the boxes, (criteria provided in Ayo Isaiah's [article](https://www.freecodecamp.org/news/how-to-choose-a-laptop-for-programming-a9e36f8b4cfe/)), but configuring Ubuntu LTS was a tad more difficult than I initially thought.

The most common operating system is the microsoft windows OS. However, windows users can run Linux on windows a few different ways, one of those being through the use of WSL, or *Windows Subsystem for Linux.* In my case, I required access to my office computer and the only way I knew how to do this was by installing WSL on my home laptop to be able to use ssh client. The advantage of WSL is that you can run Linux applications, such as ssh client, without the extra weight of a virtual machine <sup>[1](https://solarianprogrammer.com/2017/04/15/install-wsl-windows-subsystem-for-linux/).
  
So, I excitedly pulled out the file from an undergraduate course in scientific computing with C++ and started pouring through the notes until I found a handout from my instructor detailing how to set my laptop up to support Linux. 
  
Great!

First thing to do was to enable *Developer Mode.* This is done by navigating to Settings &#8594; Update & Security &#8594; For Developers and then checking off the *Developer Mode* box.
  
Alright, so far so good!
  
Next up was enabling *Windows Subsystem for Linux,* which can be done by navigating to *Windows Features* panel and checking off the respective box.
  
Wonderful!
  
Finally, it was time to download *Ubuntu* from the Microsoft store...error: kernel needs to be updated. The Ubuntu terminal will immediately exit out if you try to type anything in it following the error message...as I learned after about 15 tries, but I digress. Luckily, there was a quick fix to this minor issue; update the kernel! I initially didn't plan on creating a blog post about configuring Ubuntu LTS, so I did make note of the exact error code that appeared and what I did to remedy it.

