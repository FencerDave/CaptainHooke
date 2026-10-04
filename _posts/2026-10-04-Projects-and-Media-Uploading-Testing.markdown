---
layout: post
title:  "Examples and Template for Media Uploads"
date:   2026-09-30 07:42:00 -0000
categories: blog
---
# Self-Serving post here, 
I'm new to this so it'll be useful to do my homework once and figure out how to include media of different types in these posts, so this is both an introduction to my world and projects, and a personal How-To guide for using Ruby/Jekyll (And I guess mostly this is me learning HTML..)
Ah, the "HyperText MarkupLanguage..."
To-Do: 
 - [x] Refresh my memory of managing links inside of posts! (And downloads?)
 - [x] Simple Image, alongside narration (learn to format and include along text?)
 - [x] Image Gallery, scroll-through, for showing progress along a project or other many-images without clogging the post
 - [x] Google Slides / Docs / sheets? etc- Apparently easy from File-->Share options as an <iFrame> link
 - [ ] PDFs - Can treat sort of as image, but may want to route through google iframe as per above. (Download links also important! Most browsers will open a download automatically in their preferred way) 
 - [x] Youtube Embedded Player
 - [ ] Embedded StreamLit App - Tools that I make in Python, and want to be able to deploy for the world to use! (Streamlit hosts for free so long as it's a public Repo/project, and I think I can Embed that website in this page/post instead of having to link to the streamlit account page!)
 - [ ] Google Maps Link (With Overlay or Serach-Results, to highlight a location, place, landmark, OR for a future API project-

{% comment %}
Others? Recommendations from Claudius
 - [ ] Github GIST <script src="https://gist.github.com/USERNAME/GIST_ID.js"></script> renders a syntax-highlighted, embeddable code snippet
 - [ ] Math (KaTeX) — Hydejack uses KaTeX to efficiently render math, built in, no setup. Handy for anything electrochemistry-adjacent
 - [ ] Mermaid diagrams — not built in, but one <script src="...mermaid.min.js"> CDN tag plus a <pre class="mermaid"> block gets you flowcharts/sequence diagrams rendered client-side, no image export needed.
 - [ ] Interactive charts (Plotly/Observable) — if you ever want to embed a live data viz rather than a static plot image, a Plotly HTML export or Observable notebook embed both just drop in as iframes/script tags the same way Streamlit does.
{% endcomment %}

## General Formatting
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


## Image: 
Welcome to my Workbench! Just a humble little setup next to my Work-from-home space, 
so that if I need a break I have a productive hobby to jump into. Or at least in theory!

I have a number of old projects (I got really into trying to make bigger and bigger DataLoggers
when I was in Shanghai/Seattle because I didn't have the ability to buy better Battery Testers since we 
were renting from the UW Clean Energy Institute - **NOTHING** motivates me to put in sweat-equity than the
threat of dealing with beaurocracy! (Frankly making a new Battery Tester from scratch is one of my key motivations
of this work! I want to make a DIY tutorial so that EVERY TEST ENGINEER out of school can experience building a battery Test channel from scratch! 

![My workbench, using a cheap but lovely 30V, 30A Power supply to power my brand new $20 Oscilloscope](/assets/2026-10/2026-10-04_WorkBench.jpg){:data-width="400" data-height="150"}
Finally I have a power supply and an Oscilloscope. (Actually what I don't have is a good DC multimeter, it's probably going to be my first goal for a PiPico microcontroller, especially since that and a data-logger are a LONG WAY to the battery testing setup, considering that CCCV charging can be done manually with the power supply and constant-R discharge is easy by definition if all we need to do is cycle! (It can even shut itself off at Vmin if we have diodes in the discharge circuit so that the diode V-Step is the VMin!) 
{:.lead}

## Image Gallery: 
Let's see if this works to make a scroll-able image list for my current hobby of Shuttle Tatting for Lacework!  
The Librarian found me a book on shuttle tatting many months ago (in a littlefreelibrary) and I just recently found a few posts 
that dragged me into the instagram world of tatting and got me to finally get a few shuttles and some cotton/silk thread to try! 

<div class="my-gallery" style="display:flex; gap:0.5rem; overflow-x:auto; padding-bottom:0.5rem;">
  <img src="/assets/2026-10/2026-10-04_Doilie_0-Pattern.jpg" style="height:220px; border-radius:6px;">
  <img src="/assets/2026-10/2026-10-04_Doilie_1-shuttles.jpg" style="height:220px; border-radius:6px;">
  <img src="/assets/2026-10/2026-10-04_Doilie_2_Chain.jpg" style="height:220px; border-radius:6px;">
  <img src="/assets/2026-10/2026-10-04_Doilie_3-HalfRing-ontrain.jpg" style="height:220px; border-radius:6px;">
  <img src="/assets/2026-10/2026-10-04_Doilie_4-FirstRing.jpg" style="height:220px; border-radius:6px;">
</div>


## G-Suite Products Embedded Hosting:
Somewhere I have some Slide Decks that I've given either as talks or as interview panel hosts (I got hired at Form Energy in 2021 
with an educational talk on how to think about Battery Impedance from many different perspectives, why they are all valid but with notes,
and strategies for both experimentally and strategically navigating the trade-off spaces there. 

In any case, Let's share out the group slide presentation for my Pre-Capstone for my UW Masters' Project: "EIS-y as Py" where we trained a Neural network to recognize 
Good vs Bad EIS scans (Electrochemical Impedance Spectroscopy) for a professor who has automated their Electrolyte Experiments and EIS scans. This software feedback
allowed their work to flag what data needed to be Re-Tested the next day in order to have a good quality MetaData. 

<iframe src="https://docs.google.com/presentation/d/e/2PACX-1vRhCAqMEb6vRVEizarrz5AP1rldjxHAnNT565Is4pfaV-KS1ACDj7lrMXm_68MySfpXr3FVUfwZzH38/pubembed?start=false&loop=false&delayms=10000" frameborder="10" width="600" height="400" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>

(I should spend some extra time with google products but that's a note for another time) 

### Youtube Embedded Player: 

Back in the summer of 2021, I taught a 10-week Robotics course over Zoom, using VEX Robotics' [FREE ONLINE ROBOT](https://www.vexrobotics.com/vexcode/vr) tool to teach both Block-based and Pythonic robot controls and basic programming and problem solving principles. The goal, in partnership with HartfordCT Kappa League and MakerspaceCT, was to lay the groundwork for a future In-Person STEM Robotics club based in the Hartford CT area. The Makerspace is still doing amazing work for the local folks and I'm delighted to have been able to help for that summer, and some day I'd love to find or re-create those files (most were lost on a company-owned laptop when I switched jobs!) and actually have an entire educational robotics series on youtube for folks to follow along with. 

In any case, as an example of embedding a youtube video, here I am talking Robotics for the intro course which I did actually pre-record and upload: 

<iframe width="560" height="315" src="https://www.youtube.com/embed/1Tgh-h82SjE?si=HKfZylMKbc2XHBGC" title="YouTube: VexPython Week 1 Intro" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

### StreamLit Apps: 
I've got a few github hosted projects in my history, mostly from when I was between workplaces earlier in my career and wanted to develop Open-Source code for processing battery data, doing very simple modeling of performance, etc. and one personal project I enjoyed a lot was that for my Masters' ChemE Math course, we started with a simple heat balance and progressively made the model more and more and more complex by adding more physics until I had attempted to model parameters that impact the drying of particles inside of a Spray Dryer (An industrial device that sprays liquid microdrops into hot air, so they dry rapidly without damaging the particles and with super high surface area - great for many things especially rehydrating so it's used in powdered drinks all the time!!

Currently everything lives in a [Jupyter Notebook Here](https://github.com/FencerDave/spray_py/blob/master/Modeling%20Heat%20Transfer%20into%20Sprayed%20Droplet.ipynb)
which was my final presentation and focuses on walking through all of the math, and then with examples of what happens if you assume (or obtain) different values for key parameters, etc etc. 
I would LOVE to turn this into a streamlit app to be user friendly (mostly just for fun and as a teaching / learning / portfolio project for myself of course), so eventually that will live here as an example. 





