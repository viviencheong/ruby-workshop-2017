# TechLadies Pre-Bootcamp Ruby Workshop 2017

Materials for the TechLadies Pre-Bootcamp Ruby Workshop 2017, covering CLI basics, Ruby basics, and how to build a simple HTTP server connected to a database.

## Overview

There are three main components of this workshop. We will cover:

* Using the Command line Interface (CLI) with Bash
  - Basic navigation
  - Pipes and Redirection
  - Reading manpages
  - Using `curl`
* Ruby Basics
  - data types and variables
  - control flow
  - functions
  - arrays and hashes
  - classes and object oriented programming (OOP)
* Building a Simple HTTP Server
  - Using the standard library and gems
  - Reading documentation
  - Serving static files
  - RESTful URL routing
  - Using a relational database
  - Using an ORM

I am attempting to cover a lot of breadth in a single workshop, but to minimize "just blindly follow the instructor" programming I will alternate the hands-on sections with a brief 'lecture' on the concepts behind them.

## Setup

The following has been gratefully borrowed from [the setup instructions for the HTML/CSS workshop](https://github.com/TechLadies/guess-the-number-sinatra). Note that if you have already set up your Github and Cloud9 accounts, you can skip some of the steps -- just follow those in **bold**. I'm just leaving everything in for completeness.

### On GitHub
1. Sign up for a GitHub account [here](https://github.com).
2. Once that is done, come back to this page. **On this page, fork this repo by clicking the Fork button in the top right corner (ask for help if you can't find it).**
3. Leave this window open as you will need to perform further set up actions to integrate smoothly with Cloud9.

### Setting up SSH between Github and Cloud9
4. You should receive an email notifying you to sign up for an account on Cloud9. If you do not have one, please alert us at the workshop.
5. Go to https://c9.io/ to sign up for a Cloud9 account by clicking on the GitHub icon in the top right corner. You will need to authorize Cloud9 to use your Github account.
6. Once it's done, you will be at the Dashboard page.
7. Go to `https://c9.io/account/ssh` to access your SSH Settings page.
8. Open another window and go to `https://github.com/settings/keys` to access your SSH and GPG keys on Github.
9. Click on the green New SSH key button in the top right corner.
10. Enter "Cloud9 IDE" in the Title field.
11. Switch back to the SSH Settings page in the previous window and copy everything in the grey box. Paste the contents in the Key field on your SSH and GPG keys page on Github.
12. Click on the green Add SSH key button.

### On Cloud9
13. **Click on Create New Workspace.**
14. **Enter a name for your workspace and a brief description.**
15. **Fill in `git@github.com:<YOUR_USER_NAME>/ruby-workshop-2017.git` in the field Clone from Git or Mercurial URL (optional). This is the repository that you forked to your own account in the earlier steps.**
16. **Select *Blank* for the Choose a template option.**
17. **Click on the green Create Workspace button to proceed.**
18. **You should see a loading window, and this may take a while, so keep the window open and let it run. Please try this at home.**
19. **When things are set up, you should see your workspace, with a file manager in the left column, a text editor taking up most of the space in the main right area and a smaller terminal in the bottom of the right area.**
20. **Now *in your terminal*, type: `gem install bundler`. To test that it was successfully installed, type: `bundle`. You should see a red line of text: `Could not locate Gemfile`.**

After you're done with this, continue to the next section to figure out where all the files you'll need are laid out.

## Where's the Stuff

First, if you want to view the slides I'm using, you can open the `slides.pdf` file.

There should be 4 directories in your workspace. You can ignore the `html-slides` one. `notes` will contain the notes I will be using for this workshop:

```
notes/
├── cli_101.md
├── genealogy_of_programming_languages.svg
├── resources.md
├── ruby_101.md
└── simple_server.md
```

`resources.md` contains a list of useful resources you can check out in your own time. We will be covering the notes in this order: `cli_101.md`, `ruby_101.md` and `simple_server.md`. Don't be frightened by the length of the notes. I wrote them to be very comprehensive, so you can easily refer to them even after the workshop. The notes also go into detail about some things I may not talk about during the workshop, and is for those who are interested to dig around more. (I always end up writing long notes. It must be some strange compulsion).

The `exercises` folder will contain the skeleton code that you will work to fill up throughout the workshop. I will direct you to the relevant files at the needed time; the notes will also refer to them:

```
exercises/
├── ruby_101
│   ├── dog_class.rb
│   ├── player.rb
│   ├── roll_and_die_final.rb
│   └── roll_and_die_oop.rb
└── simple_http_server
    ├── index.html
    ├── init_db.rb
    ├── player.rb
    ├── players.rb
    └── server.rb
```

Finally, `references` will contain the completed code for each exercise. It is there for you to refer to in case you get lost along the way. But of course, make a good attempt on your own first before looking at them.

## Misc

If you spot typos/mistakes in the notes and etc., kindly let me know and I will correct them :)
