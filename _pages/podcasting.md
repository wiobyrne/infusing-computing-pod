---
layout: page
title: "Podcasting With Jekyll"
permalink: /podcast
---

This site is built using the static site generator [Jekyll](https://jekyllrb.com/), the audio files live on the [Internet Archive](https://archive.org/details/infusingcomputing/) and the site itself is hosted on [GitHub pages](https://pages.github.com/).

### What is this?

This webseries is meant to provide an alternative to webinars to disseminate information from the [Infusing Computing research project](https://www.infusingcomputing.com/). We wanted a platform that was a bit more open, accessible, and approachable with people in and out of the project. We figured that webinars would only be reviewed by project participants..and have the potential to be ignored. A podcast series provides bite-sized (around 10 minute) segments that can be consumed by individuals during the everyday events of their lives.

Podcasting relies on a pretty simple technology - RSS. RSS often gets generated for a website almost as a by-product of adding content, this allows people to "subscribe" to your website and be notified or fed updates. Jekyll generates RSS straight out of the box and every podcast needs a website so we thought - why not kill two birds with one stone?

### How do you do this?

After a bit of research, we realized that the platform we use to host the website (Weebly) is horrible for creating a podcast feed. WordPress would provide a much better option. This is partially due to a decision to host the [audio files for the podcast](https://archive.org/details/infusingcomputing/) on the Internet Archive. This allows the files to be hosted for free. This also allows us to Creative Commons license the audio files and make them available for others to review, remix, reuse. Lastly, it is important that the materials, tools, and process are all transparent to show others how this may be accomplished. 

After realizing that Weebly would not work, and starting up a new WordPress instance would not be an option, we researched the [Podcast Generator](http://www.podcastgenerator.net/) which worked for [Doug Belshaw](https://dougbelshaw.com/) and [Dai Barnes](http://daibarnes.info/) on the [TIDE podcast](http://tidepodcast.org/). After some epxloration, we could not get this running and looked for other opportunities to serve the podcast website, while not being solely "owned" by one person. 

After more research and exploration, we identified the potential to use [Jekyll](https://jekyllrb.com/) and [GitHub Pages](https://pages.github.com/) to create individual posts for each episode and power the RSS feed for subscriptions. This inspiration is all due to [Tim Klapdor](https://timklapdor.com/). This site was inspired by Tim's use of the [Jekyll Skeleton](https://github.com/timklapdor/jekyll-skeleton) to create the [LinkRot Podcast](https://github.com/timklapdor/link-rot). We also liked the embedded HTML5 player ([Plyr](https://github.com/Selz/plyr)) in the post page for each podcast to allow people to sample and listen without having to subscribe or download anything. This was an element used in the LinkRot Podcast.

Jekyll is a static site generator that can be used to create simple blogs from plain text files. [GitHub](https://github.com/) is a cloud [Git](https://git-scm.com/) repository hosting service that provides a handy web interface for managing, editing, and collaborating on Git repositories. By using Jekyll to create pages and share via GitHub, GitHub Pages allows us to share a website using free static web hosting from a GitHub repository. To learn about Jekyll, GitHub, and GitHub pages, [this workshop](https://evanwill.github.io/go-go-ghpages/) from [Evan Will](https://evanwill.github.io/) was an invaluable resource. Screencast of the workshop is available [here](https://www.youtube.com/watch?v=SWVjQsvQocA&feature=youtu.be).

We used the repositories from the Jekyll Skeleton and LinkRot Podcast to create this website.  

This project will most likely include a constant amount of fiddling and tweaks to keep it running, while making it look better online. Once again, one of the key goals is to show what can be done to create this alternative publishing and dissemination model in professional development experiences. 

### Our Process

**1.** Record the conversation using Zoom

**2.** Edit and export audio from Zoom. Edit audio in [Audacity](https://www.audacityteam.org/) or [Soundtrap](https://www.soundtrap.com/)

**3.** Edit metadata

**4.** Upload file to the Internet Archive file - copy link to MP3

**5.** Create a new post in Markdown and add in the relevant front matter to the YAML section. The following guidance is from the LinkRot podcast

``` yaml
layout: post
title: "Title Goes Here"
date: Publishing date and time
file: link to file in S3
summary: "Quick exerpt of episode"
description: "Longer information"
duration: "how long in minutes and seconds" 
length: "in seconds"
explicit: "do we swear" 
keywords: "keyword tags"
block: "hold back publishing it" 
voices: "who did the talking"
```

**6.** Add links and show notes to the content section. 

**7.** Once we're complete Commit to GitHub

**8.** Site and RSS is updated and the new episode is pushed out
