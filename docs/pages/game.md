---
title: Game
heading: About Space Jawns
description: Learn what Space Jawns is all about, how to play the game, and the game controls.
permalink: /game/
site_name: true

faqs:
  - question: What software is Space Jawns being developed with?
    answer: Space Jawns is being developed in Unity 3D using C#.
  - question: Are there on-screen controls for Android?
    answer: No, but we do plan on adding that feature in an upcoming update.
  - question: How many developers are on the development team?
    answer: Space Jawns is written by a solo developer currently.
  - question: Got more questions?
    answer: Contact us for any further questions on the <a href="/support" title="Space Jawns Support">Support</a> page.
---

<nav class="page-menu" role="navigation" aria-expanded="false" aria-label="Page menu">
  <i>Jump to:</i>
  <ul>
    <li class="first"><a href="/about">About the Game</a><i class="fas fa-grip-lines-vertical"></i></li>
    <li><a href="/game#how-to-play">How to Play</a><i class="fas fa-grip-lines-vertical"></i></li>
    <li><a href="/game#controls">Controls</a><i class="fas fa-grip-lines-vertical"></i></li>
    <li><a href="/game/changelog">Changelog</a><i class="fas fa-grip-lines-vertical"></i></li>
    <li class="last"><a href="/game/credits">Credits</a><i class="fas fa-grip-lines-vertical"></i></li>
  </ul>
</nav>

<h2>About the Game</h2>
Space Jawns is a Classic space shooter game series built for today's computers and mobile devices. Space Jawns has been inspired by 30+ years of playing space video games, and more recently the constant release of early access games on Steam. The first space games I ever played were on the Atari and Commodore 64 systems with games like Space Invaders, Galaga, and Zaxxon. These games were some of the most polished space games I have ever played, hands down. There were no early access releases, no Post-Release patches, and definitely no Pay to Win games in those days. The only thing you were paying for was the quarter to possibly get your name on the high score list. I call these the Golden Years of video games, and they are what have inspired Space Jawns from it's core.

As computers advanced over the years, I moved onto DOS games like TIE Fighter, then more advanced Windows games like Freelancer, and eventually my favorite to date, Star Wars Galaxies: Jump to Lightspeed. The space gameplay in Jump to Lightspeed was a great throwback and update to the old X-Wing/TIE Fighter games. It was very sad to see it go when SOE shut down the SWG servers in Dec. 2011. Since then, there have been some attempts to create the next best space game, and right now it looks like Star Citizen may hold that title, as it is really pushing the limits to what could be the greatest space game to date.

Space Jawns was created as an ode to what space videos games used to be in those Golden Years of video games. It strives to set an example of what video games should continue to be today. That means a completed game that is FUN and AFFORDABLE for all ages! I am not going to be selling Early Access to Space Jawns. You get to play it for free like any other normal Alpha or Beta Testing that software companies do where they want Gamers to test the game and provide feedback. I am not looking to get rich and then never finish my game, which I feel is a big issue with game developers currently releasing games through Steam's greenlight program. My goal is to listen to Alpha and Beta tester feedback to make a better game wherever possible. The main goal is to complete the game before trying to sell it. I think that's a pretty fair deal for those who may want to purchase it once it's ready for release.

Thank you for taking the time to read about Space Jawns. Now you should go [Download Space Jawns](/download). Once you have given it a try join the Space Jawns Discord channel to report bugs, give feedback and suggestions, or ask questions about the game so far. Your feedback is greatly appreciated!

Thanks!

Jason

<h2 id="how-to-play">How to Play</h2>
The main objective of Space Jawns is to get the highest Score before all of your ships are destroyed by enemy ships, asteroids, or Enemy Turrets.

<h2 id="controls">Controls</h2>

### PC/Mac/Linux Controls

#### Keyboard Controls
**Move Left:** A, Left Arrow, Joystick/Gamepad Left X-axis.
**Move Right:** D, Right Arrow, Joystick/Gamepad Right X-axis.
**Fire 1:** Space Bar, Left Mouse Button
**Pause:** P or Escape
**Take Screenshot:** F5
**Quit:** Escape

### Android Controls

**Move Left:** Tilt device to left like a steering wheel.
**Move Right:** Tile device to right like a steering wheel.
**Fire 1:** Tap your screen.
**Take Screenshot:** Use Native screenshot gesture.
**Quit:** Return to Home

{% if page.faqs %}
  <h2>Space Jawns Game FAQs</h2>
  <dl class="faq">
    {% for item in page.faqs %}
      <div>
        <dt>{{ item.question }}</dt>
        <dd>{{ item.answer }}</dd>
      </div>
    {% endfor %}
  </dl>
{% endif %}
