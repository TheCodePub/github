# Introduction to GitHub

What's GitHub? If you've googled "GitHub", you might have seen this summary on Wikipedia:

> GitHub is a Web-based Git repository hosting service, which offers all of the distributed revision control and source code management (SCM) functionality of Git as well as adding its own features.

Which sounds really boring and technical and complicated. Blergh. Let's zoom out from the technology and focus on what you can do with GitHub: in a gist, GitHub is a tool to collaborate with people. If you're building something with other people, you can use GitHub to host your files, plan ahead, track issues, and make sure you don't do conflicting work. That collaboration is primarily done through *issues* and *pull requests*, and the best way to understand GitHub is to get our hands dirty and create a pull request.

## Your first Pull Request

Hooray! A pull request! But what's even a "Pull Request"? *Creating a pull request* is a fancy way of saying *suggesting a change* or *proposing a change*. It's how people collaborate on GitHub and make sure they don't do any conflicting work. When you create a `Pull Request`, you've made an edit to something, and you're requesting that the owner of what you're editing reviews your change.

Say someone has published a list of great design books on GitHub:

```
- The Design of Everyday Things by Donald A. Norman
- On Web Typography by Jason Santa Maria
- Mobile First by Luke Wroblewski
- Don't Make Me Blink by Steve Krug
```

You notice a mistake in the last book title: it's actually "Don't Make Me **Think**". If you want to suggest a change to fix the title, you would copy the list, and make the change:

```
- The Design of Everyday Things by Donald A. Norman
- On Web Typography by Jason Santa Maria
- Mobile First by Luke Wroblewski
- Don't Make Me Think by Steve Krug
```

You then create a pull request—a request to the owner of the list to "pull in" your changes. They can accept your change, whereupon it's saved into their version, or they can reject your suggestion. Every Pull Request also comes with a discussion thread where you can talk about why the change is a good (or bad) idea, and if there are any additional changes you need to make for the owner to accept it. 

[Here's how a pull request created to fix the spelling mistake in the example above would look like](https://github.com/TheCodePub/github/pull/4). Click around to see what's going on: in addition to the discussion, there's a tab for commits, and a tab for files. Don't worry if you don't understand what all of this means yet: we'll get back to it soon.

## Your challenge

We have a list for Code Pub Hackers who've created a Pull Request with the help of this guide: http://thecodepub.github.io/lab. Your challenge is to add yourself to that list. Ready? Great! Here's how to do it:

### Step 1: Clone the repository

1. Create a GitHub account
* There are several ways to a clone the repository (or project). One way is to use GitHub's official client for Mac and Windows. Head over to https://desktop.github.com and download the app.
* Install the app, and log in with your GitHub account.
* Go back to your browser and head over to https://github.com/TheCodePub/thecodepub.github.io
* Look for a button on the far right labeled "Clone in Desktop". Click it to clone the repository. 

### Step 2: Add yourself to the list


1. In GitHub for Desktop, open the folder of the newly cloned repository by clicking on `Repository -> Open in Finder` (or press CMD+Shift+F)
* We need an image for the list, so let's start by adding it to the project. Find the folder `/images/hackers/`. Add an image to it (of yourself or something else), and make it 260 px wide and 260 px tall. Copy the filename of the image—we'll need it soon.
* Locate and open the folder called `_hackers`
* You'll see files ending in `.md`. Make a duplicate out of one of them (anyone), and rename the file to include your own name, like so: `[your-name].md`.
* Open your newly duplicated file with a text editor. If you haven't installed a text editor, try [Sublime](http://sublimetext.com).
* Change the file to include your name, and your twitter username if you have any. On the row that says `image:`, paste in the filename of your newly added image.
* Save the file.

### Step 3: Creating a Pull Request

1. Go back to *GitHub for Desktop*
* You should now see your uncommited changes listed in the app. If you can't see them, look for the button `1 uncommited change` in the top bar of the app.
* Create a new branch. Branches are git lingo for `versions`. This is your version of this website where you've added yourself to the list. In the top left of the app, press the "Add a branch" button. Name the branch something descriptive of your change. If your name is "Unn", the branch name could be `add-unn-to-hackers`.
* With the branch created, save your changes. When you're working with git, this is called "committing". To the left, find the field that says "Summary". Add a description of your change, and press "Commit to…" at the very bottom of the window.
* Become a member of the org. To create a pull request, you need to become a member of the TheCodePub org. Come up to Unn or Tobias and ask to be added!
* Hooray! You've made a change and saved it. In the top right corner, look for a button called "Pull Request". Press it, and a pane will fold out from the right. Press "Create Pull Request" to publish your changes to GitHub.

### Step 4: Merging

Since you're not the maintainer of this repository, you won't be able to merge the change on your own. To get it merged, you need to wait for someone with `write` access to press the button. If you don't let anyone know you've suggested a change, this may take a while, so let's make sure someone sees your Pull Request.

1. When you created the Pull Request, GitHub for Desktop displays a URL. If you haven't already clicked the URL that showed up when you created yours, do it now.
* Let's mention someone with write access to this repository to let them know that you're waiting for a review. On GitHub you can mention users and teams by writing "@" in a comment—GitHub will help autocomplete it for you. There's a team with write access to this repository called `Editors`, with fellow Code Pub Hackers. Everyone in that team can help you merge your PR, so let's mention them. You've already left a comment on your PR when you created it, so instead of leaving another one, press the pen icon in the top right corner of your existing comment to edit it.
* In your comment, start writing "@e"—the team "TheCodePub/Editors" should appear in the autocomplete dropdown. Press enter, and save your comment. Maybe add a few emojis :boom:
* And the waiting game begins. A member of the Editor team will merge your pull request, or potentially request that you make additional changes before they merge. Look out for new notifications in the very top right of GitHub.com.

When your PR gets merged, your change will be published to http://thecodepub.github.io/lab.

### Summary

What did we do here?

* We copied a project on GitHub to our own computer. This is referred to as **cloning a repository**.
* We made a change, and saved that change to a new version of the project. In git, this is referred to as **committing** and **creating a branch**.
* We suggested a change. On GitHub, this is referred to as **creating a pull request**.

When working with Git and GitHub there's a lot of complicated words used to describe simple things. Don't worry if you can't remember them all—they're not that important, and they'll stick eventually.

## Next steps

- Read about how GitHub recommends that you work with GitHub in [GitHub Flow](https://guides.github.com/introduction/flow/).
- We've used [GitHub Pages](https://pages.github.com) to publish the site in this tutorial. [Read more about creating your own GitHub Page](https://pages.github.com).
- GitHub Desktop is a great way of working with git and GitHub, but many choose to work with the terminal instead. To learn about how to use GitHub with a terminal, check out [git-it](http://jlord.us/git-it/) by @jlord.
- Read more about [Git](https://git-scm.com).
