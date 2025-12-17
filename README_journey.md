# Journey

## Document Purpose

This md file documents the steps I took to build the site.

## Logs

### 15/12/25

I'm coming back to this after some time away. I made some decisions which are frankly a bit baffling. There are unused variables which I don't think I'll need. After completing the project I'd like to look at cutting out all the unused code. Next steps are to build out the fundamental tablet design. I'm not worrying about hovers or extra css interactivity for now.

One question I have is how to manage height sensibly. I'm using a lot of padding-bottom to ensure good vertical spacing between components and sections, but I think it's messy and I wonder if there is a more stable way to manage vertical space.

Wow, I used my first github yml workflow to ensure src was being compiled to GH Pages!

### 16/12/25

Today, I finished the tablet design and began working on the desktop header. I noticed that a bug arised from using the translate property on .hero-banner-img. On mob and tab, the image is a single image spanning the width of the website, but by the desktop design the image is split into two images. The original mob/tab solution used translate to move the image back by 5% and elongate the image by 10%. Which worked fine, until the class took two images. Then I found I was only able to update one images translate property. The moment I changed the mob/tab version to use translateX, I was able to override both image in the desktop design with translateX too.

### 17/12/25

Today I refactored the styles for download and details buttons. I was using an id for styling originally, but realised this was a mistake as there were two instances per header and we can't have multiple id's of the same value! I also learnt about finding pixel distances between two elements in figma. Select element one and then hold alt as you hover over the second element. Really helpful and will save me from using the grey custom blocks. This will also help me to apply appropriate padding and margin in future projects.

Another thought I had was that (at least while developing) in future projects I could create seperate files for the three main screen sizes. This mains mob.css would be created first, then tab.css with all styles nested in the tab media query. Finally I could create dsk.css for dekstop styles. I think this clear separation of concerns would help me develop.
