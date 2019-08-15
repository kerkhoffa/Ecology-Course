# Ecology - Semester Course

[![DOI](https://zenodo.org/badge/31911336.svg)](https://zenodo.org/badge/latestdoi/31911336)

This is a set of course materials for an Ecology course (BIOL 228) at Kenyon College. The course page was built from Ethan White et al.'s [forkable](https://help.github.com/articles/fork-a-repo/) set of teaching materials for teaching biologists how to work with data through programming, database management and computing more generally. Go there to get started on your own course!

The first attempt at using this course page is in the fall of 2019. We will see how it goes.

## Below is material from the README of the original course.



- Here are some other examples of customized courses forked from Ethan White's course:
  - [Introduction to Ecology](https://atredennick.github.io/ecology_class/) by [Andrew Tredennick](https://atredennick.github.io/)
  - [Data Science for Agriculture](https://palderman.github.io/DataSciAg/) by [Phillip Alderman](http://pss.okstate.edu/pass-drctry/faculty/alderman)


## Where is everything

Core teaching materials are stored in `exercises/`, `lectures/`, and 
`materials/`.

Class specific materials are stored in the `syllabus`, `schedule` and `assignments/`.

Most of the other folders and files support creating the course website using
[Jekyll](http://jekyllrb.com/).

## Using Jekyll to build your own course website

### Simple setup

The website is setup to be easy to run automatically through GitHub:

1. [Fork](https://github.com/datacarpentry/semester-biology#fork-destination-box)
   or [import](https://import.github.com/) the repository to 
   `https://github.com/yourusername/semester-biology`.
2. Update `# Setup` information in `_config.yml` in the main directory for
   proper site rendering.
   * You must `push` this change to your repository to build and browse your 
     forked version.
   * In a few minutes you should be able to see the site at:
     `https://yourusername.github.io/semester-biology/`
3. Edit any of the markdown (.md) files
4. Commit and push the changes
   * The changes should now be reflected on the website
5. If you want to use a custom domain name instead of `github.io`, follow
   [GitHub's instructions for setting up a custom domain](https://help.github.com/articles/setting-up-a-custom-domain-with-github-pages/).

If you have any problems please
[let us know](https://github.com/datacarpentry/semester-biology/issues/new) and
we'll be happy to help.

### Previewing changes locally

If you want to view your changes locally, before pushing them to the live
website, you'll need to setup Jekyll locally. GitHub provides a [good
introduction on how to do this](https://help.github.com/articles/using-jekyll-with-pages/).

If you have Jekyll properly installed, you can then run

`bundle exec jekyll serve --baseurl ''`

from the command line and navigate to http://localhost:4000/ in your browser to
preview the current state of the website.


## Creating new pages

If you want to add new exercises, lecture notes, etc. you do this by creating a
[markdown file](http://daringfireball.net/projects/markdown/basics) in the
appropriate directory. Each markdown file needs to start with some information
that tells Jekyll what the page is. This is done using something called YAML,
and the standard YAML for a new exercise would look like this:

```
---
layout: exercise
topic: Topic group of exercise
title: Name of exercise
language: [R, Python, SQL]
---
```

This is placed at the very beginning of the markdown file and provides
information on what kind of content it is (e.g., exercise, page, etc.),
the title of the page, and what language it applies to.

The page should then be available at a url based on where the file is located
and what the file name is. So if you created a new exercise in the `exercises/`
folder called `my_awesome_exercise.md` it would be located at:

Locally: `http://localhost:4000/exercises/my_awesome_exercise`

After pushing to GitHub:
`https://yourusername.github.io/semester-biology/exercises/my_awesome_exercise`


## Acknowledgements

Development of this material is funded by [the Gordon and Betty Moore
Foundation's Data-Driven Discovery
Initiative](http://www.moore.org/programs/science/data-driven-discovery) through
[Grant GBMF4563](http://www.moore.org/grants/list/GBMF4563) to Ethan White and
the [National Science Foundation](http://nsf.gov/) as part of a [CAREER award to
Ethan White](http://nsf.gov/awardsearch/showAward.do?AwardNumber=0953694).
