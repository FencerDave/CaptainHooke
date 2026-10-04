---
layout: post
title:  "Examples and Template for Media Uploads"
date:   2026-09-30 07:42:00 -0000
categories: blog
---
### Self-Serving post here, 
I'm new to this so it'll be useful to do my homework once and figure out how to include media of different types in these posts, so this is both an introduction to my world and projects, and a personal How-To guide for using Ruby/Jekyll (And I guess mostly this is me learning HTML..)
Ah, the "HyperText MarkupLanguage..."
To-Do: 
 - [x] Refresh my memory of managing links inside of posts! (And downloads?)
 - [x] Simple Image, alongside narration (learn to format and include along text?)
 - [ ] Image Gallery, scroll-through, for showing progress along a project or other many-images without clogging the post
 - [ ] Google Slides / Docs / sheets? etc- Apparently easy from File-->Share options as an <iFrame> link
 - [ ] PDFs - Can treat sort of as image, but may want to route through google iframe as per above. (Download links also important! Most browsers will open a download automatically in their preferred way) 
 - [ ] Youtube Embedded Player
 - [ ] Embedded StreamLit App - Tools that I make in Python, and want to be able to deploy for the world to use! (Streamlit hosts for free so long as it's a public Repo/project, and I think I can Embed that website in this page/post instead of having to link to the streamlit account page!)
<!--
Others? Recommendations from Claudius
 - [ ] Github GIST <script src="https://gist.github.com/USERNAME/GIST_ID.js"></script> renders a syntax-highlighted, embeddable code snippet
 - [ ] Math (KaTeX) — Hydejack uses KaTeX to efficiently render math, built in, no setup. Handy for anything electrochemistry-adjacent
 - [ ] Mermaid diagrams — not built in, but one <script src="...mermaid.min.js"> CDN tag plus a <pre class="mermaid"> block gets you flowcharts/sequence diagrams rendered client-side, no image export needed.
 - [ ] Interactive charts (Plotly/Observable) — if you ever want to embed a live data viz rather than a static plot image, a Plotly HTML export or Observable notebook embed both just drop in as iframes/script tags the same way Streamlit does.
-->
### General Formatting
 - Make Links like this: [which goes to a Jekyll Markdown Cheatsheet](https://gist.github.com/roachhd/779fa77e9b90fe945b0c)
 - Inline Formatting works like _italics_ as well as **bold** and `codeSnippets.print()`
   - Lists indexing use whitespace
   - And they can use dashes (-), asterisks (*), or plusses (+) for some reason.
 - Numbered lists can start with 1. 2. 3. or 1) 2) 3), both render as dots I think, and Zero-indexing works fine! 

Normal linebreaks in code (press enter) with up to one space
will wrap fine, which is nice since txt editors often take line 
rendreing seriously (see above. I will clean that up) - this 
sentence takes up four lines in the source code but wraps like normal!

Use double spaces (not double newlines, that'd make new paragraph spacing)  
to ensure these lines stay separate!


### Image: 
Welcome to my Workbench! Just a humble little setup next to my Work-from-home space, 
so that if I need a break I have a productive hobby to jump into. Or at least in theory!

I have a number of old projects (I got really into trying to make bigger and bigger DataLoggers
when I was in Shanghai/Seattle because I didn't have the ability to buy better Battery Testers since we 
were renting from the UW Clean Energy Institute - **NOTHING** motivates me to put in sweat-equity than the
threat of dealing with beaurocracy! (Frankly making a new Battery Tester from scratch is one of my key motivations
of this work! I want to make a DIY tutorial so that EVERY TEST ENGINEER out of school can experience building a battery Test channel from scratch! 

![My workbench, using a cheap but lovely 30V, 30A Power supply to power my brand new $20 Oscilloscope](/_images/2026-10/2026-10-04_WorkBench.jpg){:data-width="200" data-height="66"}
Finally I have a power supply and an Oscilloscope. (Actually what I don't have is a good DC multimeter, it's probably going to be my first goal for a PiPico microcontroller, especially since that and a data-logger are a LONG WAY to the battery testing setup, considering that CCCV charging can be done manually with the power supply and constant-R discharge is easy by definition if all we need to do is cycle! (It can even shut itself off at Vmin if we have diodes in the discharge circuit so that the diode V-Step is the VMin!) 
{:.lead}




[jekyll-docs]: https://jekyllrb.com/docs/home
[fencerdave-gh]:   https://github.com/fencerdave
