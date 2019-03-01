---
title: Download
heading: Download Space Jawns
description: Downloads are currently available for Windows, Mac, Linux, and Android operating systems.
permalink: /download/
pricing_table:
  - name: Windows
    icon: <i class="fab fa-windows fa-3x fa-white"></i>
    color: "#0078d7"
    features:
      - text: <strong>Version</strong><br />3.0.0-Alpha
        highlight: false
      - text: <strong>Released</strong><br />02/28/2019
        highlight: false
      - text: <strong>Changelog</strong><br /><a href="/changelog">View Changelog</a>
        highlight: false
    call_to_action:
      link: /download#windows-downloads
      text: Download for Windows
  - name: MacOS
    icon: <i class="fab fa-apple fa-3x fa-white"></i>
    color: "#7d7d7d"
    features:
      - text: <strong>Version</strong><br />3.0.0-Alpha
        highlight: false
      - text: <strong>Released</strong><br />02/28/2019
        highlight: false
      - text: <strong>Changelog</strong><br /><a href="/changelog">View Changelog</a>
        highlight: false
    call_to_action:
      link: /download#mac-downloads
      text: Download for MacOS
  - name: Linux
    icon: <i class="fab fa-linux fa-3x fa-white"></i>
    color: "#282828"
    features:
      - text: <strong>Version</strong><br />3.0.0-Alpha
        highlight: false
      - text: <strong>Released</strong><br />02/28/2019
        highlight: false
      - text: <strong>Changelog</strong><br /><a href="/changelog">View Changelog</a>
        highlight: false
    call_to_action:
      link: /download#linux-downloads
      text: Download for Linux
  - name: Android
    icon: <i class="fab fa-android fa-3x fa-white"></i>
    color: "#A4C639"
    features:
      - text: <strong>Version</strong><br />3.0.0-Alpha
        highlight: false
      - text: <strong>Released</strong><br />02/28/2019
        highlight: false
      - text: <strong>Changelog</strong><br /><a href="/changelog">View Changelog</a>
        highlight: false
    call_to_action:
      link: /download#android-downloads
      text: Download for Android
faqs:
  - question: Is there a Space Jawns iOS version?
    answer: No. I am currently looking into a newer version of the iOS Developer license so that I can start building and testing Space Jawns for the iOS without paying their yearly fee.

  - question: How large is the install?
    answer: The extracted Space Jawns installation is currently less than X MB as of the X.X.X release.

  - question: Is there any DLC?
    answer: No. Space Jawns currently does not offer any Downloadable Content. We currently only have plans to release standalone versions in the Space Jawns series.

  - question: How much does Space Jawns cost?
    answer: Space Jawns is currently in Alpha, so it is not currently for sale. The Alpha and Beta versions of Space Jawns will be free to play. The final version price is TBD.
    
  - question: Are there any plugins or addons?
    answer: No. We currently do not have any sort of plugin system integrated into the game. We do have plans to support plugins in our Roadmap.

  - question: When will the next version be released?
    answer: Space Jawns releases are typically released every few months to add new content and fix existing major bugs. New releases are available on the downloads page.
---

<div class="plans">
  {% for plan in page.pricing_table %}
    <ul class="plan">
      <li style="background: {{ plan.color }}">
        {{ plan.icon }}<h3>{{ plan.name }}</h3>
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

<h2 id="windows-downloads">Windows Downloads</h2>
  - [Windows 64-bit download](https://www.dropbox.com/s/x5muyy79zsfeeo5/Space-Jawns-2.6.1-Alpha-Win64.exe?dl=1)
  - [Windows 32-bit download](https://www.dropbox.com/s/39q9ehud4im6tnv/Space-Jawns-2.6.1-Alpha-Win32.exe?dl=1)

<h2 id="mac-downloads">Mac Downloads</h2>
  - [MacOS 64-bit download](https://www.dropbox.com/s/dl8ttd2qypm5u2h/Space-Jawns-2.6.1-alpha.app.zip?dl=1)

<h2 id="linux-downloads">Linux Downloads</h2>
  - [Linux 64-bit download](https://www.dropbox.com/s/x5muyy79zsfeeo5/Space-Jawns-2.6.1-Alpha-Win64.exe?dl=1)
  - [Linux 32-bit download](https://www.dropbox.com/s/39q9ehud4im6tnv/Space-Jawns-2.6.1-Alpha-Win32.exe?dl=1)

<h2 id="android-downloads">Android Downloads</h2>
  - [Android Download](https://www.dropbox.com/s/7hg0dgxu9zaglta/Space-Jawns-2.6.1-Alpha.apk?dl=1)

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
