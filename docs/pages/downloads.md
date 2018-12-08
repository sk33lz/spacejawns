---
title: Downloads
heading: Download Space Jawns
description: Downloads are currently available for Windows, Mac, Linux, and Android operating systems.
permalink: /downloads/
pricing_table:
  - name: Windows
    color: "#0078d7"
    features:
      - text: <strong>Version</strong><br />2.6.1
        highlight: false
      - text: <strong>Released</strong><br />12/15/2018
        highlight: false
      - text: <strong>Changelog</strong><br /><a href="#">View Changelog</a>
        highlight: false
    call_to_action:
      link: http://mysite.com?plan=basic
      text: Download for Windows
  - name: MacOS
    color: "#7d7d7d"
    features:
      - text: <strong>Version</strong><br />2.6.1
        highlight: false
      - text: <strong>Released</strong><br />12/15/2018
        highlight: false
      - text: <strong>Changelog</strong><br /><a href="#">View Changelog</a>
        highlight: false
    call_to_action:
      link: http://mysite.com?plan=pro
      text: Download for MacOS
  - name: Linux
    color: "#282828"
    features:
      - text: <strong>Version</strong><br />2.6.1
        highlight: false
      - text: <strong>Released</strong><br />12/15/2018
        highlight: false
      - text: <strong>Changelog</strong><br /><a href="#">View Changelog</a>
        highlight: false
    call_to_action:
      link: http://mysite.com?plan=pro
      text: Download for Linux
  - name: Android
    color: "#A4C639"
    features:
      - text: <strong>Version</strong><br />2.6.1
        highlight: false
      - text: <strong>Released</strong><br />12/15/2018
        highlight: false
      - text: <strong>Changelog</strong><br /><a href="#">View Changelog</a>
        highlight: false
    call_to_action:
      link: http://mysite.com?plan=professional
      text: Download for Android
faqs:
  - question: Is there a Space Jawns iOS version?
    answer: No. We currently do not have an iOS version. A new developer license is now available that we are looking to apply or soon to develop for iOS.
  - question: How much does Space Jawns cost to download?
    answer: Space Jawns is currently in Alpha, so we are not currently selling the game. The Alpha and Beta versions of Space Jawns will be free to play.
  - question: How large is the install?
    answer: The extracted Space Jawns installation is currently less than X MB as of the X.X.X release.
  - question: Is there any DLC?
    answer: No. We currently do not offer any Space Jawns DLC. We currently only have plans to release standalone versions in the Space Jawns series.
  - question: Are there any plugins or addons?
    answer: No. We currently do not have any sort of plugin system integrated into the game. We do have plans to support plugins in our Roadmap.
---

<div class="plans">
  {% for plan in page.pricing_table %}
    <ul class="plan">
      <li style="background: {{ plan.color }}">
        <h3>{{ plan.name }}</h3>
      </li>
      {% for feature in plan.features %}
        <li {% if feature.highlight %} class="highlighted"{% endif %}>{{ feature.text }}</li>
      {% endfor %}
      {% if plan.call_to_action %}
        <li class="pricing-cta"><div class="button"><a style="background: {{ plan.color }}" href="{{ plan.call_to_action.link }}">{{ plan.call_to_action.text }} &rarr;</a></div></li>
      {% endif %}
    </ul>
  {% endfor %}
</div>
{% if page.faqs %}
  <h2>Space Jawns Downloads FAQs</h2>
  <dl class="faq">
    {% for item in page.faqs %}
      <div>
        <dt>{{ item.question }}</dt>
        <dd>{{ item.answer }}</dd>
      </div>
    {% endfor %}
  </dl>
{% endif %}
