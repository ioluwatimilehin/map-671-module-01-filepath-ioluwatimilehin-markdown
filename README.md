# Adding Maps to Documents: Markdown Example


The goal of this repository is to show how to add images to Markdown documents. This page that you are reading right now is a markdown document (.md extension).

## MAP 671 Image Process

When you make maps and export these as images, you may want to add these images to a markdown file. For example, maybe you are creating an online project where you need to present and describe a map. Adding that map image in, and additional images showing the overal mapmaking process, can be helpful to communicate with viewers about your mapmaking process and provide sound data documentation that you can refer back to in the future. 

A common question is: "Wait, how did I make that map again?" And now your future self can thank your current self because you'll have kept everything well summarized and presented!

## Filepaths in Markdown

In MAP 671, we tend to use markdown files (README.md - readme is always in all caps for the file name, it's not intended to be shouting at you) and html files. We'll address html files in a future activity.

This document shows some basic formatting you'll use in Markdown while discussing a frequent data hygiene conundrum: where'd it go? You should view this document's source to learn the Markdown syntax used to format the content.

## Types of Markdown Links

To add a link in your Markdown document, add the following syntax to the document:

```markdown
[markdown summary](https://www.markdownguide.org/)
```

The example above would work for creating a link to take the viewer to another page. The example below creates an image link by adding the exclamation point.

```markdown
![markdown summary](https://www.markdownguide.org/)
```

Except I'm using a website url in the link, so a broken link image appears if I actually try this as text in this file.

![markdown summary](https://www.markdownguide.org/)

But if I link to an image from the markdown guide.

```![markdown summary image](https://www.markdownguide.org/assets/images/markdown-mark-white.svg)```

Then it would appear as:

![markdown summary image](https://www.markdownguide.org/assets/images/markdown-mark-white.svg)


## Absolute and Relative Paths

Sometimes when you are adding images you will use an absolute path and sometimes you'll use a relative path.

In the example above with the markdown image, that's an absolute path because that includes the entire url to the image online.

Within a GitHub repository, you can more frequently use a relative path, because files and folders are all contained within that repository.

In case it's helpful, here's a separate description about absolute and relative pathnames.

Imagine if your house was a computer and you needed to get some food to make a sandwich. To make an **absolute path** to the food, you could use:

```txt
/myHouse/kitchen/cupboard04/top-shelf/food.jar
```

Let's say you are already in the kitchen. The **relative path** to the food is: 

```txt
cupboard04/top-shelf/food.jar
```

Now, what if you are in the adjacent living room? The relative path to the food is: 

```txt
../kitchen/cupboard04/top-shelf/food.jar
```
That is, go up to the common area of both the kitchen and living room, the house, and then enter the kitchen. That's what those two .. help describe in the pathname.

## Other Suggestions About Pathnames -  use forward slashes

Github.com uses a Unix-like operating system. Directories are separated by `/` forward slashes. Windows operating system uses `\` backslashes by default, but can use forward slashes `/` too. Always use forward slashes in your directory paths.

### URLs - detailed description

This description of relative and absolute pathname can be applied to including images in a Markdown file. 

What if we want to add a photograph from a website to our Markdown document? Accessing remote assets requires a URL, *Uniform Resource Locator*. 

![anatomy of a URL](graphics/url.png)    
*Anatomy of a URL*


<b>These images are just for my practice:

![Just for practicePhenology](graphics/pic2.jpg)

<i>These are cats with funny looks

![Online_Picture](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRTSLdfwCBPLnRXRg2Ihw0QollE3JeusOVYYw&usqp=CAU.jp)

I have to import another from online<b>

![cat photo](graphics/cat.jpg)

Start with `https` protocol, *Hyper Text Transfer Protocol (Secure)*. If the image is on Flickr.com, we need to add its domain name `staticflickr.com` and any subdomain, e.g., `live`.

```
https://live.staticflickr.com
```

<b> the body <b>
Next, we add the directory path to the image file, making the universally unique address as follows:

```
https://live.staticflickr.com/65535/49373295323_efb53ecfbb_h.jpg
```

The exact URL will be specific to your resource. To embed the image in the Markdown document, add the following syntax to the document:

```markdown
![Alt text for browser](https://live.staticflickr.com/65535/49373295323_efb53ecfbb_h.jpg)
```

![Lexington, Kentucky](https://live.staticflickr.com/65535/49373295323_efb53ecfbb_h.jpg)    
*There it is! A remote image embedded in a Markdown document*

The filepath used is an absolute path. If you had saved the image to an images folder within a repository, you could use a relative path to access the file.

## Application: Add Your Map

One activity to try is to add the map export you created in the previous repository to this readme file. Or you can create your own readme file and then add the image.

* Copy the filepath repository to your local computer
* Go to your map export repository and copy the jpg file
* Go to this repository filepath folder and paste the jpg file. You could paste on the same directory level or you could use an images folder and store the map image within the images folder.
* Open Visual Studio Code and open the filepath repository
* Try adding markdown links to the map image 

You can click the preview button in VS Code to see the image appear in the code editor.

![Module_01](graphics/Module-01.jpeg)

![preview button](graphics/previewbutton.png)

## Summary 

You've learned how to add an image to a markdown file! This is a great skill to have in this course and in future coding too!

## Next Steps

Please continue to the next activity that reviews adding images to html files.
