## Percussion Cartography
### NACIS 2021 - Music, Feelings, and Style session

---

### Land Acknowledgement
<details>
  <summary>Washington, DC is the ancestral territory of the Nacotchtank (Anacostan) and Piscataway peoples.</summary> 
I am writing this from Washington DC, which occupies what was was and still is the ancestral lands of the Nacotchtank (or Anacostan) and Piscataway people. Corn, beans, and squash once grew on Capitol Hill. Pottery has been unearthed on the site of what is now the White House, and burial mounds have been uncovered at Joint Base Anacostia-Bolling. Today there are roughly 4,000 Indiginous citizens of the District of Columbia, representing not only local tribal communities but also ones from all across the Americas. 

To learn more about the Nacotchtank and learn about efforts to gain recognition for the Nacotchtank history of the area, please visit the DC Native History Project at onceasitwasdc.org. 
</details>

---

### HELLO

I love a good personal project, the less useful the better. Measuring sandwiches, <a href="https://vcj.github.io/2020bn/" target="_blank">mapping newspaper football coverage</a>, I am happiest when I am wasting my own time.

The abstract I submitted to the conference has some langauge about invisible maps. That's more or less accurate, but I really just started particular project because I couldn’t go to the studio where I take drum lessons and practice during pre-vaccine days of the pandemic, and I wanted to still make things with music even though I wasn’t really able to make music. This talk...you aren’t going to understand music in a different way or whatever. I just like to take information and make it do things it isn’t designed to do. And music information is extra fun for this, because it can go in so many different ways. 

### What's out there?

Obviously the first thing to do is see what else is out there, what already exists. What I found tended to fit into one of three categories:

1 Maps of Where Music Is: Maps of where to find certain types of music, like this one <a href="https://www.davidrumsey.com/luna/servlet/detail/RUMSEY~8~1~290328~90061892:Standard-School-Broadcast--Pictoria">published by Standard Oil in 1949</a> as part of their weekly educational radio program to promote music appreciation in children.
><img src="images/musicmap1.jpg?raw=true" onclick="window.open('https://raw.githubusercontent.com/vcj/drums/master/images/musicmap1.jpg', '_blank');" />

2 Maps of Music "Networks": Non-geographic maps, like mind maps, that connect artists of similar genres, like the one at music-map.com.
<img src="images/musicweb.JPG?raw=true" onclick="window.open('https://raw.githubusercontent.com/vcj/drums/master/images/musicweb.JPG', '_blank');" />

3 Maps Inspired by Music: Like <a href ="https://cartographicperspectives.org/index.php/journal/article/view/1536">Travis White’s Cartographic Pleasures: Maps Inspired by Joy Division’s Unknown Pleasures Album Art</a>, these maps take inspiration from some aspect of music.
<img src="images/CartoPleasures.png?raw=true" onclick="window.open('https://raw.githubusercontent.com/vcj/drums/master/images/CartoPleasures.png', '_blank');" />

It's sort of difficult to find maps of the music itself. If I had to guess why, I'd say that it's because music is something you hear, and it’s difficult to conceive of something so ephemeral as having a fixed location. You can map the origin, or how it relates to similar sounds, you can apply aspects of it to the physical earth, but what about mapping the sound itself? Maps are typically - not always, of course, please note Harrison Cole's talk later this session - but often visual aids. What do you see, what do you picture, when you listen to, or make, music? How can you visualize the experience of music? How can you map that? 

### Turning Music into Data ("Data")

I started logging music notes as data points during a session of <a href="https://creativecarto.github.io/" target="_blank">Creative Carto</a> last year. I didn't do anything with it, initially, until the 30 Day Map Challenge. The <a href="https://vcj.github.io/" target="_blank">30 Day Map Challenge</a> is an absolutely unmatched opportunity to dive into your folder of halfbaked ideas...just let 'er rip. 

This non-map map just shows  how often each part of the kit is played during a given song - in this case, First Date, by blink-182.

<img src="images/drum-nonmap.jpg?raw=true" onclick="window.open('https://raw.githubusercontent.com/vcj/drums/master/images/drum-nonmap.jpg', '_blank');" />

There is inherent spatiality to drumming. I think there are actually a fair amount of drummers in NACIS! I have done no research on the topic but I’d wager that there’s some solid overlap in cartographers and drummers.

Past NACIS president Anthony Robinson is a drummer, too. This is his kit!

<img src="images/arkit.jpg?raw=true" onclick="window.open('https://raw.githubusercontent.com/vcj/drums/master/images/arkit.jpg', '_blank');" />

I show you this not just to gawk at that incredible giant china cymbal but just because there are a lot of different ways to build a kit. For the purposes of this talk, we’re going to just go with the basics. So, to set the area that we will be mapping. This is the kit in the turquoise practice room at 7DrumCity, the kit I play on most often and the basis for the next few visuals. 

