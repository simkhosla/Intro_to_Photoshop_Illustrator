# Intro_to_Photoshop_Illustrator
Quick walkthrough basics in Photoshop and Illustrator


###To Begin:
- Download the Adobe Creative Cloud versions of Adobe Photoshop and Illustrator (or any other version you may have).
- 
##PHOTOSHOP BASICS:
###Types of Images:
- Distinguish between the different image types and which type works best for you. 
- Check out the differentimages.html file to get a sense of the difference between PNG and JPEG. 

###Removing Backgrounds (the Photoshop way):
- To remove a background from an image you can either user the Magic Wand tool and do it manually. 
- OR go to Select > Color Range (and choose what color you'd like to select then Delete it). 

### The magic of layers! 
- Layers are awesome and help you work on seperate parts of your image without editing the entire thing
- They can also be used for lots of other fun stuff! (Like GIFs and SVGS -- soon). 

###Making a GIF
- Load up all the images you plan to use for the GIF as individual layers in Photoshop
- Go to Window > Timeline
- When the Timeline panel appears - click on Create Video timeline
- Make sure you click the tiny boxes on the bottom left of the panel, that moves it from a video timeline to animation frames
- Add each layer as an indiviual frame 
- set timing for each layer using the timing dropdown under the image
- set looping options (Once, Three Times, Forever)
- File > Export > Save For Web (Legacy) : here you can set all your final options for the GIF including sizing, number of colors used, etc. 


##ILLUSTRATOR BASICS: 

###Removing Vector Backgrounds (the Illustrator way)
- Pop your image onto the drawing board and select it 
- Go to Object > Image Trace > Make and Expand
- Now your image is a vector / scalable SVG graphic, instead of just a flattened image.
- Export it in whatever format you want -- if you keep it SVG it'll scale responsively in any site.

###Making Layers for SVG Animation
- I've imported an image, made an image trace and seperated it into it's three components in boat.ai
- In there you'll see a Sail layer, a Boat layer, and a Water layer. 
- For every layer that you make in Illustrator, the SVG will generate as a path id -- a seperate entity that you can add ids, classes, and animations to in HTML, CSS and Javascript

###Playing with inline SVGS:
- While an svg imported as an image (<img src = "some.svg"/), acts like a normal image but responsive, embedding an SVG inline in your HTML lets you do a lot more fun things animation wise. 
- Embedding an SVG inline: simply copy the code in your SVG file and place it into the <body> 
- From there, you can see that every individual component has id tags that match your layer names from the Illustrator file.
- Just like any other domElement, these can now be edited using "fill" and other style tags. 
- You can even ANIMATE individual components! 
- REMEMBER: this sort of animation/ styling for the individual components ONLY works if you've embeded the SVG inline! They WILL NOT works if you embed it like so: (<img src = "some.svg"/)


Hopefully that was a fun intro! 
