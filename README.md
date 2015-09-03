# Introduction to GitHub

## Your first Pull Request

Hooray! A pull request! But what's even a `Pull Request`? "Creating a pull request" is a fancy way of saying "suggesting a change". Pull Requests are what fuels the collaboration at GitHub. When you create a `Pull Request`, you've made an edit to something, and you're requesting that the owner of what you're editing reviews your change.

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

## Your challenge

We have a list of Code Pub Hackers who've created a Pull Request with the help of this guide: http://thecodepub.github.io/hackers. Your challenge is to add yourself to that list. Ready? Great! Here's how you do it:

### Step 1: Clone the repository

1. Create a GitHub account
* Head over to https://desktop.github.com and download the GitHub app
* Install the app, and log in with your GitHub account
* Go back to your browser and head over to https://github.com/TheCodePub/thecodepub.github.io
* Clone the repository. Look for a button on the far right labeled "Clone in Desktop"

### Step 2: Add yourself to the list


1. In GitHub for Desktop, open the folder of the newly cloned repository by clicking on `Repository -> Open in Finder` (or press CMD+Shift+F)
* Locate and open the folder called `code-pub-hackers`
* You'll see a lot of files ending in `.md`. Make a duplicate out of one of them (anyone), and rename it to include your own name, like so: `[your-full-name].md`
* Open your file with a text editor
* Change the file to include your full name, your twitter if you have any, and today's date.
* Save the file

### Step 3: Creating a Pull Request 

1. Open GitHub for Desktop
* You should now see your uncommited changes. If you can't see them, look for the button `1 uncommited change` in the top bar of the app
* Create a new branch. Branches are git lingo for `versions`. This is your version where you're adding yourself to the list. In the top left of the app, press the "Add a branch" button. Name the branch something descriptive, for example `add-your-name`
* With the branch created, save your changes. When you're working with git, this is called "committing". To the left, find the field that says "Summary". Add a description of your change, and press "Commit to…" at the very bottom of the window.
* That's it! You've made a change and saved it. In the top right corner, look for a button called "Pull Request". Press it, and a pane will fold out from the right. Press "Create Pull Request".

### Step 4: Merging

Since you're not the maintainer of this repository, you won't be able to merge the change. To get it merge, you need to wait for someone with `write` access to press the button. If you don't let anyone know you've suggested a change, this may take a while, so let's make sure someone sees your Pull Request.

1. When you created the Pull Request, GitHub for Desktop displayed a URL. If you haven't already clicked it, do it now.
* Let's mention someone with write access to this repository to let them know that you're waiting for a review. On GitHub you can mention users and teams by writing "@" in a comment—GitHub will help autocomplete it for you. There's a team with write access to this repository called `Editors`, with fellow Code Pub Hackers. You've already left a comment on your PR when you created it, so instead of leaving another one, press the pen icon in the top right corner of your existing comment.
* In your comment, start writing "@e"—the team "TheCodePub/Editors" should appear in the autocomplete dropdown. Press enter, and save your comment. Maybe add a few emojis :boom:
* And the waiting game begins. A member of the Editor team will merge your pull request, or potentially request that you make additional changes before they merge.

### Summary

What did we do here?

* We copied a project on GitHub to our own computer. This is referred to as **cloning a repository**.
* We made a change, and saved that change to a new version of the project. In git, this is referred to as *committing** and **creating a branch**.
* We suggested a change. On GitHub, this is referred to as **creating a pull request**.

When working with Git and GItHub there's a lot of complicated words used to describe simple things. Don't worry if you can't remember them all—it'll stick eventually.