<img src="images/drumkit2.jpg?raw=true" onclick="window.open('https://raw.githubusercontent.com/vcj/drums/master/images/drumkit2.jpg', '_blank');" />

As for the data itself: I worked from written sheet music. If you can read regular sheet music, awesome! Throw it all out, because drum sheet music is different. There isn’t a scale, really. No chords, no octaves, the note placement just refers to the different drums. Like so:  

<img src="images/drumkit2_noted.jpg?raw=true" onclick="window.open('https://raw.githubusercontent.com/vcj/drums/master/images/drumkit2_noted.jpg', '_blank');" />

After some consideration I realized that the best way to make use of my short time with you all, with as little time explaining non-cartography topics as possible was to focus on one piece of classic, widely beloved, well known music with a memorable drum pattern: Kelly Clarkson's Since U Been Gone. 

I started by sketching out the drum kit and assigning coordinates to each drum. Then I went through the written sheet music and tracked whether the drum was struck by the stick in my right or left hand, or right foot in the case of the kick drum pedal. 

### Route Map

And that produced...this.

<img src="images/toplines.png?raw=true" onclick="window.open('https://raw.githubusercontent.com/vcj/drums/master/images/toplines.png', '_blank');" />

Which doesn’t look like a lot of variation, in fact it doesn’t look like much at all, so lets zhush it up a little. 

<img src="images/animated1.gif?raw=true" onclick="window.open('https://raw.githubusercontent.com/vcj/drums/master/images/animated1.gif', '_blank');" />

This is what that looks like animated, with a couple other features as well. Color for the part of the song, and a flashing dot for each bass beat.

### Break for Practical Cartography!!!

This might be something everyone already knows and does all the time but it was new to me and I was just delighted with it. So if this is new to you too, it’s actually pretty  easy to take an existing map and create an animation over it

