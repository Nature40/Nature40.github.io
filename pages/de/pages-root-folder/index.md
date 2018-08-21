---
#
# Use the widgets beneath and the content will be
# inserted automagically in the webpage. To make
# this work, you have to use › layout: frontpage
#
layout: frontpage
header:
  image_fullwidth: header_unsplash_12.jpg
widget1:
  title: "Natur 4.0 im Überblick"
  url: '/pages/de/about/one-page-summary'
  image: widget-1-302x182.jpg
  text: 'Flächendeckendes Naturschutzmonitoring durch vernetzte Sensorik als Grundlage für einen nachhaltigen Artenschutz und die Sicherung von Ökosystemfunktionen.'
widget2:
  title: "Das Team von Natur 4.0"
  url: '/pages/de/team'
  text: 'Vernetztes Naturschutzmonitoring erfordert ein vernetztes Team im Querschnittsverbund aus Wissenschaft, Praxis und Bildung.'
  video: '<a href="#" data-reveal-id="videoModal"><img src="http://phlow.github.io/feeling-responsive/images/start-video-feeling-responsive-302x182.jpg" width="302" height="182" alt=""/></a>'
widget3:
  title: "Fragen und Kontakt"
  url: '/pages/de/qa-contact'
  image: widget-github-303x182.jpg
  text: 'Waldspaziergang mit Roboter? Hier finden Sie Antworten auf allgemeine Fragen und Kontaktinformationen.'
#
# Use the call for action to show a button on the frontpage
#
# To make internal links, just use a permalink like this
# url: /getting-started/
#
# To style the button in different colors, use no value
# to use the main color or success, alert or secondary.
# To change colors see sass/_01_settings_colors.scss
#
# callforaction:
#  url: https://tinyletter.com/feeling-responsive
#  text: Inform me about new updates and features ›
#  style: alert
permalink: /index.html
#
# This is a nasty hack to make the navigation highlight
# this page as active in the topbar navigation
#
homepage: true
---

<p id="twitter-target"><button onclick="setShowTwitter()">Ich bin damit einverstanden, dass mir Inhalte von Twitter angezeigt werden.</button></p>




<div id="videoModal" class="reveal-modal large" data-reveal="">
  <div class="flex-video widescreen vimeo" style="display: block;">
    <iframe width="1280" height="720" src="https://www.youtube.com/embed/3b5zCFSmVvU" frameborder="0" allowfullscreen></iframe>
  </div>
  <a class="close-reveal-modal">&#215;</a>
</div>
