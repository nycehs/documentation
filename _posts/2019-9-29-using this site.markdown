---
layout: post
title:  "Using this site"
date:   2019-9-29 10:18:27 -0400
categories: jekyll update
---
So you like the Documentation site and you have something to add to it. Great! Here is how.

**Jekyll**. Install Jekyll on your machine. You can follow [these instructions](https://jekyllrb.com/docs/installation/windows/), but I also found [this video series](https://www.youtube.com/watch?v=T1itpPvFWHI&list=PLLAZ4kZ9dFpOPV5C5Ay0pHaa0RJFhcmcB) helpful. Pro tip: put the playback on 1.5 speed to save time.

Installing Jekyll means installing Ruby. Both of these are done via the command line, which can be a little disorienting or confusing at first, since you can't see what's happening. But it's happening.

**Github**. Download, install, and set up GitHub desktop. Connect it to our /NYCEHS organization account. New team members will need to set up a Github account and be invited to our organization. 

Github Desktop will create a local directory on your machine. This is where it stores local files for you to work on.

On `github.com/nycehs`, we have a repository called `/Documentation`. There are two branches: `Documentation`, and `gh-pages`. The branch `gh-pages` is how the Documentation Site is actually published as a Github Page that we can see on the Internet.

Clone the /Documentation repository to your local machine. This means you're downloading files from Github to work on them. As you work on them on your local, Github Desktop will identify the files you change and the changes you make.

**Starting up Jekyll**. Open the Command Prompt and enter the commands to take you to the directory where your cloned copy of Documentation lives. [Here are basic commands for moving around folder structures](https://www.digitalcitizen.life/command-prompt-how-use-basic-commands) in the Command Prompt.

In the command prompt, once you're in the `/documentation folder`, start up Jekyll. The first time you do this, enter `bundle exec jekyll serve`. This does an initial build of the site based on the source materials.

Later, once the site is already built on your machine, you can just run `jekyll serve` which starts up Jekyll and makes it act like an internet server, allowing you to view the site in your browser at `localhost:4000/documentation/`. Better, if you start it up with `jekyll serve --force_polling`, it will automatically re-compile the site when you make changes. This is useful for seeing your edits.

**A quick Jekyll primer**. In your folder `/documentation`, you’ll see subfolders – namely `_posts` and `_site`. Jekyll takes the information in `_config.yaml`, the content of `_posts`, and other pages (you can see `about.markdown` and `index.markdown` in there), and it compiles them into HTML pages in the `_site` folder. 

What this means is that we edit .markdown files in the root directory and in _posts. This is the source material. We don’t edit things in _site – this is the output from Jekyll.

If you edit _config.yaml, then you need to re-compile the site using `bundle exec jekyll serve`. Usually - like if you create a new Jekyll site - you will be able to see it by going to `localhost:4000` in your web browser. However, our `_config.yaml` file includes `baseurl: "/documentation"` which means that we have to go to `localhost:4000/documentation/` to see the site.

**Getting to it: making changes to the site**. Now that Github Desktop is set up, you've cloned the repository, and you've started up Jekyll, you're ready to make some changes. Open `index.markdown` in Notepad++. Add a sentence or two, and then save it. Take a look at `localhost:4000/documentation/` and you should see your changes.

Now, look at Github Desktop. It should identify the file that you’ve changed. In the lower left, add a brief summary and description, and “commit to gh-pages.” Github Desktop basically guides you through the rest of the steps – next, you push it to the origin (which is the `gh-pages` branch of our Documentation repository). Once you push it to the origin, you’ll be able to see it on our Github page. Think of this basically as a staging server.

**Merging changes into the repository**. So you’ve pushed changes to gh-pages. But the main repository, Documentation, hasn’t yet changes. Github knows this.  After you’ve pushed your changes to the origin branch (gh-pages), Github Desktop prompts you to create a pull request. Click the blue button labeled “create a pull request” and it will take you to Github. First you’ll see it say "Comparing changes: there isn't anything to compare."

Notice the two buttons - you're comparing the same branch `gh-pages` to itself. Change the left button to `documentation` and you'll see the page say "Open a pull request." It's telling you that there's a change in `gh-pages` that you can merge into `documentation`. 

Create a pull request, review the next step, and then click Merge Pull Request.

You're done! You've updated the Documentation Site on your local using markdown, you pushed the changes to `gh-pages`, reviewed them on [this site right here](https://nycehs.github.io/documentation/), and then merged those changes into our shared repository.
