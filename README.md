# CMPSC 100: Fall 2020, Midterm Assessment

* Distributed: 5 October 2020
* Due: 11 October 2020

## Point value

---

|Type         |Point value |
|-------------|------------|
|Total        |100 pts.    |
|             |10% of course|

## Table of contents

* [Accepting the assignment](#Accepting-the-assignment)
* [Overview](#Overview)
  * [Evaluation](#Evaluation)
* [Instructional materials](#Instructional-materials)
* [Wrap-up](#Wrap-up)
  * [GatorGrader](#GatorGrader)
  * [Submitting your work](#Submitting-your-work)
  
## Accepting the assignment

---

- [ ] Log into the `#assignments` channel in our class [Slack](https://cmpsc-100-00-fa-2020.slack.com)
- [ ] Click the link provided for the lab assignment and accept it in GitHub classroom
- [ ] Once the assignment finishes building, click the link to go to your personal repository assignment

## "Cloning" a repository

### Using the correct download link

- [ ] On this repository's page, click the `Clone or download` button in the upper right hand corner
* You may need to scroll up to see it
- [ ] In the upper right corner of the box that appears, click `Use SSH`
- [ ] Copy the link that appears in the textbox below the phrase "Use a password with a protected key."

#### Cloning

* [ ] Type `ls` in your terminal window
* You should be in your `~` directory
- [ ] Once there, "clone" the repository using the link copied above
  * If I (the instructor) were to clone my own repository, I'd enter (your link will look different):

```
git clone git@github.com:allegheny-college-cmpsc-100-fall-2020/cmpsc-100-fall-2020-midterm-assessment-dluman
```

## Overview

This repository hosts the Midterm Assessment. As with all things in this course, this assignment allows you to access:

* notes
* previous labs, worksheets
* office hours
* Technical Leaders

Of course, this doesn't mean that you should rely on any of these resources walking you through this step-by-step. The Midterm Assessment is designed to practice cumulative problem-solving skills.

You will notice that some of the code already exists in the notebook. This will allow you to exercise some decision-making in addition to original invention. For ease, I have provided a data structure which contains some essential information required to solve the problem. You'll need to build some of the structures on your own using suggested variable names.

## Instructional materials

### Programming

* [Midterm assessment: A prime spot](assessment/CMPSC%20100%20-%20Fall%202020%20-%20Midterm%20Assessment.ipynb)

### Writing

* [Midterm reflection](writing/reflection.md)

## Wrap-up

---

### GatorGrader

GatorGrader is an Allegheny College-developed, student-written and maintained application that grades your work for you. The long and short of it, before and when you turn in your assignments, you can know what your approximate grade will be.

(It doesn't do _everything_ for us, but it gives us a good starting point for evaluating your work.)

You don't need to do anything to get it -- I will distribute all the files you need with every repository. You realize the following benefits:

* Complete grading transparency
* Grading criteria _never_ changes
* The criteria is very specific; you will know what changes you need to make

This application runs in your terminal tab, and can grade:

* The whole repository
* Just worksheets
* Just the lab

## Checking your work

---

No matter where you are in your repository, the command to start and run GatorGrader is always the same:

```
gradle grade
```

However, you need to be _in the right place_ to get the right result. The following table summarizes the various grading locations.

| Location | Grading             |
|----------|---------------------|
| Root folder | Repository requirements |
| `assessment/` | Programming requirements |
| `writing/`        | Writing requirements |

### Submitting the assignment/saving progress

The GitHub platform is a place to store your work. So, it makes some sense that should be able to _clone_ (download) from it, and push back (upload) to it. Here, we'll learn this second part.

- [ ] `cd` to your `~` folder
- [ ] Locate your `cmpsc-100-fall-2020-midterm-assessment` folder and `cd` to it.

Once in this folder, we need to tell git that there have been changes.

- [ ] Type `git add .` and press `Enter`
* This tells git to look through the _entire_ folder structure for new changes and "stage" them

- [ ] Type `git commit -m "YOUR COMMIT MESSAGE"` to "label" the commit
* This is typically something like `git commit -m "Fixing a typo"` -- the message in quotes should be as descriptive as possible, while still remaining somewhat short

- [ ] To send all changes to the server, type `git push`
- [ ] At the prompt, input the password associated with the `SSH Key` you created earlier in this exercise (yesterday)

Once the process finishes successfully, we're done!

#### A strong warning

<div class="alert alert-block alert-danger">
    <p><strong>While we may use this server to store code, <u>you</u> are responsible for using GitHub as your main backup.</strong></p>
    <p>While I back this server up on a regular basis, I cannot guarantee that I'll have the ability to restore up-to-the-minute data for your work.</p>
    <p>Remember: to err is human; to back up your work is divine.</p>
</div>
