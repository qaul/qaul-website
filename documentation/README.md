# qaul.net Web Site Editing & Translating

The [qaul.net] web site is built via the static site generator [HUGO]. Its content and sources are hosted on [github] and are editable.

Your welcome to update and translate this web page.

## Web Site Development Guide

### Install HUGO

[HUGO] can be installed on almost every platform.
Learn how to install it on your computer on [gohugo.io](https://gohugo.io/getting-started/installing#quick-install)

You need HUGO version 0.55 or newer to be able to test and run the web site.
To check your installed version you may run the following command:

```bash
hugo version
```

### Get the Web Site Sources

Clone or download the [github repository] of the web site. All needed files (templates, content, images) are in this repository.

```sh
git clone https://github.com/qaul/qaul-website.git
```

### Run and Test the Web Site locally

```sh
# move into your 
cd qaul-website

# start test server
hugo serve
```

Open the test web site in your web browser [http://localhost:1313](http://localhost:1313). When editing the web sites source files, you will see the changes immediately.

### Trouble Shooting

If you're getting an error without changing anything, check your installed HUGO version (run `hugo version` on the command line). You need at least version 0.55 or later to be able to run and test the web site.

### Edit the Web Site

Here a quick overview of the web sites file structure:

* HTML, CSS & JS Templates
  * qaul.net theme folder contains all the HTML, CSS and javascript templates `themes/hugo-theme-qaul`.
    The only exception is the HTML template of the start page.
  * The HTML template of the start page is in `layouts/index.html`
* Web site content
  * The markdown content files and the images are all residing in the `content` folder.
  * The start page content can be found in the `content/index.md` file and in the `content/home` folder.
    There is a file for each section of the start page.
  * All the tutorials are in sub folders of `content/tutorials`.
    For an explanation on how to write your own tutorial, please read the file [tutorials.md](tutorials.md).

For translating the web site read the file [translate](translate.md).

[qaul.net]: https://qaul.net
[HUGO]: https://gohugo.io/
[github]: https://github.com/qaul/qaul-website
