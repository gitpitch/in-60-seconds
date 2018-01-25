[![GitPitch](https://gitpitch.com/assets/badge.svg)](https://gitpitch.com/gitpitch/in-60-seconds/master?grs=github)

# GitPitch In 60 Seconds

To experience just how simple it is to create a GitPitch slideshow
presentation, follow along with this short tutorial.

> Tutorial also available for [GitLab](https://gitlab.com/gitpitch/in-60-seconds) and [Bitbucket](https://bitbucket.org/gitpitch/in-60-seconds) users.

### Step 1. Create **PITCHME.md**

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

Before moving on to the next step it's worth taking note of the following:

1. The **PITCHME.md** file name is case sensitive.
1. The **PITCHME.md** file content is standard Markdown.
1. The `---` markdown fragment acts as a delimiter between slides.

Using `---` is a GitPitch convention, acting as a delimiter to denote the 
separation between content on different slides in your presentation. You can use 
[custom delimiters](https://github.com/gitpitch/gitpitch/wiki/Custom-Slide-Delimiters) 
if you prefer. For this example, when GitPitch processes the Markdown content it 
will result in a simple presentation with just three slides.


### Step 2. Commit **PITCHME.md**

Now add this file to your Git repo and push to GitHub:

```
git add PITCHME.md
git commit -m "Added my first GitPitch slideshow content."
git push
```

### Step 3. Done!

Your GitPitch slideshow presentation is now waiting for you to share or present 
at its public URL. To see a live demonstration of this slideshow presentation 
[click here](https://gitpitch.com/gitpitch/in-60-seconds). Your own 
presentation should look a lot like this:

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

