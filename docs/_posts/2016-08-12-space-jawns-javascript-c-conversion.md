---
date: 2016-08-12
title: Space Jawns Javascript to C# Conversion
categories:
  - game news
  - developer blog
author_staff_member: sk33lz
---

After coming up with the idea for space jawns, I figured I would use Javascript as the main scripting language for the game logic and storing game variables. This was due to the fact that I am a web developer by trade. Developing my game in Javascript was a way I figured I would be able to practice getting better at Javascript and coding in general, meanwhile I would be able to build the game in the process. THat has paid off considerably so far, as I have started to be able to read and decipher different languages of code much easier since starting the project. It's helping me understand and execute code as I build the game, and it has also given me a new outlook on my abilities as a Developer in general.

Unfortunately, I ran into some issues with an asset that I bought from the Unity Asset store, which required C# code. Instead of trying to workaround a bunch of issues I was having with my JS code, I decided to bite the bullet and convert all of my Javascript files to C#. The benefits of doing so are too many to list, but in general the game should perform much better and be easier to debug when issues arise. Aside from that most game developers are using C# over Javascript these days, and there are many more C# coding resources for Unity available in my experience. THe code is also usually cleaner, as C# is much less forgiving. It also supports many more built in functions out of the box that C# supports.

THe conversion process itself was something that I thought was going to be very painful and take a long time, but was slingshot forward with a helpful [JS to C# conversion tool](http://www.m2h.nl/files/js_to_c.php) I found online. This tool was not perfect, but it did about 80% of the work that would have been very tedious and time consuming. I ended up being able to convert 68 Javascript files from my original game to C# in what seemed like no time. It ended up I had a bunch of warnings and notices to clean up after the fact, but in the end I was able to convert my whole project from JS to C# in just a few days. This included fixing all code warnings, alerts, and Errors, remapping all scripts to gameobjects, and testing. The conversion and Testing is complete. We have already jumped ahead 2 minor versions to 2.3.0-Alpha in testing currently. 2.2.0 was the merge from Javascript to C# and 2.3.0 is an upgrade from Unity 4.6 to Unity 5! Overall both processes went pretty smoothly and we should have a 2.3.0-Alpha release available soon!

I also look forward to continuing to get better with my coding abilities and become more comfortable as a developer in whatever language I need to build with. As I said earlier, my day job is a web developer, and while I can build many things with the software I use to build websites without code, <a href="https://www.drupal.org/" title="Drupal CMS">Drupal</a>, I am in no way a great PHP developer. I am hoping that with the skills and experience I pick up on this project I can continue to become a better developer all around. Some of my biggest pitfalls in the past have been logic and large amounts of code. building this Space Jawns in one language and converting it to another has really helped build and expand that skillset. I'm looking forward to using my new Developer skills in more development tasks at my job. My new developer skills have already started helping me in my daily tasks at work in just the short time I have been developing Space Jawns. I can't wait to see where i am in a few years.

Happy Gaming and coding if you are into that sort of thing!

-Jason
