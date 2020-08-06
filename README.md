# Michael Wiertlewski's Lab 

The website uses Jekyll and Github pages to provide custom content. You can download the structure and play with it as you'd like.
The pages, project and publications can directly be added to Github by navigating to the relevant folder and then creating a `New file` with the right structure (see below) and the right filename. Once the file is saved it will automatically update the repository and the website (it might take few minutes).

The pages are formatted using the super easy Markdown language. A useful cheatsheet showing what can be done with Markdown can be found [here](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).

## Add personal page

You can add a description of your research interest and CV in the `_people` folder. The filename should be the `<firstname>_<lastname>.md`. The header provides the informations that are used throughout the website and should be completed first.

```
---
name: Michaël Wiertlewski
position: pi
avatar: michael-wiertlewski.jpg
gscholar: https://scholar.google.com/citations?user=7-gxrtEAAAAJ
email: m.wiertlewski@tudelft.nl
linkedin: https://www.linkedin.com/in/michaël-wiertlewski-68300221/
researchgate: https://www.researchgate.net/profile/Michael_Wiertlewski
cv: cv-wiertlewski.pdf
address:
  - Department of Cognitive Robotics
  - Room F-2-360
  - Mekelweg 2
  - 2628 CD Delft, The Netherlands
---
```

Pictures live in the `images/people/` folder, the cv in the `pdf/cv/` folder and you can choose your position from 4 categories `postdoc`, `phdstudent`,`master`, `visiting`, `others`.
For a proper rendering, the image should be 1x1 aspect ratio with less than 400px wide.

## Add publications

Right now each publication is an independent post. To add a publication, create a file in the `_posts/` folder with the filename `YYYY-MM-DD-title.md`.  Each file should have a header in the like of:

```
---
title: Sensing the Frictional State of a Robotic Skin via Subtractive Color Mixing
categories: publications
authors: X. Lin, M. Wiertlewski
journal: IEEE Robotics and Automation Letters
pages: "4(3):2386 - 2392"
year: 2019
urlpaper: https://ieeexplore.ieee.org/document/8613793/
pdf: pdf/pub/2019-XL-MW-RAL.pdf
note: Best paper award at ICRA's workshop on Soft Haptics
image: images/pub/IMG_0172.jpeg
---
```

The categories tag should be left to `publications`. A poster image should be provided and put in `images/pub/`. A author's copy of the manuscript can be placed in `pdf/pub/`

## Add project

The project pages follow the same structures that the publications. To add a new project, create a page in the `_posts` folder with the filename `YYYY-MM-DD-title.md` including the following frontmatter:

```
---
categories: research
title: Interaction Design
subtitle: We study how to create compelling sensations using surface haptics
image: interaction.jpg
---
```

A description with possibly more pictures / video should follow the frontmatter. Markdown is also the formatting language of choice.

## Add news

Short news (one line) are display on the frontpage. You can add your own news by directly editing the file `data/news.yml`. Each news item has a date and a description tag. Markdown formatting can be used for providing external links or emphasis to the content.

## Acknowledgements

The structure of the website is made with Jekyll and heavily influenced by the [Kording lab page](http://kordinglab.com/) with a twist of [Bootstrap](https://getbootstrap.com/).
