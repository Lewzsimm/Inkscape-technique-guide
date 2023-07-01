# Inkscape Technique Guide

---

Created by: Lew Fitzsimmons

---

<br>
<br>

> For a proper skills refresher: Read Workflow Tips, and browse through everything in entirety; afterwards return to any techniques as needed, and read thoroughly

<br>
<br>

## TOC

---

[General Working Tips](#general-working-tips)

[Installing New Fonts](#installing-new-fonts-linux)

[Bezier Pen - Tool](#bezier-pen---tool)

[Pen - Tool](#pen---tool)

[Create/Edit Gradients - Tool](#createedit-gradients---tool)

[Create and Edit Meshes - Tool (Super gradient)](#create-and-edit-meshes---tool-super-gradient)

[Draw Caligraphic or Brush Strokes - Tool](#draw-caligraphic-or-brush-strokes---tool)

[Paint Bucket(The Cup of Confusion) - Tool](#paint-bucket---tool-the-cup-of-confusion)

[Tweak Objects by Sculpting or Tracing - Tool](#tweak-objects-by-sculpting-or-tracing---tool)

[Spray Can - Tool](#spray-can)

[Eraser(It's actually a 3-in-1) - Tool](#eraser-tool-its-actually-a-3-in-1)

[Removing Backgrounds To Create Vector Assets](#removing-backgrounds-to-create-vector-assets)

[Align and Distribute](#align-and-distribute)

[Cut one basic geometry shape out of another](#cut-one-basic-geometry-shape-out-of-another)

[Wrap Text Around A Shape](#wrap-text-around-a-shape)

[Shape Stamping](#shape-stamping)

[Toggle Snapping](#toggle-snapping)

[Create Diagram Connectors](#create-diagram-connectors)

[Path Functions](#path-functions)

[Path Effects](#path-effects)

[Create A Repeating Background/Image](#create-a-repeating-backgroundimage)

[Fill text with an image](#how-to-fill-text-with-an-image)

[3D Inner Cut-Out Depth Effect](#3d-inner-cut-out-depth-effect)

[Snowflake-Style Designs](#snowflake-style-designs)

[Mandalas](#mandalas)

[Abstract Mesh Designs](#abstract-mesh-designs)

[Geometric Spirals/Tiled Clones](#geometric-spiralstiled-clones)

[Dispersion Effect: Masking + Clone Trace Spray Tool](#dispersion-effect-masking--clone-trace-spray-tool)

[Photo Trace to Watercolor Art (Technique #1)](#photo-trace-to-watercolor-art-technique-1)

[Photo(clip) to Watercolor Art (Technique #2)](#photoclip-to-watercolor-art-technique-2)

["Halo" an Object](#how-to-halo-an-object)

[Make Designs of Objects Made of Many Smaller Objects](#how-to-make-designs-of-objects-made-of-many-smaller-objects)

[Misty Forest Scene](#make-a-misty-forest-scene)

[Monochromatic landscape art](#monochromatic-landscape-art)

[Turn a picture into text art](#turn-a-picture-into-text-art)

[Bend Text Around A Corner](#bend-text-around-a-corner)

[Basic 3D Text](#basic-3d-text)

[3D Isometric Text (From an angled persprctive with depth)](#3d-isometric-text-from-an-angled-persprctive-with-depth)

[Halftone Patterns with Tiled Clones Tool(Bonus: Image to DPI Effect)](#halftone-patterns-using-the-tiled-clones-tool)

[Shattered Graphic(Broken Glass)](#shattered-graphic)

[Wavy Lines Repeating Pattern](#wavy-lines-repeating-pattern)

[Vector Flowers](#vector-flowers)

<br>
<br>

## General Working Tips

---

* Use **Layers**! Inkscape can be quite "Linux-y" at times and do unexpected things, such as start applying filters to everything on the page rather than just the selected item because some quirk came into being that can't be undone; this can be heavily mitigated by making use of layers, and **Having a layer just for pasting finished and/or imported assets**

* For **Pixel Perfect Designs** set perfect guidlines on to the page with **Extensions > Render > Guides creator**, then when making content, use **Align and Distribute** to position things relative to the page, and/or to eachother, and when creating shapes, manually key in their sizes so that future shapes can easily be made to be exactly 50% of their size etc.

* **Duplicate** base items as you create them, and set them aside within the editor space incase you need to go back to them, then delete them only when you are finished, or better yet save them in their own space if there is any chance you may be asked to revise any part of the project.
This avoids needing to duplicate your entire project just to then Ctrl+Z everything in order to retreive something in a previous state that now has to be changed, and then imported back so you can use it; or having to re-create the asset from scratch

* When Inkscape is not acting intuitively, select your sublect and look across the bottom border of the screen for info; for example, you just might find that what you thought was an object was really a path

* **Punch one Shape out of Another** by individually converting each object into a path with **Path > Object to path**, then overlap them and choose **Path > Difference**

* **Select an Object that is Underneath another Object** by selecting the top object, then pressing the **Tab** key to cycle through them

* Instead of cntl+c cntl+v, we can use **Cntl+D** to quickly duplicate our selection

* Holding **Ctrl+Shift** while resizing a selection will retain it's proportions

* **Stamp Clones of an Object** by grabbing it, and while the mouse key is being held down, pressing **Spacebar** will drop a duplicate beneath wherever the object is

* The shortcut for grouping two selections is **ctrl+G**

* If you have the **Edit Paths By Nodes - Tool** selected and press **Del** rather than deleting the selection, it will be attempting to delete individual nodes, if no nodes are selected then nothing will happen

* On Text, with the cursor between two letters; hold Alt and tap the left or right arrow keys to adjust the "Horizontal Kerning"(gap between letters) between them exclusively, as opposed to adjusting the global setting.

* The **Tweak Objects/Sculpt-Tool** only works after first selecting your targets with the **Select-Tool**!

* **Masking** works like clipping but can be done with gradients etc. It will use the color/lightness of the mask object to determine what it'a going to crop from the photo (A translucent white star used as a mask gets you a star shaped translucent clip, but a black star get's you nothing, likewise a white circle with a black star will leave you with a circular crop that has the star shape cut out of it )

> A Wise Man Once Said: "Path Functions ONLY work on PATHS! Remember this, and you will go far!"

* **Path effects** can only be applied to a single path at a time!

* An **Object to Fill Pattern hack** is that you can select any image/shape that you like and go to **Object > Pattern > Object to Pattern** and it will now become availabe within the submenu of **Fill** as a **Pattern Fill** option: The hidden hack here is a work-around for the fact that you cannot do ***Path Effects to Objects***. We get around it by turning our picture into a pattern, then applying it onto a basic shape, which then **Can** be made to use **Path Effects**!

<br>
<br>

## Installing New Fonts (Linux)

---

> Be sure to check the License rights before using in a commercial project

Inkscape does not require (or offer) any specific way of installing fonts. Essentially, one has to download whatever fonts one would like and place them in the default font directory. Many Linux distributions and other operating systems will allow to install a font by double-clicking on the file, which will then install/copy the font into the correct directory for you.

If your operating system does not offer this comfortable way of installing fonts, these hints may help you:

    * On Linux, fonts can be made available systemwide, to be accessible to core GUI resources such as KDE or GNOME. More commonly, users only install fonts so they can be used by product-making applications including Inkscape and OpenOffice.org.

    * Truetype fonts are installed by placement of the files into the /usr/share/fonts/ttf directory (or C:\WINDOWS\FONTS for Windows types).

> mv ~/downloads/*.ttf /usr/share/fonts/ttf

    * It is advisable that the font cache file be deleted in the process. This file is fonts.cache-1, located in /usr/share/fonts (or C:\WINDOWS\FONTS for Windows types). After font files have been transferred to the default font directory, delete this fonts.cache-1 file and the .fonts.cache-1 file in your home directory (or "My Documents" directory for Windows types).

> rm -f /usr/share/fonts/*fonts.cache-1
> rm -f ~/*fonts.cache-1

* Once done doing this, you need to rebuild your font cache files (only if you are using Linux or some other OS for which font caches are used) so other programs can effectively use the fonts. Do this by going to your default font directory (/usr/share/fonts) and typing as root:

> fc-cache

### Installing without admin rights

On most Linux distributions, there is a directory called .fonts in your home directory. You can install fonts only for yourself by copying them there. This does not require admin rights.

Previously, GNOME's Nautilus file browser had a special location called fonts:/// which could be used to install fonts. After the migration to GVFS, this no longer works, but may be re-added some time in the future.

<br>
<br>

## Bezier Pen - Tool

---

## Mode: Create regular bezier patches

> Modes are sub-types of the selected tool

Note: All bezier actions end with a double-click

* ### Straight line

* Click to set a point, move the mouse to a destination, then double-click and both points will be joined together, forming a line.

By clicking the **Paintbrush>Stroke** style we can change the width and the style of the line.

> Note that holding CTRL(linux) will cause the cursor to snap to the grid, which is how you ensure that the lines are symmetrical

* ### Curved Line

 Click to set a point but keeping the left mouse depressed this time, move the mouse to a destination and then release, then move the cursor to define the curvature, and finally double-click to create the curved line.

If our curves are filled with a color, we need to go back to the fil and stroke menu, select fill, and then choose no paint. Obviously if we want a fill then do the opposite here and choose a fitting fill.

* ### Chaining the straight and/or curved lines

This happens via the single click, weather we were making a straight line or a curve, as long as we do not double click, we can keep making lines using the previous destination as the anchor point, and upon a double click our lines will then be drawn.

For curved lines, expirement with holding down shift or cntrl. Cntrl will lock to the grid, whereas shift will cause only the current line to be morphed(Hard to explain, just test it really fast if you are making curves).

* ### Cleaning up our lines and curves(Edit Paths by Node tool)

Oops! I suck at this! No problem!

Click on the **"edit paths by nodes"** tool to select any of the points that were made with the bezier tool, and manipulate them.

It's sometimes easier to make extra nodes poorly with the intention of coming in afterwards and tweaking everything up to look good.

This tool also gives us access to the bending handle, which is much easier than getting the curves right the first time free hand using only the curved bezier tool.

<br>
<br>

## Removing Backgrounds To Create Vector Assets

---

There are two ways to go about this, first is the use case of removing a white background on a logo(etc) that you would like to make transparent:

* ### Trace Bitmap

Import then select the image, then click **Path>Trace Bitmap**.
The options here can be a little overwhelming, but default will usually get the job done, that being **"single scan, brightness cutoff, brightness threshold 0.450"**.
Click update button in the widget to see a preview, and if the results are not good, it may be possible to get a better result by adjusting the brightness threshold slightly.

> Here this is selecting the Dark areas from the image, but if instead we wanted the light areas to be traced, we click-on the box labelled **Invert Image**

* In the case of colors: go with **"Multiple scans, Colors, Scans = 8"**, confirm that as per default, the boxes for **smooth, stack, and remove background** are checked.

* I have also had good results going with **"Multiple scans > Brightness steps"** as this will make you a black and white which then can be colored with a fill and/or stroke once selected.

> Use to get an asset from a photograph: Doable but largely dependent on the photograph, this will have to be done by feel and experimentation. A good place to start is with the single scan brightness cutoff.

* #### Removing a selected portion of the picture as your asset

Since inkscape doesn't have an eraser tool nor does it have a crop tool, we have to do a workaround using Paths.

* First, use the bezier tool to create a frame for the asset that we want to remove. This could be a square or any other complete shape, including a tracing of the object.

* Once we have our bezier shape, select it, then **Holding Shift**>Select the background image. This is telling inkscape that the first selection, our outline, is the foreground, so do not select these in reverse.

* Next, go to the menu and select **Object>Clip>Set** which will tell inkscape to clip the foreground oblect from the background object, thereby deleting the remainder of the background object in the proccess.

* ### Method #2: Create BSpline Path (For more complicated images)

This is the tool to use for a detailed tracing of an object. Functioning much like the regular bezier tool but with more precision and without the curves, zoom in on the subject and trace it out using as many nodea as required to do so.

A key difference with this tool is that you do not have to do it all in one go as the path can be changed on the fly, or also left half done and returned to after completing other tasks on the same subject by selecting the tool again and clicking on the last node that you left off from.

> If you want to remove a portion of the completed clipping: use the bezier to trace around the area that you want(you can use the original image, then drag it over to the clipping if that is easier), select this and then hold shift and select the clipping, then go to **Path > Intersection**.

> If you want to **Stamp the image OUT of the clipping** go to **Path > Difference**, BUT beware that the outline from the Bezier tool must still be present for this to work, as this is an interaction between paths, not of the new path to be stamped out interacting with the actual image. Applying a Fill is handy here as it will let you see if the Difference took effect as intended or not.

> An example use case here is using Trace Bitmap to extract the shadows from an image, placing an item into the scene that was not previously there, then using gradient to mimic lighting illumination angles on to it, then returning the shadows back on to the top of the image and making them semi-transparent. Now your add-in subject looks like it is natively part of the scene.

<br>
<br>

## Align and Distribute

---

* On the bottom right of the screen(when tools are on the right rather than the top, as is my current setup) **click on the left facing menu arrow > and select align and distribute**.

* From here you can do things such as first select the target object, then select a background object by holding shift, then within the GUI we can see a tab called **Relative to:**____; if we were to choose **'first selected'** then click a related alignment icon, the first object that we selected will be aligned in relation to the second object accordingly.
This is handy when we need perfectly centered objects, among other uses.

* One prominent other use is changing **'Relative To:'** to **'Page'**, now selections can be aligned perfectly relative to the page.

<br>
<br>

## Cut one basic geometry shape out of another

---

To do this you select **Path > Difference**, but note that this is the Path menu, so this will only work for things that are Paths natively. To work on those that are not, they will have to be converted to paths first via **Path > Object to path**, but beware doing this can be a bit janky especially with the cube tool.

<br>
<br>

## Wrap Text Around A Shape

---

In this example I will have used align and distribute to punch the center out of a circle using a smaller centered circle, and have clicked on the Text object and created the word EXAMPLE;

* We will begin by selecting a transparent fill and a black stroke, then making a circle which is going to serve as a guide for the wrapping of our text, but will not actually be part of the logo.

* This is a heck of a lot easier than it seems as inkscape has a built in function for this! Just select your shape and the text, then from the top menu select ***Text > Put on path***.

* This usually results in the text being upside down, but no problem, just select the text by itself, single click it afterwards to get the rotation interface tools to show up, and just rotate it the other way around.

* To get the text on the INSIDE of the circle instead, with the text and circle selected, go to **Object > Flip vertical**

> NOTE: The text is now TIED to that guide circle that we had made!

* Moving the circle effects the text! Why? Because the Text is not taking after the circle, it was instead literally mapped to the same ***Path*** as the circle.
So, once we are done with the circle and don't want to use it to manipulate our text any more, we can select the text and the object that it will be living in/on and group them together by selecting both, then going to **Object > Group**.

This will remove the Text's association with the guide circle as a side effect, and it can now be safely deleted.

<br>
<br>

## Shape Stamping

---

This one is a little odd, but notice that when a shape is selected, in the center of it is a blue crosshair, this is the pivot point.

* If this is placed outside of the shape it will turn red, indicating that the point is now exterior, and if the rotation handles are used the shape will orbit this point in space, rather than spin.  

* While doing this, at any point pressing **Spacebar** will cause the image to stamp out a copy of itself. This can be used to easily create spirals of shapes.

<br>
<br>

## Pen - Tool

---

* Smoothing: Increasing this value will "Clean up" a squiggly-drawn line. Think of a poorly scratched signature being evened out to look elegant.

* Shape: This is describing the total feel of a drawn line as opposed to the head of the pen. For example **Triangle** will cause your line to start off normal and then taper off gradually to a fading point at the end, like a triangle!

* Shape: From clipboard: Yes, that clipboard, as in the one that holds whatever you Ctrl+C. What this does is say we create a shape, we then select the shape and copy it(to the clipboard, naturally); now, when we select **From Clipboard** and draw a line, it will populate our shape across the start and ending points of our line, creating what is essentially a Cntrl+V paste, but conformed to the shape of our line. If the line is long, the shape will be stretched wide, and if we create a U shape, our image will be warped as such.

<br>
<br>

## Draw Caligraphic or Brush Strokes - Tool

---

* Brush types: Dip pen, Marker, Brush, Splotch; these are actually all just presets of various brush settings and not actually differing functions of the Caligraphic Tool.

* Dip pen = Fine yet blocky, Marker = curvy and rounded, Brush = Blocky and wide but with rounded edges, Wiggly = the look of brush blotching, and * Splotch = the look of using excessive ink/paint and letting it pool when the pen is not in motion.

### Value settings

* **Thinning** takes into account the speed at which you make the stroke, think ink pooling in a quill or paintbrush, or the lack there-of.

* **Mass** is the size of the pen or brush

* **Wiggle** introduces a slight squiggle which plays off of stroke speed. At 100%, if you move slowly the pen will create "curly-Qs", but at any setting, moving the pen quickly will result in a straight line.

* **Tremor** Like wiggle, but less loopy and more jagged

* **Caps** Like starting your stroke with the paintbrush rolled onto it's side, then reversing your hand so it also ends on it's side, creating oblong beginning and endings to the stroke at high settings

<br>
<br>

## Create/Edit Gradients - Tool

---

This is for shapes that are already created that you want to add a gradient to after the fact. Manipulate the points to get the desired result.

<br>
<br>

## Create and Edit Meshes - Tool (Super gradient)

---

Imagine you want to create a gradient that conforms to a shape rather than being entirely linear, this is the tool. After selecting our shape and this tool, from the top menu we can select **New:** mesh gradient, or conical gradient, and get mesh points within our shape that we can manipulate to create gradient paths.

We can change the color for any of the points if desired, as well as bend the lines to create warped transitions.

<br>
<br>

## Toggle Snapping

---

This is found in the right-toolbar and when on, if you have an object selected that is like another existing object, for examole a square, it will attempt to snap them together along the grid in an attempt to assist you with alignment. This can be toggled off for more artistic fine placement

<br>
<br>

## Paint Bucket - Tool (The Cup of Confusion)

---

This isn't the paint bucket you are used to, this one is FAR more powerful, but with that great power comes the potential for great confusion.

* First off, it will take on the stroke and fill of whatever the last item that you had selected, so be careful to watch for that.

* This Paint bucket doesn't necessarily do a fill, but it will create a new vector on top of the object you want to fill OF THE FILL that you were asking it to do, using the original as a template rather than changing it.

* To achieve the familiar effect of just a fill, you can leave this over top of the original on a separate layer, or group two objects together.

> But wait, it gets weirder...

* ### It can also trace

By creating a square for example, with transparent fill and a black stroke to play off of, you can use that to inherit, then use Paint Bucket on the item that you want to trace, and what you're left with is the traced image as a vector.

* ### Cut-Out shapes

To illustrate let's say I want to make a cresent moon using Paint Bucket out of two circles. First, I would overlap the circles, then make a square with the fill and stroke that I want the Paint Bucket to inherit, I then click the square and use the paint bucket on the bottom/beneath circle, and Paint Bucket will have made a vector of just the visible portion of the beneath circle, leaving me with a cresent moon of the fill and stroke that I had inherited from the square.

* ### Get a Fill-Copy Cut-out of an image

Choose the correct **Fill by** setting for the item you want a solid-color cut out of.

* If the image is a single solid picture with the background still attached:

Create a white box with no stroke for Paint Bucket to base off of(optional?), choose a White Fill and a Transparent Stroke, then select **Fill by: Saturation** which will fill by grabbing any saturated color, creating a solid white "paper cut-out" copy in the shape of our image.

* If the image is already cut-out/has no background:

Try **Fill by: Saturation** anyways, but if it doesn't work, then try one of the other channels, if all else fails, duplicate the image, stick it onto a black square/background then combine; now paint bucket will be able to distinguish the saturation of the entire image from the background.

> If the image has a halo/stroke to it that you don't want, such as one caused by pixellation, set the **Grow/shrink by:** to Appx. **-2** so that when the fill is done, it leaves behind that part of the perimeter. Also of note, a good starting point for **Threshold:** is **45**.

<br>
<br>

## Tweak Objects by Sculpting or Tracing - Tool

---

* First select whatever object(s) you want to manipulate with the tool (this one lends several of it's features best to many) then choose the tool and a mode for the tool.

The modes's tool-tips are largely self explanatory, and playing with them is probably the best way to go here.

A couple notable features:

* **Blur** is baked into this tool rather than getting It's own dedicated tool.

* **Push Paths Into Any Direction** is the **Sculpting Brush** we are familiar with from photo editing software that let's us warp body parts etc.

<br>
<br>

## Spray Can

---

This shoots out copies of whatever we have selected.

* Want to make artificial stars? Create a single one to use as a template for the Spray Can, then use it to paint the sly of your image.

* This can also be used sort of like how we were stamping shapes earlier. By creating for example a transparent filled triangle, we could then spray paint ourselves a halo of triangles according to whatever the modifiers are set to in the GUI (ex: increasing the with will give us wider triangles than our template, and and increasing the amount will give us more triangles relative to the time the mouse key is depressed)

Again, playing around with the values on this one until it looks right is the best approach

### Spray Copy VS Spray Clone

The difference here is that with spray copy selected the Spray Can will work as expected, however spray **Clone** will actually lock anything the Spray Can makes to the proportions of the object that we had used as a template, so if we change the template object after the fact, ***ALL** of our Spray Can clones will change* accordingly.

This also means that if we are using Clone and want to **Delete the template** we will have to group the sprayed clones together with something else, excluding the template, to break the association before doing so.

<br>
<br>

## Eraser Tool (It's actually a 3-in-1)

---

* **Delete Objects Touched By Eraser:** This paints a thin red line that will delete any objects that it touches

* **Cut Out From Paths and Shapes:** This will erase It's literal path according to the brush size, however when it completely intersects an object, it will break the object into two separate pieces, creating 2 separate objects.

* **Clip From Objects:** This works like the traditional eraser, it will remove anything you paint over(brush size is adjustable)

<br>
<br>

## Create Diagram Connectors

---

Underwhelming, but useful for creating flowcharts etc.

When creating lines with this tool, it will only paint the lines between two different objects; not below or onto them, making it easy to get clean lines that are meant to connect two separate objects.

<br>
<br>

## Path Functions

---

These are all of the main Path functions that are found within the Path menu that interact with two overlapping objects:

* **Union:** Combines the outlines of the shapes to form one new shape

* **Difference:** Cuts out the overlapping object from the base layer, leaving behind the remainder

* **Intersection:** Creates a new object from the part that overlaps, and removes the remainder

* **Division:** Uses the perimeter of the top object as a cutter, and cleaves the base object into two new objects

* **Cut Path** Does the same as **Division** only to the stroke, removing all fill and leaving behind only the split stroke of the base object

* **Combine** This will combine the two objects but punch-out anything that overlaps. This however is tied to an either-or icon option in the upper right of the GUI, where the other option will not punch out the overlapping space but instead will keep it. The difference here as opposed to **Union** in that this will perserve the overlapping stroke lines between the objects, from both layers.

<br>
<br>

## Path Effects

---

Found inside of **Path > Path Effects**

There are a tonne of options here that could constitute their own separate tutorial, but here I will look at

* ### Mirror Symmetry

> This one is super useful and powerful for logo and sprite design:

As usual, playing with the values is probably the best thing to do, but the functinality here is that it will create an attached-mirror-image duplicate of the shape that will mirror exactly any changes made to the nodes on the original, which come with the standard rotation and stretching options.

This is super handy for creating things like logo shields and other non-standard shapes

Note that we can delete individual nodes as well to fundamentally change the result of the shape.

Once satisfied with the design, go to **Path > Union** and it will be transformed into a single standard object.

* ### Knot

This is another good one for making Celtic Knots etc.

* What you want to do here is make two objects that have a stroke but no fill, convert them to paths (**Path > Object to path**) and then overlap them.

When Knot is selected it will create gaps around the parts where the lines are intersecting with eachother.

There is a small circle with a point inside on our object here, this is called the **Switcher** and It's function is to decide which line will be on top/beneath/on the same plane at intersections.

Click on different intersecting points to then use the Switcher to decide how you want the weave to look.

* When finished, you can fix the look here using the **Edit Paths by Nodes-Tool** and stretching the points to fit.

* A good QOL hack here is to select a shape, turn on the stroke to a fixed size, then stretch the paths to touch the stroke, and then remove the stroke afterwards; repeating for each intersection all of our intersection points will be evenly spaced apart. (This is necessary as the default look after using Knot is very square, which is likely not the look that you are going for)

<br>
<br>

## Create A Repeating Background/Image

---

There is a hacky method to making this nice and painless, so go ahead and grab whatever assets you want, or make whatever designs you want and have them ready to go.

1. Create a canvas that is **1000px X 1000px:** This is essential, as it is part of the hack.

2. From the top menu go to **File > Preferences > Behavior > Steps** and set the field **Arrow keys move by:** to 1000px.

3. Create a square that is 1000px X 1000px (exactly the size of our canvas) and set it aside for later.

That's it for the hacking, now we can build the image, and here is the method:

* Whenever an image is outside the bounds of the canvas, it must be duplicated, and the copy must be moved to the opposite side of the canvas, and this is going to happen, and land in exactly the right pixel-perfect position thanks to our hack by one tap of the arrow key, because it was set to 1000px!

* In the case of the image going outside of the canvas in a corner, because this is vertical and horizontal, we will need to do the process twice, once for the horizontal, and again for the vertical.

* Once our image is complete, we can finalize our creation by selecting all objects that are touching the canvas together, and going to **Object > Group**

* Finally, we will take the square that we have set aside, and place it directly over top of our canvas. Here we can use **Align and Distribute** to get it perfectly centered, and then go to **Object > Clip > Set**

* We now have a perfectly aligned tile that when duplicated will interlock perfectly from any side into a seamless repeating pattern.

<br>
<br>

## How to fill text with an image

---

This is much easier than it sounds:

* Make some text, then put it over top of a graphic, then **Object > Clip > Path** and that's it!

* For a bonus, duplicate the text first, and use a copies of the text to make a drop shadow or another backing image, then combine the two.

<br>
<br>

## 3D Inner Cut-Out Depth Effect

---

* Create a shape, save a copy and set that aside

* Now create a duplicate, and uniformly shrink that by appx 5%

* Repeat this until you have several layers; the more you have, the deeper the cut-out will be

* When you have reached the final layer, again create a copy and seit it aside

* Finally, select all and apply a Drop Shadow Filter **Filters > Drop Shadow > Shadow Type > Inner Cutout**

Selecting **Inner cutout** will be key here, and the rest of the options may be tweaked as desired

What we have now is made entirely out of shadows, but say we wanted color:

* Take the first copy that was set aside (the large one) and move it to the bottom of the Z heirarchy so that it is under the shadows, and apply color to it for the new base color.

* Finally, take the last copy that was set aside (small) and place it in the center, and make it darker or lighter than the base color to suit your desired effect.

<br>
<br>

## Snowflake-Style Designs

---

* Bring down a vertical and a horizontal guide somewhere that is not on the canvas(for visibility), and put the cross in the center of the viewport

* We will be doing all of our work in one quarter of the space, then using a filter that is going to essentially multiply it by 4

* Take the **Bezier** tool and create a shape that will represent our "paper" in one of the corners (I use top-left)

* next create some shapes to stamp over top, these will represent holes

* Select all of the "hole" shapes and go to **Path > Union**(Because path effects, which we will be using, only work on a single path at a time, not groups of paths)

* Hold **Shift** and select the "paper" image along with the "holes", then go to **Path > Difference** to create the cut-out-paper effect

* Next, go to **Path > Path Effects > Mirror Symmetry** and notice it is now taking up 2 of the 4 sections

* Go back to the menu again and select **Path > Path Effects > Rotate Copies** and this is going to multiply our image based upon the **Number Of Copies** field (A standard snowflake usually has 6)

* Select the **Edit Paths By Nodes-Tool** and select the node in the center of the image, and pull it down and around until the shape is starting to resemble a snowflake

* Anything done to any of the remaining nodes will be reflected across all sides of the design (For each of the *Number of copies*) tweak the nodes until you're happy with the look

> To add more nodes to an area for added detail, select 2 nodes of which the new nodes are to be added in-between, then in the upper-left of the screen(Or bottom right depending) click the button **Insert new nodes into selected segments** and then click anywhere on the line between our two selected nodes to add another. You can add many nodes here for great detail. Try selecting every-other node down the line then pulling them all outwards uniformly to create "jaggies", and put a bit of blur on the end of them for a melty look

<br>
<br>

## Mandalas

Use the same concepts as described above in Snowflake-Style Designs, except rather than doing the "paper" part, cutting out shapes from it etc.
Just draw the shapes the way you would like them, but then to add another dimension of complexity to them, you can:

* Rotate the image(holding Ctrl for snapping) 90* and repeat the **Path > Path Effects > Mirror Symmetry** step, and then also repeat the **Path > Path Effects > Rotate Copies** step

* Try copy pasting portions of the mandala in combination with resizing for various effects.

> A good way of getting perfectly centered guidelines on the page for this one is to go to **Extensions > Render > Guides creator**

---

<br>
<br>

## Abstract Mesh Designs

---

This will be achieved using **Path Effects** so if we start with an object, it must first be converted.

* Start by making a single vertical line with the **Bezier-Tool**(transparent Fill, colored Stroke), duplicate it, and holding Ctrl move the duplicate to the opposite side of the canvas

* Select both lines and then select **Path > Combine**, and we will now have a base that can work with our coming path effects.

* Next open **Path > Path Effects** and select **Stitch Sub-paths**

* Increase the **Number of paths:** to the desired number of lines, then select the **Edit paths by nodes-tool** to manipulate individual nodes.

* To get an additional "bendy-line-tool" select **Edit on canvas** from the GUI

> This doesn't have to be done with only lines! You can take any shape you want and then do the **Path > Combine** step to make it valid, but you will need at least two objects/lines, a single empty square for example will not work

<br>
<br>

## Geometric Spirals/Tiled Clones

---

Start out by creating a shape and selecting it

* ### Go to **Edit > Clone > Create Tiled Clones**

This will duplicate the shape into a grid either by specifying the number of replicas within each coloumn x each row, or by specifying a length X height value, which will be an either-or selection from within the GUI

This is the default, being the **symmetry** tab with **P1:Simple translation** selected, and is the most basic use case.

* ### To make a repeating Spiral, go to the **Shift** tab

There are many values to toy around with here, but the two that we are mainly here for are **Shift: X** and it's corresponding **Per column** field

* **Per column** is the distance from the original that the clone will be created, so by going to the negative values, we can cause an overlap, as such **-50** will give us a perfect half-way point overlap

* To make an inwards colidescope effect, go to the **Scale** tab, and the fields that we are concerned with here are the **Scale X and Scale Y** values, and the **Per column** fields, as well as the **Apply to tiled clones: Rows, columns** fields.

Here the **scale** is going to adjust the size of the replicas, so by setting the **Per column** fields to a uniform value, we can get a smaller, centered, perfect replica.

If the replica is only slightly smaller **Scale X: -2.00% & Scale Y: -2.00%** and then we go to the **Apply to tiled clones** field and set it to **Rows: 1** but **Columns:__** to a high number, we will get that number of clones, each progressively smaller, one inside of the next, creating a narrowing tube effect.

* To spin it, select the **Rotation** tab and adjust the **Per column** field

> Try a combination of shapes and/or a Bezier shape, then making them all one with **Path > Combine** for some interesting effects

> The **Unclump** button gives them a sort of "stacked paper" look

> The **Blur and Opacity** tab can yield some nice fading effects

> If you are trying to **change the colors but it won't let you**  go to **Edit > Clone > Unlink clones recursively**

> Once **Unlink clones recursively** has been applied, you can then select say, only half of your replicas from the image and then apply a gradient to them, or any combination thereof

<br>
<br>

## Dispersion Effect: Masking + Clone Trace Spray Tool

---

> Make an image break apart into 1000 tiny pieces that are shaped like itself

This effect is where we take a clipping of a photograph (ex. a maple leaf), shrink a clone of it to use with the spray tool, place the image partially over a canvas, create a mask of the part that is covering the canvas, delete that part from the image, then use the spray can in combination with the mask to spray a bunch of clones that take on the colors of the mask we made from the image, giving the illusion of our image breaking apart into a hundred small pieces of itself, then finally using the sculpting and/or blur tools to sweep around the pieces until happy with the look.

> See **Get a Fill-Copy Cut-out of an image** above in the **Paint Bucket-Tool** section for a useful technique that lends itself to this

* Start out by getting a solid-white cut-out of our main object (possibly using the Paint Bucket technique above), set one aside, duplicate it so we have one to shrink down to size for the spray can, and set that aside as well.

* Simplify the Spray can's cut-out: Because we are going to be making a tonne of copies of this one, it would make sense to lighten the load on the hardware by lessening the amount of nodes it has, so with it selected, go to the **Edit paths by nodes-tool**, then choose **Path > Simplify**, and repeat this until the amount of nodes is as small as possible without ruining the look of the shape.

* Lock down the proportions by holding **Ctrl** and shrink down the Spray can's cut-out to the desired size

* Now we select a bunch of default settings for the Spray Can:

Select the spray can's cut-out,select the **Spray can**, and choose the following: **Mode: Spray copies of the initial selection**, **Width: 15**, **Amount: 35**, **Rotation: 50**, **Scale: 25**, **Scatter: 1**, **Focus:1** ; and then for the Eye-Icons, the second **"Apply over no transparent areas"** toggles off the ability for the spray can to apply to anything that is transparent, and since we will be using a cut-out, of which we want to mimic it's shape-over top of a transparent background, **Toggle this to Off**, Next, click the **Prevent overlapping objects** button and start with the Offset at 25%, Next choose the **Eye-dropper icon**, which will make a couple new Icons appear, of which select **Apply Picked color to fill** (Yeesh! Almost Done!), and Finally, within the GUI under the **Trace-tab** click on the checkbox **Trace the drawing under the clones/ sprayed items**.

> What is now happening is that wherever we spray on the cut-out image, the spray tool is sampling the color from that location and because of the Trace drawing under the clones/sprayed items, the spray is appearing beneath our image.

> We placed the image Partially over the canvas so that we could get this effect, without having the spray can paint outside of the shape of the image, and do it in a location where we could later come in and remove only the portion of the image that is covering our spray.

* Next, for more volume and a swept effect, duplicate the sprayed clones, then select the **Tweak/Sculpt-Tool**, start with **Width: 25 , Force: 40** and set the **Mode:** to **Move objects in random directions**, and give them a little nudging

* Now we take care of the Mask:

> The way a Mask works is you make a solid shape, usually a rectangle of sorts, and whatever is under this will be taken into the shape, and the rest deleted; basically like the stamp version of a crop

Create our Mask shape, then place it over top of the part of the image that we want to keep, and go to **Object > Mask > Set mask**

> Note that Mask is **Non-Destructive** which means that if we want to change this again later, we select our "Mask"(the cropped image) and go to **Object > Mask > Release mask** which will return both the original image, as well as the shape used to create the Mask.

* Finally, we want a jagged-portion of cut-outs along the edge of the image that correspond exactly to our sprayed cut outs so that it looks like they are indeed coming from the image.

* Select the portion of sprayed clones that will be overlapping the main image and **Duplicate** them, and set their fill to Green(for consistency as is best practice)

* Do the **Object > Mask > Release mask** to get our full image and Mask shape back, because we are going to cut our spray shapes out of the edge of the mask shape, and then re-apply it.

* Gather up our clones for cutting out of the mask and go to **Path > Union** to combine them

> If we need extra clones here to cover areas of straight line which may be undesirable, we can ungroup the cutting-clones, grab one of them and duplicate it, then drag that over where we want another leaf to appear, and with the mouse; press **Spacebar** to stamp a copy, then re-select them and **Path > Combine**

* Select the Masking shape, hold **Shift** and then select the cutting clones, and go to **Path > Difference** to create the final Masking shape

* Select the Mask, hold **Shift** select the image, and **Object > Mask > Set mask**

* Group the Spray-can clones and positon them, Return the image to the canvas and align it with the clones, and now we have our completed image, ready to be placed into our project!

> For further fine tuning, select some of the clones, and return to the Tweak/Sculpt-Tool, try choosing the **Shrink Objects /or Enlarge-Tool** to create more natural, and/or perspective effects, then further duplicate some clones and experiment with other settings

<br>
<br>

---

## Photo Trace to Watercolor Art (Technique #1)

> This technique extracts the blacks from the photo and procceeds from there, see Technique #2 that begins with a direct clipping

Grab a photo and apply **Path > Trace Bitmap** single scan

* Create a Gradient to color the black parts of our Trace, place that over the parts of the picture that we are keeping and **Object > Clip > Set**

* Select the **Edit Paths by nodes-Tool** and delete any unwanted paths from the image

* create a background color or gradient in a shape to use to clip our image with, drop it to the bottom of the heirarchy, and then **Object > Clip > Set**

> Gotchya Alert: With the select tool selected, in the upper right of it's toolbar is an option labelled **"Move gradients(in fill or stroke) along with objects"** if this is not checked, any applied gradients will not move with the image when you move the image, no matter what you do!

* Next go to **Filters > Textures > Watercolor**

> At any point go to **Filters > Filter editor** and select some of the various effects the filter uses and tweak them

* From here, procceed to make new shapes (or groups of shapes) on to **New Layers**. re-applying and adjusting the Watercolor filter to create what appear to be paint strokes, such as a yellow circle placed in the sky as a sun, or a blue one in water for more depth and color; playing with the Blur and Transparency sliders

> This could be done on a large picture with the intention of later bringing in a clipping box of the desired dimensions and removing snapshots of the scene

> Gotchya #2: After applying a Watercolor filter, you can move around your shape and inkscape will re calculate the effect depending on where you move it much like it tries to change the gradients as explained above, but this time, when you are happy with the look, click the selector tool and resize it by any amount, 0.00001% even, and this will lock the watercolor effect into place, and the shape can then be moved to the desired location in the scene.

<br>
<br>

---

## Photo(clip) to Watercolor Art (Technique #2)

* Create a colored canvas

* Get a photograph with a centerpiece you'd like to use

* Use a Mask (gradient oval shape with blur applied etc) over top of an area of the image you want to capture **Object > Mask > Set**, and place in the center of the canvas

* To create the Watercolor effect, we will make circular shapes and apply **Filter > Textures > Watercolor**, and we can get a GUI to edit the filter by going to **Filter > Filter editor**, where we can select **Turbulence** and this will adjust the look of the splotch's "liquid vs oil" quality (With **Fractal noise** selected as the type, settings of **Base frequency: 0.045, Octaves: 3, Seed: 15** is a good starting point). Next, go to **Displacement Map** and edit the **Scale**.

Once the desired texture of the paint is achieved, **Gaussian blur** is usually a good place to go next if further editing is desired, as the way the Watercolor filter works with Blur, is the lesser the blur setting, the less watercolor effect the filter will apply in turn.

> Note that sometimes Inkscape likes to cut off the bottom of thiis GUI's box, so look for **Effect Parameters** hiding beneath the color bar at the bottom of the screen if it is not visible

* Take a splotch, place it Underneath the focal image, then select the **Eyedropper** from the GUI to match the color to the area that the blotch is in to make it look like it's bleeding out of the picture.

Repeat this until the perimeter looks like watercolor instead of the cut out shape

> If an area is looking too faint and opacity is mot desirable, try duplicating it to double the thickness

* Next, click on the main image and adjust it's brightness and contrast if desired with **Filters > Color > Lightness Contrast**

* A nice final effect here to put lines on top of the image is to use **Path > Trace bitmap** on the original image, then place it over top of the piece.

If **Brightness cutoff** is too harsh, use **Edge detection**

* Now with the tracing selected, in the **Fill and stroke GUI** change the **Blend Mode** to Color dodge, and give it a feel that matches the scene

* Finally, group up the image, then make a clipping shape, and crop it out with **Object > Clip > Set**

<br>
<br>

---

## How To "Halo" an Object

Example = Shapes that resemble the planet Saturn

* Start with a uniform circle, color it white

* Duplicate the circle, change the color to an Orange(this one will be the rings), then hold shift and resize the circle to be roughly the shape of the outer rings

* Duplicate the ringed section, turn it green, and shrink down, forming the hole of the rings by then selecting the orange ring and selecting **Path > Difference**

* Next we will have to divide our main object into two so that one piece can be infront of the halo in the hierarchy and the other can be behind it.
Do this by selecting the **Bezier-Tool** and making a line through the center of the planet

* Now duplicate the Planet, and make the copy Green, then use the heirarchy buttons to drop it **Behind the Bezier line**

* Selecting the green planet and the Bezier line, select **Path > Division**

* The Green part has now been divided in two, and we can remove the bottom half.

* Now with our heirarchy in the order of **Rings < Planet < Green Half-Planet** we should see the effect of the rings wrapping around the planet.

> At this stage the rings should be adjusted to the desired dimensions and position, as the covered portion of them will be removed

* Finally we will clip out everything that is behind the remaining green half by selecting it, and the rings, then selecting **Path > Difference**

We now have a Planet with a Halo Effect!

<br>
<br>

---

## How To Make Designs of Objects Made of Many Smaller Objects

The premise: We will use the spray tool to create a pile of small images, then use a mask representing our large image to select all those that fall within it's bounds, then we will "un-crop" and move any images that got cut off in the process (so it looks like objects and not just a cut-out)

* For this example we will be starting out with the completed planet as demonstrated above in "How To "Halo" an Object":

* Find some images that will constitute the smaller images in the scene, convert them to vectors with **Trace bitmap**, and remove any unneccessary "mess" that may muddy them up when they are shrunk down and multiplied, then use as many **Path > Simplify** passes as possible without comprimising the quality(when shrunk), and set them aside

> For the best starting scale, zoom the viewport to the canvas, and then shrink each of the small images up until the point where if they were any smaller, you wouldn't be able to see detail

* Choose the colors for your objects

* Prepare the **Spray-Tool** by selecting one of the small objects then clicking the spray-tool icon, and from the toolbar, begin with these starting settings:

*Mode: Spray Copies, Width: 1, Amount: 50, Rotation: 50, Scale: 50, Scatter: 50, Focus: 1, "Eyeball Icons": Both toggled On, Everything else: Off*

* Spray a dense pile of objects onto an area, and repeat for each of your small objects, one on top of the other (order and placement does not matter, all we want at this point is density, and volume)

* drag a selection box over the entire pile to select them all and select **Object > Align and Redistribute**.

> It may be a good Idea to move these well above/below the canvas at this stage

What we are interested in here is the **Remove Overlaps** section of the GUI, set it to **H: 1, V: 1** and all of the images will be dispersed across the page, ready for us to select and use chunks

* If not quite satisfied with the object field, select 1/3rds of it and again place one on top of the other, and **Remove Overlaps** again

* To increase the density, select the whole group, Duplicate, and once again, maybe rotate it a bit, and then **Remove Overlaps**

* Take the Planet object, and drag it over-top of an area that you would like to use for the fill, drop the transparency so you can see what you're doing

* We only need the part of the field that has our object, so box-select that area, Duplicate it, and move that to another space to work on

Separate the large object from the small ones, and then group the small ones with **Object > Group**

* Put the Planet object back into position over the newly grouped small objects and **Object > Clip > Set**

At this stage our small objects look like a cut-out, so let's fix the objects on the perimeter to look whole again

* Each object on the perimeter must be selected individually(Double click until it lets you, it's a bit finicky), and then we have to **Right-Click** it, and select **Pop selection out of group**

> Add in/resize/move small objects at this point to get a final look that you are happy with

* Re-group the items once satisfied, and move into position!

<br>
<br>

---

## Make A Misty Forest Scene

* Create what will become a branch by making a branch-ish shape with the **Bezier-Tool** on the regular setting; noting that branches appear linear on top, but jagged on the bottom, as gravity is pulling the branches and leaves downwards(It's going to look like a 5-year old cut it out of a piece of construction paper, this is fine).

* Make a jagged shape the length of the branch to use to clip out the underportion of the branch with, place it over top into position and do **Path > Difference**

* Duplicate that, make the copy a shade or two lighter, then place it ontop, but slightly above the first one to create a layered look, then select **Edit Paths by Node-Tool** and align the points on either end so it looks like one shape and not two.

* Group them, set it aside, duplicate it, reverse the orientation, and set that aside; now we have what will become the left and right branches for our trees

* Using the Bezier-Tool, make a **Thin tree-trunk** and give it a dark fill

* Next, duplicate both the left and right branches and shrink each down to create a Medium-size branch, then do again making a Small-size branch

* Start by selecting a Large branch and using the **Spray-Tool** spray the bottom layer of branches on the corresponding side of tree(from the bottom to appz half way up in a triangular manner), and again with the other side respectively.

> This can be a slight bit messy, so keep in mind that you can always over spray a little then come in and delete individual clones until you have the right shape

Starting settings: *Mode: Spray Objects in a single path, Width: 5, Amount: 10, Rotation: 8, Scale: 30, Scatter: 5, Focus: 0, "Eyeball Icons": Both toggled On, Everything else: Off*

* Repeat for the medium branches, followed by the small branches, working your way to the top of the tree

> When you get to the very top try finishing it with a couple of small branches cloned manually

* Select the finished tree, set it aside; and now we have a whole tree that we can use with the spray can, so make duplicates of 3-4 different sizes(Make some skinner, some fatter as well), facing left and right, and set them aside after grouping them each respectively.

* Use the same spray settings as before, but set **Rotation:** to 0 so the Trees remain straight, and use the large trees to create the foreground for the scene

> Duplicate and strategically place some trees as desired

* Group the foreground trees, then Duplicate and reverse them; now go to **Filters > Color > Simple blend** and set the **Blend mode** to *screen*

Now, choose a color that "grays out" the look a little bit, and we will then lower the heirarchy to make this a middle-background layer, place it in the center of the scene

* Add some fog to the foreground by using **Filter > Textures > Watercolor**, applied to a gray circle, this can be done to taste

> For watercolor tips, see **Photo to watercolor art**

* make another layer of fog and place it on top of the middle layer-grayed out trees

* Use the smallest set of trees to make some final distance trees free-hand, set their opacity to a very low percentage

* From here, tweak up the sky or the background if desired

* Select the entire scene with a bounding box selection duplicate it, group it and move it aside; then create a box in the dimension of the "picture" of our scene that we want to take, perhaps matching the background dimensions, perhaps not, and **Object > Clip > Set**

We now have a final picture of our scene!

<br>
<br>

---

## Monochromatic landscape art

Because everything is a shade of the same color, as long as things are made on small scale, garbage shapes end up looking rather realistic

* Create a background that is some form of gradient of the color we will be using for the project, try and leave a bright spot wherever you envision the sun to be in the scene(this step can always be changed later)

* Create a few shapes that will be the hills (maybe a smaller one for the foreground, large for the middleground, another another smaller for the background?), and apply a gradient of the mono color that the project is using to them, having the tops of them darkest

* create some tiny low-detail trees with the **Bezier-Tool** in the chosen mono color to spray across the top outlines of the hills (all we're after is their tiny silhouettes), use spray tool with a high degree of variance, or do it manually, whatever works for the project

* Group the trees and the hills accordingly, and place into the scene, layered as desired.

* Create a couple of circle shapes, then turn them into white fog with **Filter > Textures > Watercolor** and apply over and in between the layers of the scene

* Add whatever else you like to the scene, bird silhouettes, planes, clouds etc. all will look fine from such a distance

<br>
<br>

---

## Turn a picture into text art

> Upon final review, I would begin this by cutting the subject image into two pieces so that 1. The edges of the picture side can be worked on where the seam is, and 2. so that the entire background is able to be transparent, as this method as stands leaves you with a solid background that you cannot remove afterwards. Consider this before starting

This usually works best with high contrast between the subject and the background, and with a bolder text font to hold more of the image so that here is less empty space in the final product

* Use the **Bezier-Tool** with **BSpline path** selected to cut the subject out of the chosen picture

* Duplicate the image and position it

> Orient/flip your picture so that the portion to show the text is the brighter side, as the text will come out more readable

* create a backdrop square that matches the color of the canvas and move it behind the image in a way that cuts the image in half, and drop it to the bottom of the heirarchy

> Don't use a Stroke on this, though not the end of the world, it will cause you a minor headache in later steps that you will have to fix with **Align and Redistribute**

* Use the **Bezier-Tool, Regular Path** to draw a green mask over the image, into the shape that you want the text to flow, and use **Edit paths by nodes-Tool** to make it slightly larger than your subject, as text tends to have some trailing space

* Next, using the **Text-Tool** with a nicely contrasting color selected, create the text that will be used to flow inside of the image, this can be changed once in position

* Select the Text, then select the Clipping Mask, and go to **Text > Flow into Frame**

* From here, return to the **Text-Tool** and adjust the font sizee and the line spacing until it looks about the way you want it, and further tweak the mask shape with **Edit paths by node-Tool** if desired

> Do not let your text bleed off of the canvas or else when converted to object all of the overflowed text will appear. Instead, finish the last line manually

* *Once you are happy with the look and ready to move forward* select the text and go to **Path > Object to path**

* At this point, the clipping mask can now be safely deleted

* Next, select the subject picture, duplicate it, then drop it down the heirarchy a single step so that it is on top of the original, but underneath the text

* Now select first the text, and then the duplicated image and **Object > Clip > Set**

> At this point you will see nothing but the original image, that is because the text is over top of it perfectly, we will now remove the half of that image that is on the same side as the text to reveal the effect

* Select the rectangle shape we made in an earlier step, and bring it up one step

* Group the final product, and export!

<br>
<br>

---

## Bend Text Around A Corner

> This example will be using the **Create 3D Boxes-Tool** , but the concept can be applied to other shapes

* Make a cube in such a way that you can see 3 of It's faces, and go to **Path > Object to path** to finalize

* Go to **Path > Break apart** to turn the cube into it's individual face-pieces

* select all of the visible faces and move them aside slightly to reveal the other unseen faces of the cube, then Delete these unseen faces as we will not be using them

* Create your text block set up to roughly what youre looking to see bent in half, as well as a text block for the bottom/top/3rd face of the cube

* Because we will be using a Path Effect on our text, for each text block, select and convert to paths with **Path > Object to Path**

* We will use a Path Effect to slice the text in half so we can then attach one half to each of the 2 faces that we will be bending around; select the text then go to **Path > Path Effects**, click the + icon to add an effect, and choose **Slice**

* For each half of our newly sliced text, we need to now go to **Path > Object to path**

* Select the first half of text to apply, along with it's destination face and choose **Extensions > Modify path > Envelope**

> The other half may likely "Quirk-Out" here and try to apply itself in a disoriented manner, to fix this, just Ctrl+Z to undo, and flip the text object horizontally + rotate 90* to the left, and then re-apply it

* Delete the faces of the cube to leave behind only the text

* Select one group of text at a time and go to **Path > Fill and Stroke** to tune up the colors and shades!

<br>
<br>

---

## Basic 3D Text

> There is no 3D text tool, so this has to be done the "Hard Way"

* Make some text without a stroke, using a solid color, then go to **Path > Object to path**, **Object > Ungroup**, and then **Path > Combine**

> Because text is created as an object, but we want individual pathing for each character in our text, and then need those letters to be able to be edited with path effects as a group, we must do the above steps

* Duplicate, and set aside a copy

* Duplicate again and pull off-center into a "3D-Like" position, then reselect the back copy and make it a darker shade, then uniformly shrink it *Very Slightly*

* Select the darker text, and then the foreground, and choose **Extensions > Generate From Path > Interpolate** with *Exponent: 1, Interpolation Steps:60, Interpolation Method: 1, Interpolate style = Checked-On,*

> Here Interpolation steps is the number of iterations or passes this filter will take from the first object in back, to the second object in front. Interpolate in it's most basic form does this between 2 solid lines, so if we were to apply an interpolate of 3 steps to the two lines, it would draw us 3 evenly spaced lines within the 2, leaving us with 5 evenly spaced lines. This can also be applied to other Paths, so by using two letters and many steps, it will make the 3D effect.
> **Interpolate *Style*** equates to the color and texture, so if the behind one is black ant the front one white, we get a depth effect

* Finally take the text that was set aside, and optionally make the shade lighter, then place on top to complete the effect

<br>
<br>

---

## 3D Isometric Text (From an angled persprctive with depth)
>
> This starts off the same way as when creating Basic 3D Text

* Make some text without a stroke, using a solid color, then go to **Path > Object to path**, **Object > Ungroup**, and then **Path > Combine**

> Because text is created as an object, but we want individual pathing for each character in our text, and then need those letters to be able to be edited with path effects as a group, we must do the above steps

* Select **Path > Path Effects > Perspective/Envelope**, and We want *Type: Perspective, with Overflow perspective = Checked-on*

* Now select the **Edit Paths by nodes-Tool** and use the *Diamonds in the corners* to put a perspective onto the text

* Next, choose **Extensions > Generate from path > Motion**

> From here if you just wanted to slap everything together, you could select the background(blocky) parts of the text then go to **Path > Union** to get rid of the little lines, and put the face back on, then call it a day...

* Next, we want to cut the opacity on the top layer of the text and put it into place, then delete any part of the background text that its going to be covering when we are done

* Pull the top layer off again and select the bottom layer of all the text, then apply a gradient to it to simulate the light shining onto it

This will leave you with a basic finished product, and from here it's all about selecting various faces and applying gradients and changing the shades to mimic the effects and/or lighting that you are going for

<br>
<br>

---

## Halftone Patterns using the Tiled Clones Tool

These are grid-like patterns that start out large and then decrease in size relative to an object's opacity values that is chosen as a template.

Generally, a rectangle is created with an gradient applied to it to use as a temporary background, mimicing how we envision the pattern to look as it fades from large to small, and our object is then chosen as the input item for the Tiled Clones tool and placed on top of the rectangle.

* Create your gradient rectangle and your input object for creating the tiled clones

* Select the rectangle and go to **Edit > Clone > Create Tiled Clones** and in the GUI, set **Symmetry: simple transition** and under **Trace** check the *Trace the drawing under the clones/sprayed items* to **On**, and under **Pick from the drawing** select **Opacity**, and for **Apply the value to the clones** toggle *Size* to **On**

* Now select the number of Rows, columns for the tool to create, then drag your cloning object into the upper left corner of the rectangle

* Click the **Create** button you will have your pattern

> If the original cloning object is changed at this point, it will effect all clones, so the entire pattern can be tweaked by selecting it

* From here, the pattern can be combined and/or moved, and the background rectangle can be safely deleted if desired.

> We don't have to use linear gradients and rectangles, any shape and opacity mix will work! Try a circle for a background with a *radial gradient*!

### Do it with hexagons to create a Honeycomb-Fade pattern

This is done the same as before, then duplicating the result, and moving it into place, however we have to make sure that the pattern is spaced correctly for this to work, and we do that with the GUI's **Shift tab**

* For **Shift** we want to have a space that is the same size as our hexagon under each of them, so that our duplicates can lock together uniformly, so we can get that with **Shift Y > Per row: %100.00**(which is saying "give us space equivalent to %100 of our original object"), and then because of the nature of the shape of a Hexagon, it's angles fit together per column at half of it's size, so set **Shift X > Per column: %50.00**. Go ahead and click the Create button

* Duplicate the pattern for a grand total of 4 copies, and then move into position to create the Honeycomb pattern!

> Put a gradient underneath as a background for a cool effect

### Do it with Dots over a Photograph

This results in some pro looking ink print photo-graphics that lend themselves well to adverts

* Use a color photo with a prominent subject that you would like to capture (this will have the same feel as **Trace Bitmap**)

* Create a small object for the cloning object, this could be anything, but let's go with a dot

> **The Gradient object *MUST* be placed on top of the cloning object or this will not work** this is because the effect is based on the gradient object only, and that object is the only object that is selected, meaning it will use whatever is behind it as it's cloning target

* From within the **Trace** tab, the only setting we need to change is **Pick from the drawing** as since we are using an image and not a gradient, we want to select **Color**

* Experiment with **Rows, columns** and hit **Create**

> If you need to use the lighter colors as your base instead of the dark ones, under the **Trace** tab, check **Invert** to *On*, then change your dot to white

You now have a cool DPI effect print of your picture!

<br>
<br>

---

## Shattered Graphic

This is the effect of having your logo look like broken glass

* Take your target image and make it into a **Pattern** using the **Object to Fill Pattern Hack** as seen in *General Working Tips*, then apply it to your target shape as it's fill

> An **Object to Fill Pattern hack** is that you can select any image/shape that you like and go to **Object > Pattern > Object to Pattern** and it will now become availabe within the submenu of **Fill** as a **Pattern Fill** option: The hidden hack here is a work-around for the fact that you cannot do ***Path Effects to Objects***. We get around it by turning our picture into a pattern, then applying it onto a basic shape, which then **Can** be made to use **Path Effects**!

* Create a square that has a transparent Fill and a thin black Stroke, select it and go to **Path > Path effects > Construct grid** and set the **Size X:** and **Size Y:** to something close to double the shard size that you're after (6x6?)

* Select the **Edit paths by nodes-tool** and give the grid a bit of an angled perspective, then *Duplicate the grid* and flip and/or rotate the copy

* Overlap your grids so that they look close to the final shard size that you're after(we will be distorting them after)

> Repeat this step if desired for more randomness and shards

* **Path effects** can only be applied to a single path at a time, so select all of your grids, and go to **Path > Combine** to make them all into one

* Place the "shard grid" over the image in the desired position, select both and go to **Path > Division**

> If you want to get rid of the black lines for a seamless look, just remove the stroke

* You will now have your image looking like someone went at it with a pizza cutter, very unnatural for something broken, so we will fix that with the **Tweak Objects/Sculpt-Tool**:

Select all of the pieces together with the **Select-Tool**, then after selecting the **Sculpt-Tool**, move through various modes to manipulate the pieces.

Generally the only options for **Mode:** that you'll need to use to get the shattered effect are **Rotate objects** and **Move objects**

> Basic starting points: *Width: 10, Force: 30, Fidelity: 30*

* For a final effect, duplicate the final product, apply a black mask along with some blur, and drop it one step below in the heirarchy for a bit of depth!

<br>
<br>

---

## Wavy Lines Repeating Pattern

>Read the section **Repeating Background/Image** for an overview as the same concept will be used here

* Create a perfect square of 1000 x 1000 px to use as the background, and this square cannot have a stroke, or else you will see a grid when it is tiled and used in production

* Next go to **Edit > Preferences > Steps** and set **Arrow keys move by:** to 1000px, which matches our canvas, so we can easily repeat our patterns

* Select the **Bezier Pen-Tool** and make a wavy horizontal line

> The **Spiro Path** Mode works particularly well for this

* Duplicate it, then flip the duplicate upside-down with the **Flip Objects Vertically** button in the toolbar

* Select the *Edit paths by node-Tool** and tweak the result, as well as clean up any stray lines

* Select both of the lines and choose **Extentions > Generate from path > Interpolate**

> Exponent is how close to one side of the two lines the generated lines will be (0.0 = Even), Steps is how many lines will be generated, Method is trivial, and the rest should be left unselected for this effect

* choose a color for your wave (stroke), and optionally add a gradient to it

* Next, select the pattern and go to **Path > Stroke to path** (because it's easier to resize this etc. when it behaves like a path)

* When everything is tiled to your liking, duplicate the background square, select the patterns and the duplicated square that is now on top, go to **Object > Clip > Set**, and you're done!

<br>
<br>

---

## Vector Flowers

* Start by creating a 35 point star, and give it really long points, resembling a characture of the Sun

* Next we apply a **Radial Gradient** from within the **Fill** GUI, and edit it with the **Gradients-Tool** and change it's transitioning color to White, as it is not transparent, and we want a color shift, not a transparency fade-out with our radial gradient; and finally along the **Gradient-Tool**'s editing line, double click at roughly the halfway point to add another color-stop of a complimentry color, and repeat for a total of 3 colors ending with white

> What we want to have is a solid color in the middle, transitioning to the secondary, then ternary lighter colors from the palatte, to white at the ends

> The tips of the star will become the most visible parts of the flower, so if a light flower is not what you are after, just eliminate the white color stop, or replace it

* We now want to use a **Path Effect** and so must change this to a path with **Path > Object to path**

* Select **Extensions > Modify path > Jitter Nodes** and with **Shift Nodes** and **Uniform** selected, play with the **Modify displacement** settings until the star looks "reasonably mangled"

> Maximum displacement **X: 27, Y:16** did the job for this example, but this feature tends to be different whenever used as the shape and scale seem to factor into it's calculations somehow, meaning you'll have to play with it and feel it out

* On to **Tiled Clones**, which we will be using to make 25 clones of this pattern, that become incrimentally smaller, and rotate with some randomness as they decrease in size

* Select the shape and go to **Edit > Clone > Create Tiled Clones**

> The settings for **Create Tiled Clones** are: *Symmetry =  P1:simple translation, Shift = Shift X - Per column: -100, Scale = Per column: Scale X: -5.0, Scale Y: -5.0, Rotation = Angle - Per column: 20, Randomize: 25
> Rows: 1, Columns: 25; The rest = Default

* Once those settings are locked in, hit **Create**, and there's our flower!

> Upon much expirimentation I have found that you can get flowers that look nuch more organic by slightly rounding the tips of the star, and using much less points on the star, creating the bulk through iterations instead

<br>
<br>

---

## Notes On Filters

### Bevels >

> These will be a brief description of the look of ones I have tried followed by a drop-effect after the "--", meaning what they look like when applied to a duplicate of the subject and then dropped behind(NA = proportions remain equal and do not show without alteration of the duplicate's size)

* Bloom: Light coming from the top-left on the diagonal to bottom-right in bars, that wash out whatever it touches to white, with high contrast -- NA

* Brushed Metal: Shiny and finely pixelated rubber, with bright raised midpoints -- NA

* Button: Classic 3D Leather effect with a touch of shine, reminds of a leather car seat, or dash -- NA

* Combined Lighting: Light coming from the top-left on the diagonal, not harsh like Bloom, closer to what you'd expect from an attempt at 3D lighting -- NA

* Dark Glass: Looks more like a raised logo on a new product that's still under protective laminated plastic -- *Adds a plastic-ish drop shadow*

* Deep Colors Plastic: Retro attempt at 3D lighting, finely blotted texture on the light, looks fine from a distance -- NA

* Diffuse Light: This one is a built in editor, good for changing brightness and lighting aspects -- NA

* Electronic Microscopy: Looks like those colored logos with a poured in plastic filling(nice) -- *Adds a slight drop shadow with what might look like slightly raised ridges*

* Fat oil: Like Flux on top of your image after getting hit with the heat -- *A slight wavy, fluxy drop shadow*

* Glowing Metal: Big, hideous 3D lighting texture with a black drop-shadow -- *A nice looking drop shadow with an added 3D texture to it*

* Jigsaw piece: Sort of a flattening, with a matte finish; reminds of how logos tend to appear on pizza boxes -- *A deep Bold-ing effect*

* Matte Bevel: Like 3D lighting only instead of light it's being hit with an airbrush using black paint -- *Generic drop shadow look*

* Matte Jelly: This is another lighting editor but has a bit of a texture to it

* Melted jelly: A low-fi texture with 3D lighting -- *Light, but Lo-fi drop shadow(decent for retention of shape)*

* Melted Jelly Matte: Same as Melted Jelly, but slightly more hi-fi -- *standard light drop shadow*

* Metal Casting: Like someone took Chrome text then tried to print it on a printer from 1987 -- NA

* Molten Metal: Adds a little "toffy-ness" moreso than anything 'molten'. It is quite subtle -- *would be NA if not for the fact that there may be traces of a bump-or-two from the 'molten' effect*

* Neon: As advertized, though more subtle than you'd assume, with a finely ridged-yet pixel-y texture, and a dark drop shadow -- *Standard drop shadow*

* Pressed Steel: Looks like someone turned thick gelatine out of a mould, has a backing ridge to it, looks good but is very heavy -- *Adds ridges, almost a 3D effect, nice*

* Raised border: Does what it says, but also 'nope' because it's washed out and slightly distorted -- *Drop shadow with slight grit*

* Ridged Border: Subtle, internal 3D texture effect, nice-professional -- NA

* Smart Jelly: Melted Jelly Matte but without the drop-shadow -- NA

* Specular Light: Another lighting editor but this one has a slider called 'Azmouth' which is basically mimicing light bouncing off of 3D ridged areas(which of course do not exist aside from this lighting) -- NA

* Stained Glass: Accurate and realistic, but unclean on text as it adds exterior shadowing. Would be best used on images intended for having this applied to it; almost like coloring-book style with the colors pre-done, then the only issue would be the drop shadow on the exterior of the entire image, which then can just be cropped out -- *A flux-y look underneath*

* Translucent: This seems to be stained glass but dusted with a layer of white powder/spray -- *same as stained glass, but grainey*
