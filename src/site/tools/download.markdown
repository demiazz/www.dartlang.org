---
layout: default
title: "Download Dart"
description: "The download bundles that support the Dart language."
has-permalinks: false
download_experiment: true
js:
- url: /js/download-info.js
  defer: true
---

# Getting Dart Is Easy!

<div class="btn-group-responsive btn-group hero-hldr btn-group-justified os-choices" style="display: table;">
  <div class="btn-group">
    <button type="button" class="btn btn-default btn-lg" id="windows">Windows (Vista, 7, 8)</button>
  </div>
  <div class="btn-group">
    <button type="button" class="btn btn-default btn-lg" id="linux">Linux</button>
  </div>
  <div class="btn-group">
    <button type="button" class="btn btn-default btn-lg" id="macos">Mac OS X</button>
  </div>
</div>

<div class="windows" markdown="1">
## Download Dart

{% include downloads/_get_dart_editor.html %}

## Or download just what you need {#windows-separate-download}
</div>

<div class="linux" markdown="1">
First install Dart, and then choose your editor.
(Want a one-click download?
Skip to [Step 2](#step-2) and choose **Dart Editor**,
which includes Dart.)
</div>

<div class="macos" markdown="1">
First install Dart, and then choose your editor.
(Want a one-click download?
Skip to [Step 2](#step-2) and choose **Dart Editor**,
which includes Dart.)
</div>

{% for platform in site.custom.downloads.binaries %}
{% capture partial %}downloads/_{{platform.os}}_section.html{% endcapture %}
<div class="{{platform.os}}" markdown="1">
{% include {{partial}} %}
</div>
{% endfor %}

<aside class="alert-info alert" markdown="1">
**Want another Dart version?**
Use the [download archive.](/tools/download-archive)
It lets you choose specific versions
of the Dart downloads.
It also has the latest **dev channel** builds,
which let you try new features a few weeks earlier than the stable channel.
</aside>

<div id="step-2">
<div class="windows" markdown="1">
### Pick an editor

[Dart Editor](/tools/editor/) isn't your only choice.
The following plugins add Dart smarts to popular code editors.

{% include downloads/_other_editors.markdown %}
</div>

<div class="linux" markdown="1">
{% include downloads/_step2_pick_an_editor.markdown %}
</div>

<div class="macos" markdown="1">
{% include downloads/_step2_pick_an_editor.markdown %}
</div>
</div>
