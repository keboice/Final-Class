#Class 12: Grab Bag/Smorgasbord

## SF Class Notes

Today is our last class!

Hopefully you know how to get started with D3 and some of the idioms used in creating visualizations.

Let's do a brief review of some of the visualizations we've built along the way and share our project progress. Also check out this visualization of [rhyme patterns from the musical 'Hamilton'](http://graphics.wsj.com/hamilton/) along with [notes on how they made it](https://source.opennews.org/en-US/articles/hamilton-algorithm/).

How do you make gifs of visualizations? I use [Licecap](http://www.cockos.com/licecap/) because it's easy, but if you're comfortable with command line tools and want to make high-quality gifs check out [this workflow](http://bl.ocks.org/mbostock/4b88b250bc4439289d94).

##Final Project
#### Motion Chart
D3 Time Series Chart using Mike Bostock's [Wealth and Health of Nations] (https://bost.ocks.org/mike/nations/) chart as a template. Added interface elements - start button and slider. Click on image below to go to chart.
[<img src='motion.gif'>] (http://bl.ocks.org/keboice/raw/037f7ac2089bbe455e86140d24bdefc9/)

#### Dancing Ansombe's
Press buttons to transition the plot
[<img src='anscombes.gif'>](http://bl.ocks.org/keboice/1ad291d2506da8b9418e47d2f96f7a58)

#### Baseball Scatterplot
[<img src=https://cloud.githubusercontent.com/assets/156229/15914266/5d3918b6-2d94-11e6-87b8-ea019597b1e0.png width=500 />](http://bl.ocks.org/syntagmatic/ba23d525f8986cb0ebf30a5dd30c9dd2)

#### Barley Boxplot by Ramesh

[<img src=https://cloud.githubusercontent.com/assets/156229/15921058/9882d512-2dd3-11e6-9532-a9afe70d7de9.png width=500 />](http://bl.ocks.org/sampathweb/98ae33d2c8409234ec8d05f1be76a86f)

#### Dancing Barley Sites
[<img src=https://cloud.githubusercontent.com/assets/156229/15916448/09e06552-2da8-11e6-81c2-05ab6875faf5.gif width=500 />](http://bl.ocks.org/syntagmatic/raw/77b6fae2592e90540c0f01cdbd9b332c/)

#### Extended Barley Yield Small Multiples
[<img src=https://cloud.githubusercontent.com/assets/156229/15488188/c0d6c0f0-2108-11e6-83e8-613d953a0f35.png width=500 />](http://bl.ocks.org/syntagmatic/166e594e16727d9c550ae1eee1f848d4)

#### Chicago Gun Imports
[<img src=https://cloud.githubusercontent.com/assets/156229/15912221/e580bce0-2d87-11e6-8429-b3bcf37fce55.gif width=500 />](http://bl.ocks.org/syntagmatic/5e9a3394a21f5c4656dbed14c300a8f1)

#### Playing with Projections - Science Satellites
[<img src=https://cloud.githubusercontent.com/assets/156229/15728663/be3966ca-2812-11e6-8dc5-f7de24de34fa.gif width=500 />](http://bl.ocks.org/syntagmatic/ae462bc7fea8a2b97bc75196359e8a39)

#### Drought Small Multiples
[<img src=https://cloud.githubusercontent.com/assets/156229/15911919/b2aa35a4-2d86-11e6-9de5-0b39f7c871e8.png width=500 />](http://bl.ocks.org/syntagmatic/d54249c65e15be1612e1cf7d7d02e3f2)

#### Color Cycling Bars
[<img src=https://cloud.githubusercontent.com/assets/156229/15914367/2efbcfd8-2d95-11e6-97c0-d71a1cac5c7d.gif width=500 />](http://bl.ocks.org/syntagmatic/fda03bb0e99febe49fca0fe63f5ca55e)

#### Canvas Drawing with D3 Elastic Easing
[<img src=https://cloud.githubusercontent.com/assets/156229/15914464/f5dd4f6e-2d95-11e6-9451-066d520a9577.gif width=500 />](http://bl.ocks.org/syntagmatic/fe07ddb690ba19887044ae899ba81fd2)

#### Gooey Phyllotaxis with Blur
[<img src=https://cloud.githubusercontent.com/assets/156229/15923986/cb5b6574-2de4-11e6-9485-603faa882e93.gif width=500 />](http://bl.ocks.org/syntagmatic/6a921aed54be2a2bea5e56cf2157768b)


## Kevin's Class Notes

You're never done learning D3, and no class can teach you everything. Here, we'll go over some things many of you have asked about, with a variety of activities to choose from.

Node, Mobile, Fiddly Bits, New Layouts, Live applications?

Let's look at and discuss [another chart](http://www.nytimes.com/interactive/2016/03/01/upshot/super-tuesday-live-republican-delegate-estimates.html?rref=collection%2Fsectioncollection%2Fupshot&action=click&contentCollection=upshot&region=stream&module=stream_unit&version=latest&contentPlacement=2&pgtype=sectionfront) that we'll use today. It touches on many of these things.

<img src='thisguy.png'>

Look at the inspector and find the data this is loading. We're interested in the simpler one, called `republican-sims.json`. [Download it](http://int.nyt.com/newsgraphics/2016-02-20-live-upshot-model/data/out/republican-sims.json) locally.

I got it started for you. Take a look at [example.html](example.html) and download it if you like. Get it running on your machine.

Let's discuss how this works.

We have five goals here that touch on many different aspects.

1. *Node* In real life we don't need to do any preprocessing, but it's easy to see how we might if the file were bigger. Let's use [Node.js](https://nodejs.org/en/) to render out a json file that includes the median, min and max projection for each candidate.

2. *Mobile* Let's get this guy looking good on a phone. What design decisions might we need to make? What technical considerations?

3. *Fiddly bits* Sad but true: the first 90 percent and the last 10 percent usually take the same amount of time. Try to match the design (or improve on it!), customizing colors, borders, axes and labels, adding to the function as necessary.

4. *New layouts* Interactivity can be hard, and possible not worth it, but there are ranges of it that could help. Something like [this](http://bl.ocks.org/ilyabo/1339996) is more or less free. But you could try to implement a [Voronoi layout](http://bl.ocks.org/mbostock/4060366). Lesson for any layout or example: get the demo working locally, remove unnecessary code, then tweak as necessary.

5. *Live applications* One of the only reasons this chart is fun is because it feels live. How might you build this with updates in mind?




What else?
