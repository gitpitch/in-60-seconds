[![GitPitch](https://gitpitch.com/assets/badge.svg)](https://gitpitch.com/gitpitch/in-60-seconds/master?grs=github)

# GitPitch In 60 Seconds

To experience the simplicity and power of the GitPitch markdown
presentation service, follow along with this short tutorial.

> Tutorial also available for [GitLab](https://gitlab.com/gitpitch/in-60-seconds) and [Bitbucket](https://bitbucket.org/gitpitch/in-60-seconds) users.

### Introduction

As a *GitHub* user you are probably familiar with the **README.md** convention.
A convention that automatically turns any **README.md** file found within a
*GitHub* repository into nicely rendered project documentation on *github.com*.

GitPitch introduces a brand new convention for all *GitHub* users, the
**PITCHME.md** convention.

This new convention automatically turns any **PITCHME.md** file found within a *GitHub* repository into a modern, responsive slide deck that is automatically available for sharing and presenting directly on
[gitpitch.com](https://gitpitch.com).

With awareness of this new **PITCHME.md** convention in mind, let's jump
straight into the *GitPitch In 60 Seconds* tutorial.

<br>

### Step 1. Fork this Repository

Create a fork of this repository.

Forking this repository will create a new `in-60-seconds` repository under
your own *GitHub* account. Within your new repository you will find the basic
file structure for a GitPitch slideshow presentation:

```
.
├── PITCHME.md
├── PITCHME.yaml
└── assets
    ├── css
    │   └── PITCHME.css
    └── img
        └── *.png, jpg, gif
```

Only one file is *required* to create a GitPitch slideshow presentation, a
**PITCHME.md** markdown file. This is the file where you add the markdown
content for your slides. Optional files, such as **PITCHME.yaml** and
**PITCHME.css** can be added to activate custom settings and styles for your
slide deck.

Having *forked* this repository you are now ready to move on to step 2. in this
*GitPitch In 60 Seconds* tutorial.

<br>

### Step 2. Congrats on creating your first GitPitch Slideshow Presentation!

Following a *fork* of the repository a **PITCHME.md** markdown file will be
found in your new repository. This means that your first GitPitch slide deck
is immediately available at the following URL:

```
https://gitpitch.com/$USER/in-60-seconds
```

> You must substitute **your** *GitHub* account name for `$USER` in the above slideshow URL.

Using **your** slideshow URL, go ahead and open your new slide deck in the
browser now. When you open your slide deck you should see the first sample
slide that should look a lot like this screenshot:

![TUTORIAL](/doc/assets/gitpitch-in-60-seconds-1.png)

> For comparison purposes, the slideshow URL for the GitPitch In-60-Seconds sample presentation associated with the *gitpitch* GitHub account can be launched [here](https://gitpitch.com/gitpitch/in-60-seconds).

<br>

That's it for the first part of the *GitPitch In 60 Seconds* tutorial. If you
are eager to jump straight back into the *GitPitch Docs*, click [here](https://gitpitch.com/docs/getting-started/tutorial). But if you want to
learn a little more about how the sample presentation for this tutorial was
created - *and that's strongly recommended* - then read on for additional
details and tips.

<br>

### The PITCHME.md Markdown File

Here are some top tips about **PITCHME.md** markdown files that are used to
create GitPitch slide decks:

1. The **PITCHME.md** file name is a new convention introduced by GitPitch
1. The **PITCHME.md** file name is case sensitive
1. The **PITCHME.md** file content is standard GitHub Flavored Markdown
1. The **PITCHME.md** file content also supports [GitPitch Markdown Shortcuts + Widgets](https://gitpitch.com/docs/markdown-features)
1. The `---` markdown fragment acts as a [slide delimiter](https://gitpitch.com/docs/getting-started/delimiters/) that partitions your slideshow content


<br>

### Inside the PITCHME.md Markdown File

The sample **PITCHME.md** within this repository is automatically rendered
as a slide deck with just 5 slides. Each slide introduces important new
concepts while demonstrating the simplicity and power of
*GitHub Flavored Markdown* combined with
[GitPitch Markdown Shortcuts + Widgets](https://gitpitch.com/docs/markdown-features).

The following sections discuss the *markdown* snippets used on each slide
within the sample **PITCHME.md** file in this repository to help you quickly
familiarize yourself with some of the most fundamental and *fun* GitPitch
capabilities.

### Sample Slide #1

Let's jump straight in. The *markdown* snippet for the first slide in the
sample slide deck is shown here:

```

# Let's Get Started

```

This *markdown* snippet renders as follows:

![TUTORIAL](/doc/assets/gitpitch-in-60-seconds-1.png)

As you can see, this slide couldn't be much simpler. The slide uses standard
markdown heading syntax to render text on the slide. The text is automatically
centered on the slide thanks to the default [automatic layout policies](https://gitpitch.com/docs/layout-features/automatic-slideshow-layout/)
for GitPitch slide decks.

### Sample Slide #2

The *markdown* snippet for the second slide in the sample slide deck is shown
here:

```

---

## Add Some Slide Candy

![](assets/img/presentation.png)


```

This *markdown* snippet renders as follows:

![TUTORIAL](/doc/assets/gitpitch-in-60-seconds-2.png)

This sample slide introduces the first use of a [slide delimiter](https://gitpitch.com/docs/getting-started/delimiters/). Slide
delimiters are used to denote the starting point of each new slide in the
deck. This sample slide also demonstrates a mixture of text and image content
being rendered on the slide. Again, only standard markdown syntax is being
used here.

We also see the first use of a relative path to a repository file -
`assets/img/presentation.png` - to *render* the content of that file on the
slide. **PITCHME.md** files can reference source-code, text, image, and
even video files [(pro only)](https://gitpitch.com/docs/pro-features/bonus)
within the repository and see the contents of those files rendered on any
slide. Cool ;)


### Sample Slide #3

The *markdown* snippet for the third slide in the sample slide deck is shown
here:

```

---

@snap[west span-50]
## Customize Slide Content Layout
@snapend

@snap[east span-50]
![](assets/img/presentation.png)
@snapend

```

This *markdown* snippet renders as follows:

![TUTORIAL](/doc/assets/gitpitch-in-60-seconds-3.png)

What just happened? This sample slide introduces one of the most exciting
and unique GitPitch features -
[Snap Layouts](https://gitpitch.com/docs/layout-features/snap-position-layouts).

Most markdown presentation tools and services offer little control
over the layout of content on slides. But GitPitch gives you complete control
over slide-content layout. The same kind of flexibility you may have enjoyed
when working with old fashioned *drag-and-drop* tools like Powerpoint and
Keynote. But now powered by Markdown. The *snap-layouts* feature allows you to
create unique slide designs that fit your specific needs.

If you look carefully at the sample *markdown* snippet for this slide you can
see that the `@snap` tag syntax introduced by *snap-layouts* simply wraps
blocks of standard markdown slide content. It couldn't be easier!


### Sample Slide #4

The *markdown* snippet for the fourth slide in the sample slide deck is shown
here:

```

---?color=#E58537

@snap[north-west]
#### Add a splash of @color[cyan](**color**) and you are ready to start presenting...
@snapend

@snap[west span-55]
@ul[spaced text-white]
- You will be amazed
- What you can achieve
- *With a little imagination...*
- And **GitPitch Markdown**
@ulend
@snapend

@snap[east span-45]
@img[shadow](assets/img/conference.png)
@snapend

```

This *markdown* snippet renders as follows:

![TUTORIAL](/doc/assets/gitpitch-in-60-seconds-4.gif)

I thought it was time we added a little *sparkle* and a splash of color to our
slide deck ;-) This sample slide demonstrates a number of great features. We
have already been introduced above to
[snap layouts](https://gitpitch.com/docs/layout-features/snap-position-layouts)
so we will focus on what's new on this slide.

Let's first look at the slide delimiter for this sample slide, it looks as
follows:

```
---?color=#E58537
```

As noted earlier, slide delimiters are used to denote the starting point of
each new slide in the deck. But they can also be used to activate a whole range
of slide-specific features. In this example, we are using
[color delimiter syntax](https://gitpitch.com/docs/rich-media-features/color-backgrounds/) to
assign a custom background color for our sample slide. This is just the
tip of the iceberg as *delimiters* can be used to render background images,
video, color, gradients, and even
[source-code](https://gitpitch.com/docs/code-features/presenting/) on slides.

Beyond delimiters, this sample slide also demonstrates the use of a hugely
popular GitPitch feature known as
[Markdown Fragments](https://gitpitch.com/docs/markdown-features/fragments/).
Fragments can be used to reveal individual elements on a slide one-by-one. As distinct to revealing all elements on the slide at once. In this case, we are
revealing list items. But fragments can be applied to just about any content
on your slides.

### Sample Slide #5

The *markdown* snippet for this final slide in the sample slide deck is shown
here:

```

---?image=assets/img/presenter.jpg

@snap[north span-100 headline]
## Now It's Your Turn
@snapend

@snap[south span-100 text-06]
[Click here to jump straight into the interactive feature guides in the GitPitch Docs @fa[external-link]](https://gitpitch.com/docs/getting-started/tutorial/)
@snapend

```

This *markdown* snippet renders as follows:

![TUTORIAL](/doc/assets/gitpitch-in-60-seconds-5.png)

The previous sample slide introduced us to the power and flexibility
of slide *delimiters*. This slide demonstrates the use of
[background image delimiter syntax](https://gitpitch.com/docs/image-features/background/) that can be used
to inject an image as a background for any slide. Additional parameters on
this *image* delimiter can be used to position, size, scale, and even control
opacity [(pro only)](https://gitpitch.com/docs/pro-features/bonus) so you can
create the background effects you need.

Again, if you look carefully at the sample *markdown* snippet for this slide
you can see that the `@snap` tag syntax introduced by *snap-layouts* is taking
advantage of a number of
[custom CSS styles](https://gitpitch.com/docs/themes/custom/) - such as
`span-100` and `headline` - to control the appearance of content displayed on
the slide. As a presentation author this features gives you almost unlimited flexibility to create slide decks that truly reflect your product or brand.

<br>

### The Fastest Way from Idea to Presentation.

And that brings us to the end of our whirlwind tour - the
*GitPitch In 60 Seconds* tutorial. If you made it all the way to the end,
congratulations!

While this short tutorial only introduces you to a small number of available
[GitPitch features](https://gitpitch.com/features) we hope what
you have seen so far has made you eager to learn more. Now is your chance to
jump straight back into the interactive GitPitch feature guides
[here](https://gitpitch.com/docs/getting-started/tutorial).
