# Write a Tutorial

**[tutorials] can be created easily**

Each tutorial has an own folder in the `content/tutorials` folder of this repository. You can have a look at the existing tutorials to get an idea how this is done.

## Step by Step Guide

1. Create a new folder for your tutorial. Give this folder a meaningful name (without spaces or special characters in it).
2. Put all the images and files into your tutorial folder.
3. Create an `index.md` file in your tutorial folder. 
    * If you write the tutorial in another language than English, make the two letter language code part of the file name. e.g. `index.fr.md` for French.
    * Write your tutorial in text-editor. The text needs to be formatted in [markdown].
    * Link your files and images in the tutorial.
    * Set the tutorial meta information in the tutorial header
        * `title` the title of your tutorial
        * `preview` the filename of an image in your tutorial folder which is used as a thumbnail image in the [tutorial overview] page.
        * `tags` define some tags that categorize the topic of your tutorial. They will be shown in the tutorial overview as well as in your tutorial.

Here an example `index.md` file

```md
---
title: 'My first Tutorial'
preview: previewImage.jpg
tags:
- MyTag
- AnotherTag
---
# My first Tutorial

Example text...

An embedded image:

![](image.jpg)
```

1. Once you finished editing, you are ready to publish the tutorial. 


[tutorials]: https://qaul.net/tutorials/
[markdown]: https://www.markdownguide.org/getting-started
[tutorial overview]: https://qaul.net/tutorials/
