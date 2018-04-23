[![GitPitch](https://gitpitch.com/assets/badge.svg)](https://gitpitch.com/gitpitch/in-60-seconds/master?grs=github)

# GitPitch In 60 Seconds

To experience just how simple it is to create a GitPitch slideshow
presentation, follow along with this short tutorial.

> Tutorial also available for [GitLab](https://gitlab.com/gitpitch/in-60-seconds) and [Bitbucket](https://bitbucket.org/gitpitch/in-60-seconds) users.

### Step 1. Create a Repository on GitHub

Using an existing account on GitHub, either:

- Create a new repository on GitHub and clone it to your local disk or 
- Select one of your existing repositories on GitHub and make sure it has been cloned to your local disk

This tutorial will show how by simply adding files to your chosen repository, [https://gitpitch.com](https://gitpitch.com) can read and automatically translate those files into an online slideshow presentation.


### Step 2. Create a **PITCHME.md** File in the root directory of your Repository

Using your preferred code editor create a file called **PITCHME.md**, then add 
and save the following Markdown content:

```
# Flux 

An application architecture for React

---

### Flux Design

- Dispatcher: Manages Data Flow
- Stores: Handle State & Logic
- Views: Render Data via React

---

![Flux Explained](https://facebook.github.io/flux/img/flux-simple-f8-diagram-explained-1300w.png)
```

It is worth taking note of the following:

1. The **PITCHME.md** file name is a new convention introduced by GitPitch
1. The **PITCHME.md** file name is case sensitive
1. The **PITCHME.md** file content is standard GitHub Flavored Markdown
1. The `---` markdown fragment acts as a delimiter between content on different slides

For the sample markdown used in this tutorial, when GitPitch processes the sample **PITCHME.md** markdown content it will result in a simple presentation with just three slides.


### Step 2. Push **PITCHME.md** to your GitHub Repository in the Cloud

At this point you have simply created one new file within your chosen repository. Now you need to add this file under Git version control and then push these local changes to your upstream repository on GitHub in the cloud:

```
git add PITCHME.md
git commit -m "Added my first GitPitch slideshow content."
git push
```

At this point, the upstream version of your chosen repository on GitHub should have the new **PITCHME.md** file in it's root directory.


### Step 3. Done!

Your GitPitch slideshow presentation is now waiting for you to share or present at its public URL.

You can access your slideshow presenttion on `gitpitch.com` by building a URL with the following structure:

```
https://gitpitch.com/$USER/$REPO/$BRANCH
```

Where the following substitutions must be made by you to reflect your details:

- `$USER` - must be replaced with your GitHub account name
- `$REPO` - must be replaced with the name of your chosen GitHub repository
- `$BRANCH` - must be replaced with the branch you used when adding your `PITCHME.md` file. If you did not specifically create a feature branch for this tutorial, then the default branch name is `master`.

For example, this tutorial is itself within a repository. And that repository includes a `PITCHME.md` file. So you can view the associated GitPitch slideshow presentation at the following URL:

[https://gitpitch.com/gitpitch/in-60-seconds](https://gitpitch.com/gitpitch/in-60-seconds

Note how `$USER` has been replaced with my GitHub account name ( gitpitch ) and `$REPO` has been replaced with the name of my repository ( in-60-seconds ). 

Once you have created your own GitPitch slideshow presentation URL it should open and look a lot like this:

![Slideshow-In-60-Seconds](/images/in-60-seconds.jpg)

Immediately you can [download](https://github.com/gitpitch/gitpitch/wiki/Slideshow-Offline) 
your slideshow for offline presentation, 
[print](https://github.com/gitpitch/gitpitch/wiki/Slideshow-Printing) it as a 
PDF document, or [share](https://github.com/gitpitch/gitpitch/wiki/Slideshow-Sharing) 
it on social media.

### The Fastest Way from Idea to Presentation.

Beyond support for standard Markdown on presentation slides, GitPitch 
delivers a [wide range of features](https://gitpitch.com/features) that cater
to developers, speakers, educators, etc.

See the [Template Gallery](https://gitpitch.com/templates) for quickstart
markdown presentaton templates. Simply clone, fork, or download the templates
repo and start customizing the presentation markdown to reflect your needs.

To view a live slideshow demonstration of a wide range of features try
out the GitPitch [Kitchen Sink](https://gitpitch.com/gitpitch/kitchen-sink).
To dig deeper, see the [GitPitch Wiki](https://github.com/gitpitch/gitpitch/wiki)
for a detailed How-To.

And don't forget to check out [GitPitch Pro Features](https://gitpitch.com/pro-features)
to learn about working with **private Git repos** and to enjoy enhanced
presentation features, including privacy, confidentiality, and team
collaboration.