Take an image in png format - put it into R, there’s a package for that (it's called, as you might expect, png), add a grid (the package for that is...grid), note the x and y coordinates, and use that to plot your animation with ggplot and gganimate. I'm glossing over a lot of a little trial and error in getting the coordinates where you want them, I wouldn’t want to do that for something with too many points, but it’s a neat way of working with cartography you can’t or don’t want to try to do in R. 

For example!!! This is a Pan Am airline map from 1978 with a bit of simple animation. Sure, you could do this in InDesign, but R is free.

<img src="images/panam.gif?raw=true" onclick="window.open('https://raw.githubusercontent.com/vcj/drums/master/images/panam.gif', '_blank');" />

I did not crop out the grid here - in fact, its easier to show you what I did with just a screenshot of RStudio. The file panam9.csv contains the three points that were connected by the geom_line, and the geom_points are the larger dots (being connected by the line). You'll also notice that there is a point at 0,0 and one at 10,10: this stabilized the image as I engaged in the trial and error to place dots on San Francisco, Honolulu, and Sydney. It was much easier once I added those stabilization dots. How many tries did it take before I added the dots? Well....here's a hint, check the csv file name. 

<img src="images/rback.jpg?raw=true" onclick="window.open('https://raw.githubusercontent.com/vcj/drums/master/images/rback.jpg', '_blank');" />

Anyway. This is what my left and right hands are doing when I play Since U Been Gone. It’s a mega-micro route map, showing how I am navigating the setup. If these were real, on-the-ground coordinates we’d need like 7 or 8 decimal places. And sure, there’s no north arrow, but as we all know north is a societal construct. 

A given piece of music, a song, to me, is fairly linear. It has a start, it has an end, there’s a progress of things that happen in between. That stuff in between? That all has, if we don’t want to approach this so literally with a route map, we can take another angle, we can assign everything weight based on frequency, tone, beat… any aspect, really, anything can be visualized. 

Earlier I posed a question about what you see when you hear or make music. I don't know what you see, but for me, there are highs and lows. And I don’t mean emotionally, though there are those too, I mean, say, if there’s a lot of bass drum, that suggests a deeper tone. A lot of hihat, that’s higher in tone. The more I hit a particular drum or cymbal, the bigger that is. If that makes sense. It might not! 

### Welcome to German Terrain Hell

This is a cartography talk, though, so lets talk about cartography. 

<img src="images/cartopl2.jpg?raw=true" onclick="window.open('https://raw.githubusercontent.com/vcj/drums/master/images/cartopl2.jpg', '_blank');" />

Popping back to Travis White’s transect maps for a moment, I’ve always liked this sketch included in Cartographic Perspectives, in particular the elevation transect at the bottom. It conveys a very nice, very clear, line from one end of crater lake to the other. 

<img src="images/germanterrainchaos.jpg?raw=true" onclick="window.open('https://raw.githubusercontent.com/vcj/drums/master/images/germanterrainchaos.jpg', '_blank');" />
 
But sometimes that through line isn’t so nice and clear. Sometimes it’s messy and jumbled and there are a lot of them all working from the same baseline, it can get a little nonsensical. Like this page from the <a href="https://www.davidrumsey.com/luna/servlet/view/search?search=SUBMIT&cat=0&q=pub_list_no%3D%2212189.000%22&dateRangeStart=&dateRangeEnd=&sort=pub_list_no_initialsort%2Cpub_date%2Cpub_list_no%2Cseries_no&QuickSearchA=QuickSearchA">
“Handatlas der Allgemeinen Erdkunde, Laender und Staatenkunde, In achtzig Karten,”</a> or Hand atlas of General Geography, Country and National Studies, in 80 maps, by Georg Leonhart Bauerkeller and Ludwig Ewald, that I found while browsing the David Rumsey Map Collection. And you’ve always got to read the publication notes there, because they cut right to the heart of it.

“Considered by authorities to be one of the most beautiful atlases of the 19th century, it is particularly noteworthy for its quality registration, sharp images, use of brown for relief and solid blue for water, multi-color lithography, and it's scope of content. Particularly noteworthy presentations being: maps, diagrams and illustrations of glaciers in the Alps, an elevation diagram of major mountains and sea depths,a  map of Switzerland with relief depicted with hachures and giving a shaded relief 3-D effect. Most of the text planned to accompany the maps was never completed. 

The atlas was largely ignored by contemporary and subsequent scholars despite its high quality.”

I guess using blue for water had to be noteworthy at some point? This chaotic imaginary landmass of every tall mountain on the earth is great, but let’s take a look at another of the beautiful but ignored elevation diagrams. 

<img src="images/sideview.jpg?raw=true" onclick="window.open('https://raw.githubusercontent.com/vcj/drums/master/images/sideview.jpg', '_blank');" />

Like I was saying about nonsensical - I feel most cross-section style visuals will take you across a single transect, these Germans crammed the entire known planet into one! Trying to describe this...it's like every line of latitude compressed by longitude? I think that's how to describe this?

This is the North American Cartographic Information Society, lets take a closer look at that North American Cartographic Information. 

<img src="images/closer.jpg?raw=true" onclick="window.open('https://raw.githubusercontent.com/vcj/drums/master/images/closer.jpg', '_blank');" />

I was just so taken by the unusual juxtaposition of these features, where the point is not to show you how it is but to show you how it relates to everything else, and I felt a similar approach would serve me well here.

### Brief aside to...explain? 

<img src="images/thorp.jpg?raw=true" onclick="window.open('https://raw.githubusercontent.com/vcj/drums/master/images/thorp.jpg', '_blank');" />

I was putting together this talk at the same time as I was reading Jer Thorp’s book Living in Data. Early on he mentions what he calls “question farming,” which he defines as “using visualization not to simplify something but to unfurl its complexities in interesting ways, exposing things that weren’t before able to be seen.”  Here, you could say I guess I farmed the question “What if Since U Been Gone was a mountain range mapped by those Germans?

### "Mind" "Maps"

Which took me back to R, to get the base lines (pun intended of course, though I think that joke worked better - if at all - said out loud). A little arithmetic gave me the number of hits per drum per section:


<img src="images/dotplot.jpg?raw=true" onclick="window.open('https://raw.githubusercontent.com/vcj/drums/master/images/dotplot.jpg', '_blank');" />

and I used that to make this weird little map!

<img src="images/drums pano.jpg?raw=true" onclick="window.open('https://raw.githubusercontent.com/vcj/drums/master/images/drums pano.jpg', '_blank');" /> 

Here, the height represents the frequency, while the width and general shape represents beat distribution. The color doesn’t mean anything except to separate the parts of the kit, I just like bright colors. I'm not totally sure about this one, sometimes I think it looks really cool and sometimes I think it looks like third rate Tufte. But it’s a fair representation of what going on in my head when I’m playing and listening to the song, a map of the linear progression through the piece with elevation (or depth) assigned by frequency. 

### Rendering with the Frenemy
These are not the only ways I've tried to visualize drum patterns. I'll spare you most of the wrecks, but I do want to share this little friend here.

Made in AerialOD, I was trying to show 3D terrain based on frequency and it looks like I sat on some dixie cups! Reader, I laughed out loud when this rendered. 

<img src="images/mistake.jpg?raw=true" onclick="window.open('https://raw.githubusercontent.com/vcj/drums/master/images/mistake.jpg', '_blank');" /> 


So there you have it, a handful of different ways to make cartography out of percussion! If you have any questions and the conference isn't literally going on right now, feel free to tweet them @hurricanevicky. 

### BYE


---
<p style="font-size:11px">Page template forked from <a href="https://github.com/evanca/quick-portfolio">evanca</a></p>
<!-- Remove above link if you don't want to attibute -->
