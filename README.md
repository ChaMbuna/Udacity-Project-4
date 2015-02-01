Cameron Pittman: Portfolio Website Optimization
===============================================

Goal
----
The PageSpeed score of 90 is for index.html (both mobile and laptop scores should be at least 90).

The frame rate of 60fps should be obtained for the pizza page (views/pizza.html). The file you need to study and change is views/js/main.js.

The original project is available at <a href="https://github.com/udacity/frontend-nanodegree-mobile-portfolio">https://github.com/udacity/frontend-nanodegree-mobile-portfolio</a>.

<a href="https://github.com/udacity/frontend-nanodegree-mobile-portfolio/archive/master.zip">Click here to download the project files</a>.

All files and links below are to my optimized version meeting the goals stated above.

Launching the website
---------------------
You can view the optimized website at <a href="http://chambuna.github.io/">http://chambuna.github.io/</a>

Alternatively, you can <a href="https://github.com/ChaMbuna/ChaMbuna.github.io/archive/master.zip">download the project files here</a>. Extract the files and open index.html to launch the site from your computer.


Optimizations
=============

Images
------
- Resolution was reduced when unnecessarily large
- All images are now hosted locally
- Thumbnails were made where necessary
- Filesize compressed with Photoshop & Kraken.io

JavaScript
----------
- Scripts not critical to build the DOM are loaded asynchronously
- Moved non-critical scripts to bottom of html

CSS
---
- CSS for print taken out of the critical rendering path
- stylsheet minimized and loaded inline
- unused id & class selectors removed from bootstrap framework

Fonts
-----
- Fonts are loaded with @font-face vs link rel


Pizza page spicific FPS optimizations
=====================================

- Scroll-position is now stored in variable outside of loop and no longer calculated for each pizza. (Idea adapted from http://www.webreference.com/programming/javascript/jkm3/index.html)
- Local function variables used to improve performance. (Idea adapted from http://www.webreference.com/programming/javascript/jkm3/index.html)
- Rewrote for loop for pizza sizes (calculations are now done outside of loop)

- Cleaned up generic code erros (using JSHint & Brackets)
- removed unnecessary function requestAnimationFrame & unused variable currentScrollY