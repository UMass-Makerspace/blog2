---
layout: post
current: post
cover:  assets/images/photogram/photogram-finished.png
navigation: True
title: The Surprisingly Simple Process of 3D Modeling with Photogrammetry
date: 2020-04-08 05:05:00
tags: [articles]
class: post-template
subclass: 'post tag-articles'
author: tyler
---
## The Surprisingly Simple Process of 3D Modeling with Photogrammetry

Have you ever seen something or someone and thought, “Hey… I’d like to turn this into a 3D model that I can print”. Well think no more, I’m going to tell you how to get started, all you need is a smartphone and a computer. 

I got started using a drone, where images from above can provide quick and highly accurate models of large areas and buildings. But, the concepts are scalable, and a phone camera works just fine for small objects and people. 
![Figure 1: Click on "Try it now" to start the free trial and download the product.](assets/images/photogram/agisoft-screenshot.png)
Anyway, I used Agisoft Metashape to get started. It is a great product with a 30-day free trial and a very quick, easy download which is compatible
with Linux, Mac, and Windows. Give it a Google
search and find the free trial install.

### Choose your Subject
Once you have Metashape installed, it is time to choose your object or person. I have found that people work best for 3D modeling using smartphones because of the texture, size, opacity, and reflectivity of human faces, but the right object can work just as well given the right circumstances. Professional photogrammeters use rigs in order to perfectly capture every angle of an object with a consistently lit surface.
![Figure 2: This is a very professional setup as an example of stationary cameras and stationary subjects.](assets/images/photogram/camera-setup.png)
For the purposes of this post, however, we leave the object or person stationary on the floor (or standing) and rotate the camera around it/them at many different (eyeballed) angles.
![Figure 3: In this setup, a small object remains stationary while the camera rotates around it at set angles, with the same background.](assets/images/photogram/at-home.png)

#### A good subject means that it is:

![](assets/images/photogram/face.png)
-A person: people work really well in amateur photogrammetry processes because of likely bad lighting and the effectiveness of handheld smartphone cameras. This screenshot is my second attempt at a person. I only used about 65 images, and got subpar results, which is much better than it could have gone using so few images and terrible lighting.

![](assets/images/photogram/weird-fuckin-thing.png)
-A larger object with low reflectivity and high opacity. Smaller objects don’t work as well with poor lighting and background because Metashape can’t tell what is the floor or what is the object – in other words, the depth is bad. Photogrammetric software has a lot of trouble understanding why reflective and see-through objects look so different from different angles. This table was the first object I attempted to model, it has a transparent glass top. It came out terrible – like a muffin too big for its container. This is because Metashape couldn’t understand what images belonged where in the model due to the see-through top. 

### Take the Photos

Now that you have your subject, find a wide open area with pretty consistent lightning. So, close windows, turn on overhead lights, and clear an area with about a 3foot radius around your subject, you will need more room than you think. If it’s cloudy outside, then that is perfect.
![Figure 4: Garages are great!](assets/images/photogram/garage.png)
Next take out your smartphone and photograph the subject! For the purpose of this, just have the subject stay stationary and rotate around with your camera. Auto settings are fine. The idea is to photograph 360 degrees around your subject at many different angles. So directly above (90 degrees), then slightly lower at about 65 degrees, then 35 degrees, then 0 degrees. This doesn’t have to be exact; the models will likely look like a first try. Try to get a decent amount of overlap as you rotate around the subject, but about 50 photos is plenty for your first model. 

### Upload and Process in Metashape

The hard part is over! Next, import your photos to Metashape as indicated in the figure below.
![](assets/images/photogram/metashape.png)
The rest of the process is very simple, but it does take time. Basically it will all be done in the workflow tab: 
![](assets/images/photogram/selection.png)

Select them, and apply the processes in descending order. So, align the photos, then build dense cloud, then mesh, then texture. Each process will make the model look more and more like the real thing. Note: you must continuously crop during each step. You can do this very easily by using the crop tool: 
After you select points and areas which will be of the room you are modeling in, click the X two spaces the the right of the crop tool. This will delete the selected points. Alternatively, select the parts you want to keep and click the “crop selected” button three to the right of the crop tool in order to delete everything other than the selected. If you crop nothing, you will get something like this: 
![](assets/images/photogram/photogram-finished.png)
After each step, you can view progress by selecting “point cloud”, “dense cloud”, and “texture/mesh” views: 
![](assets/images/photogram/textures.png)

Another note: To hide the weird blue squares (which actually indicate where the picture was take and what angle relative to the subject), grid, and trackball, simply click Model 🡪 Show/hide items and then click whatever you don’t want to see anymore. 
![](assets/images/photogram/fix.png)
Default settings will be fine for this, with medium accuracy all around the board for quicker processing times. If you want a really crisp model, then increase the accuracy levels and it is very important to increase tie point limit and key tie point limit under advanced settings during the align photos phase (around 80,000+ and 10,000+ respectively).

So, if you are still with me, you should be able to make a pretty good 3D model! If you try, and the photos don’t align (I usually look for about 80% of photos to align) or the model comes out terrible, it unfortunately is likely due to poor photos. There is no solution around that other than retake the photos in a different space with potentially a different object. But, that is the best way to learn what works and what doesn’t! 

If you so desire, these files can be exported and done with as you please. In the coming weeks, a new blog post and workshop will be posted on how to 3D print these files. So we can essentially 3D print a human. The week after that will be giving it artificial intelligence, then you can have your very own UMass makerspace clone!
![](assets/images/photogram/spiderman-pointing.png)
