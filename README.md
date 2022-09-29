# engl5376-staticsite
Playground for hand-coded site for Online Publishing

## 9/29/2022 - Initial Commit

Based on the given template, the starting site looked something like ![starting point](/img/start.png).

I started by deleting all of the CSS and applying "the new CSS reset" to remove all default formatting.

I then added header and nav sections to contain the Logo/home button and the rest of the internal navigation. I moved the given h1 into the the header and replaced the template text wiht just my name. I grabbed the first scripty font from Google Fonts and applied it to that h1. After changing the font, the logo no longer lined up with the navigation.

I deleted the entire contact section and replaced it with an H2 and introductory section (stolen from my Twitter bio). I didn't like the text going the full length of the page so I set a much smaller `max-width`

I then started a paragraph with a more in depth  about me section covering my work and ensemble history. I then turned one of the given H2s into an H3 to introduce the paragraphs.

I found some svg icons and added them as links to my LinkedIn, my work GitHub page, and my musician site. For some fun interactivity, I added a grow on hover animation.

I then turned the last remaining H2 into a contact section. Based on my findings from the first assignment, I decided to try my suggestion of embedding a Google form as a contact form instead of linking out to it. The form wasn't that customizable and unfortunately came with its own heading (more specifically a title for the form). Unfortunately, the font for the form title is not customizable, so I just deleted the title and replaced it with a hand waving emoji.

The site was looking a little boring so I found a cute animation of a person writing. This then made the content too long for the page so I added `position: sticky;` to the header so the header and navigation would scroll as I scrolled. The header text would then overlap with the main content text so I added a a backgroud with a high opacity to keep the header text legible.

With the always visble header, I decided to add a footer. I modified a [codepen](https://codepen.io/mfritsch) for a heart animation and added the mid-10s trend of made with <3 as well as a copyright with a link to my main playground site.

With my initial commit, the site now looks something like ![initial commit](/img/initial-commit.gif).

### The tech stack

I'm using Visual Studio Code as my IDE. Autocomplete and live staging are nice features. Plus it's free.

I'm using GitHub because it's familiar and it's integration with Netlify.

Netlify gives free staged hosting for this site. The current staged version of this site will always be available at https://engl5376-staticsite.netlify.app/. Having it staged also lets me test it on my actual mobile devices instead of just using the Chrome webdev tools that I would have to do if I were only using local files. An added benefit is that each pull request I open will have its owndeploy preview. For example, [my first pull request](https://github.com/codyjtclark/engl5376-staticsite/pull/1). Admittedly, this PR changed nothing but the human readability of the CSS, but as I make more design and content changes, I'll have an automatic snapshots with a dedicated URL for every change.

### TODOs:
- Vertically center logo and navigation
- Move to flexbox? I currently use a hacky `float: left` on the image. That caused problems setting a max-width for the container holding the paragraphs. Setting a max-width twice what I really needed made it work, but there has to be a better way to get the results I want.
- Figure out how to control the space between the external link icons. When I try to add a padding, they simply disappear. I'm currently using a hacky `justify-content:space-between;` coupled with`max-width:40%` to get the current result.
- Perhaps left align the contact form and add an image to the right? The page feels unbalanced.
- Delineate the sections of the website more clearly. Everything's white.
