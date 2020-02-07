---
sectionid: Uploading Map to GitHub
sectionclass: h1
is-parent: yes
title: Uploading Map to GitHub
number: 6000
---

The information that can be found below is taken from [this presentation](https://maptimela.github.io/map-website/). If you wish to learn more about QGIS and GitHub then feel free to look the presentation over.

For this you are going to need a GitHub account
Once signed in make a repository by clicking the plus sign near your profile and scrolling down to the “New Repository” button. 
This will open up a new page. Set the owner and name the repository. You can add a description if you want, make it public or private if you want, and initialize the repository with a README if you want, the first and the last choice are optional.
You have created a repository.

The next step involves going to QGIS and installing a plugin that will connect it to the web.
Go to the taskbar and click on Plugins then Manage and Install Plugins.
Search for a plugin called qgis2web and install it to QGIS.
This plugin will showup in the Web section of the taskbar. Go to it and find the plugin, clicking on it will bring up a new window.

Export your information, making sure that you indicate a specific place to export it to such as near the other map files on the desktop.
Within your repository you are going to drag the exported file directly onto the webpage.
From there you will go to the settings tab, scroll down to GitHub Pages, select master branch for the Source and choose a theme for the webpage.
Back at the repository create a new file called index.md, this will be your homepage.

Once this is completed, open the index file and click on the pencil icon near the History button.

Add the code below to embed the map within your webpage.: 

**<iframe src="qgis2web/index.html" allowfullscreen="" width="100%"**

From there you can go to the settings and change the theme of the webpage to suit your data.

[The published map should look like this.](https://visualizela.github.io/planningdocs/)
