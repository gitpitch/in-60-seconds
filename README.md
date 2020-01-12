[![GitPitch](https://gitpitch.com/assets/badge.svg)](https://gitpitch.com/gitpitch/in-60-seconds/master?grs=github)

# GitPitch In 60 Seconds

To experience the simplicity and power of the GitPitch markdown
presentation service, follow along with this short tutorial.

> Tutorial also available for [GitLab](https://gitlab.com/gitpitch/in-60-seconds) and [Bitbucket](https://bitbucket.org/gitpitch/in-60-seconds) users.

### Introduction

The recommended and best way to create, preview, and
present a GitPitch markdown presentation is to use
[GitPitch Desktop](https://gitpitch.com/docs/pro-features/desktop). But for an
almost instant introduction to GitPitch without needing to download anything
we can work directly within a respository on Git. And that's what we'll do 
right here.

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

### Step 2. Congrats on creating your first GitPitch Markdown Presentation!

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
are eager to jump straight back into the *GitPitch Docs* so you can download
**GitPitch Desktop**, click
[here](https://gitpitch.com/docs/getting-started/tutorial). But if you want to
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
1. The **PITCHME.md** file content also supports [GitPitch Markdown Widgets](https://gitpitch.com/docs/markdown-features/widgets)
1. The `---` markdown fragment acts as a [slide delimiter](https://gitpitch.com/docs/getting-started/delimiters/) that partitions your slideshow content


<br>

### Inside the PITCHME.md Markdown File

The sample **PITCHME.md** within this repository is automatically rendered
as a slide deck with just 6 slides. Each slide introduces important new
concepts while demonstrating the simplicity and power of
*GitHub Flavored Markdown* combined with
[GitPitch Markdown Widgets](https://gitpitch.com/docs/markdown-features/widgets).

The following sections discuss the *markdown* snippets used on each slide
within the sample **PITCHME.md** file in this repository to help you quickly
familiarize yourself with some of the most fundamental and *fun* GitPitch
capabilities.

### Sample Slide #1

Let's jump straight in. The *markdown* snippet for the first slide in the
sample slide deck is shown here:

```

# Let's Get **Started**

```

This *markdown* snippet renders as follows:

![TUTORIAL](/doc/assets/gitpitch-in-60-seconds-1.png)

As you can see, this slide couldn't be much simpler. The slide uses standard
markdown heading syntax to render text on the slide. The text is automatically
centered on the slide thanks to the default [automatic layout policies](https://gitpitch.com/docs/layout-features/automatic-layout/)
for GitPitch slide decks. It's also worth nothing that emphasized text, such
as bold and italics, can be automatically rendered by your 
[custom theme](https://gitpitch.com/docs/themes/default) to use a distinct
color for additional emphasis on any word or phrase. Nice!

### Sample Slide #2

The *markdown* snippet for the second slide in the sample slide deck is shown
here:

```

---

### Add Some Slide Candy

![IMAGE](assets/img/presentation.png)


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
even video files [(pro only)](https://gitpitch.com/docs/pro-features/power)
within the repository and see the contents of those files rendered on any
slide. Cool ;)


### Sample Slide #3

The *markdown* snippet for the third slide in the sample slide deck is shown
here:

```

---?color=linear-gradient(180deg, white 75%, black 25%)

@snap[west span-55]
## Customize the Layout
@snapend

@snap[north-east span-45]
![IMAGE](assets/img/presentation.png)
@snapend

@snap[south span-100]
Snap Layouts let you create custom slide designs directly within your markdown.
@snapend

```

This *markdown* snippet renders as follows:

![TUTORIAL](/doc/assets/gitpitch-in-60-seconds-3.png)

What just happened? This sample slide introduces one of the most exciting
and unique GitPitch features -
[Snap Layouts](https://gitpitch.com/docs/layout-features/snap-layouts).

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

---

@snap[north-west span-50 text-center]
#### Engage your Audience
@snapend

@snap[west span-55]
@ul[list-spaced-bullets text-09]
- You will be amazed
- What you can achieve
- With a **little imagination**
- And GitPitch Markdown
@ulend
@snapend

@snap[east span-45]
![IMAGE](assets/img/conference.png)
@snapend

@snap[south span-100 bg-black fragment]
@img[shadow](assets/img/conference.png)
@snapend

```

This *markdown* snippet renders as follows:

![TUTORIAL](/doc/assets/gitpitch-in-60-seconds.gif)

I thought it was time we added a little *interaction* to our
slide deck ;-) This sample slide demonstrates a number of great features. We
have already been introduced above to
[snap layouts](https://gitpitch.com/docs/layout-features/snap-layouts)
so we will focus on what's new on this slide.

This sample slide also demonstrates the use of a hugely popular GitPitch feature
known as [Markdown Fragments](https://gitpitch.com/docs/markdown-features/fragments/).
Fragments can be used to reveal individual elements on a slide one-by-one. As distinct
to revealing all elements on the slide at once. In this case, we are
revealing list items. But fragments can be applied to just about any content
on your slides. As we can see with the reveal of the final large image on the slide.

### Sample Slide #5

The *markdown* snippet for the fifth slide in the sample slide deck is shown
here:

```

---

@snap[north-east span-100 text-pink text-06]
Let your code do the talking!
@snapend

    ```sql zoom-18
    CREATE TABLE "topic" (
        "id" serial NOT NULL PRIMARY KEY,
        "forum_id" integer NOT NULL,
        "subject" varchar(255) NOT NULL
    );
    ALTER TABLE "topic"
    ADD CONSTRAINT forum_id
    FOREIGN KEY ("forum_id")
    REFERENCES "forum" ("id");
    ```

@snap[south span-100 text-gray text-08]
@[1-5](You can step-and-ZOOM into fenced-code blocks, source files, and Github GIST.)
@[6,7, zoom-13](Using GitPitch live code presenting with optional annotations.)
@[8-9, zoom-12](This means no more switching between your slide deck and IDE on stage.)
@snapend

```

This *markdown* snippet renders as follows:

![LIVE-CODE-PRESENTING](/doc/assets/gitpitch-in-60-seconds-code.gif)

This sample slide demonstrates the basic features of
[GitPitch Live Code Presenting](https://gitpitch.com/docs/code-features/presenting).
See the docs to learn more about the wide range of unique code presenting
features available to GitPitch presentation authors.


### Sample Slide #6

The *markdown* snippet for this final slide in the sample slide deck is shown
here:

```

---?image=assets/img/code.jpg&opacity=60&position=left&size=45% 100%

@snap[east span-50 text-center]
## Now It's **Your** Turn
@snapend

@snap[south-east span-50 text-center text-06]
[Download GitPitch Desktop @fa[external-link]](https://gitpitch.com/docs/getting-started/tutorial/)
@snapend

```

This *markdown* snippet renders as follows:

![TUTORIAL](/doc/assets/gitpitch-in-60-seconds-6.png)


This slide demonstrates the use of
[background image delimiter syntax](https://gitpitch.com/docs/image-features/background/)
that can be used to inject an image as a background for any slide. Additional
parameters on this *image* delimiter can be used to position, size, scale, and
even control opacity [(pro only)](https://gitpitch.com/docs/pro-features/power)
so you can create the background effects you need.

Again, if you look carefully at the sample *markdown* snippet for this slide
you can see that the `@snap` tag syntax introduced by *snap-layouts* is taking
advantage of a number of
[built-in CSS styles](https://gitpitch.com/docs/themes/css-utility-styles/) -
such as `span-50` and `text-06` - to control the appearance of content
displayed on the slide. As a presentation author this features gives you
almost unlimited flexibility to create slide decks that truly reflect your
product or brand.

<br>

### The Fastest Way from Idea to Presentation.

And that brings us to the end of our whirlwind tour - the
*GitPitch In 60 Seconds* tutorial. If you made it all the way to the end,
congratulations!

While this short tutorial only introduces you to a small number of available
[GitPitch features](https://gitpitch.com/features) we hope what
you have seen so far has made you eager to learn more. And here's one final
enticement...a quick intro to **GitPitch Desktop**, the dedicated presentation
tool for MacOS, Linux, and Windows 10 [Pro + Enterprise].

![DESKTOP](assets/img/gitpitch-desktop.gif)

<br>

Excited? We hope so. Time now to jump straight back into the GitPitch docs
and download [GitPitch Desktop](https://gitpitch.com/docs/getting-started/tutorial).
