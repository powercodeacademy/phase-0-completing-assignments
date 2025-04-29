Learning Goals
--------------

*   Understand the steps needed to complete an assignment and submit it in Canvas

Introduction
------------

During this course, you will work on various assignments as you learn to code. All assignments will be interactive pieces of curriculum that require some work. Some assignments may ask you to follow a set of instructions, while others will ask you to figure out your own solution to pass specific tests. This lesson is your first assignment!

All assignments are hosted on GitHub. In order to work on them, however, you will need to complete work on your local machine. The general process is:

*   Click the "Octocat" GitHub logo in the top right of the page to navigate to the assignment repo on GitHub
*   Create a personal copy (a 'fork') of the assignment in GitHub
*   Download your personal copy (referred to as 'cloning') to your computer
*   Complete the required work
*   Submit your completed work to Canvas

In this assignment, you'll learn the workflow that you will be using to complete your assignments. 

MacOS: Completing Assignments Code Along
----------------------------------------

### A Quick Note on Organizing Work on Your Machine

Throughout this course, you will be downloading many assignments, so it is important to keep your code organized. If you haven't yet, we recommend that you go through the steps in [the previous lesson](https://github.com/learn-co-curriculum/phase-0-organizing-work-on-your-computer) to set up a directory where you can keep all of your work for this course.

> **Note:** The process we'll go through in this lesson will create sub-folders automatically. Whenever you are starting a new assignment, navigate back to your main `prework` folder (`cd ~/Development/code/prework`) before cloning the assignment to ensure these sub-folders don't get created _within each other_.

### Accessing GitHub and Forking

All the lessons in this course have a corresponding repository (repo) in GitHub. On the lesson page in Canvas, you should see a link to the GitHub repo. Clicking that link will open the repository in GitHub.

To fork an assignment, open the GitHub repository and click the **Fork** button in the upper right corner of the page. This creates a copy of the repository under your own GitHub account. If prompted, choose your personal GitHub account.

Once the fork is complete, you’ll have your own copy of the assignment repo where you can make changes. This is where you’ll complete your work for the lesson.

The README.md file in the repository will contain instructions for the assignment. You can follow along with those either directly in GitHub or from within your code editor after cloning.

Forking is a process that creates an exact copy of the code and files. After forking, you can freely edit your copy without affecting the original.

**Go ahead and fork this lesson’s repository now to get started.**

Once you’ve forked the repository, the next step is to download (clone) it to your local machine.

### Cloning to Your Local Machine

To download the repository for this lesson, make sure you're in your personal fork on GitHub, then click the **Code** button. A pop-up will appear which shows several options for cloning: **HTTPS**, **SSH**, and **GitHub CLI**. **Before doing anything else**, be sure to switch to **SSH**. With **SSH** selected, you should see what looks sort of like an email in the box below, starting with `git@github.com:`. You should see your GitHub name after the `:`.

> **Aside:** Why SSH? If you followed the setup instructions, you have added your personal SSH key to GitHub. GitHub will store your personal copies of all the work you do in this course. Because you've added your SSH key, GitHub will know who you are when you send work from your local machine to GitHub to be stored. Using HTTPS instead would require you to sign in from your terminal using your log-in credentials each time you try to push your code to GitHub; it also may not work at all for some assignments.

From here, click the copy button.

![clone-repo](https://curriculum-content.s3.amazonaws.com/phase-0/completing-assignments/clone-repo.gif)

Now, open your terminal and navigate to where you'd like to download the assignment (e.g. `cd ~/Development/code`). Type `git clone` and a space, then paste in the copied SSH link from GitHub. It should look something like this:

    $ git clone git@github.com:<your-user-name>/phase-0-completing-assignments.git
    

Press enter, and you should see a flurry of terminal activity.

> **Troubleshooting**: If you are a Mac user and you see the following message:
> 
> `xcrun: error: invalid active developer path`
> 
> You need to install the Xcode Command Line Tools. Run the following command to install them:
> 
>     $ xcode-select --install
>     
> 
> And follow the prompts. Then try running the `git clone` command again. See [this Stack Overflow post](https://stackoverflow.com/a/52522566) for more details. Note that you may need to re-install `xcode-select` any time you update your Mac OS version.

Once the terminal gives you control to type again, a new folder with the GitHub name of the assignment will have been created. Change directory into this folder to access the assignment files.

    $ cd phase-0-completing-assignments
    

Now type `code .` to open up a text editor window with access to all of the assignment's files. These instructions are now also available on your local machine in `README.md`.

> Note: the first time you open a directory in Visual Studio Code, you'll see a message asking "Do you trust the authors of the files in this folders?" This is a [security feature](https://code.visualstudio.com/docs/editor/workspace-trust) of Visual Studio Code. It's safe to choose "Yes", and we recommend selecting the "Trust the authors of all the files in the parent folder" option to prevent this warning from coming up every time you open a lesson. Just be sure to download your code from trusted sources!

Completing an Assignment
------------------------

Most assignments include tests to help you verify your code is working. These tests run locally in your terminal.

### For each new lesson:

1.  Open your terminal and navigate into the lesson directory.
2.  Run:
    
        npm install
    
    **⚠️ You’ll need to run `npm install` every time you start a new lesson.** If you skip this step, you’ll likely run into errors when trying to run the tests.
    
3.  Then run:
    
        npm test
    

You should again see a flurry of text as dependencies are installed. Then you'll see the results of your test. By cloning this assignment down, you've already passed the test!

    This assignment
        ✓ has been correctly cloned to your local environment
    
    
      1 passing (5ms)
    

### Submitting Your Work

For this lesson, once you've forked the repository and passed the tests, submit a link to **your forked repository** in Canvas.

In future lessons, you'll submit a link to a **pull request**, but that won’t be required just yet — we’ll walk through that process later.

Types of Assignments
--------------------

For most assignments, you will go through the process we just walked through. In our curriculum, these assignments are often referred to as **labs** — coding lessons that include tests. There are a few other types of assignments, though, that require slightly different submission steps:

*   **Code-alongs:** These also require code, but will guide you through what needs to be written. There are no tests to pass, but you will still need to go through forking, cloning, and running `npm install`. There aren't tests for these assignments, but you should still submit your work in Canvas.
*   **Projects:** For these assignments, you'll be building fully functional applications. Some guidelines and requirements will be provided, but it will be up to you to design and create your own app. These will eventually become the projects you showcase to our senior developers! You will submit your projects in Canvas by submitting a link to your GitHub repo.

Submitting Assignments
----------------------

For most assignments, you'll need to manually submit a link to your work on Canvas--this will usually be a link to a Pull Request, but could also be a link to a repo or something else. While viewing an assignment, you should see a **Submit Assignment** section in the bottom of the page.

![submit assignment form](https://curriculum-content.s3.amazonaws.com/canvas-welcome/submit-assignment-canvas-form.png)

Upon submission you should see confetti appear, indicating that your submission has been accepted.

> **Note:** It is possible to submit lab and code-along assignments manually this way. However, the assignment will only be marked as **Submitted**, not **Complete**.

Conclusion
----------

Congratulations! You've completed your first assignment! You now know how to work on and submit assignments going forward:

*   Click the **Ocotocat** GitHub logo to navigate to the assignment repo
*   Fork the repo using the Fork button in the top right
*   Once the assignment is forked, clone it down to your local machine
*   Navigate to the lesson's directory and run `npm install`
*   Complete any required work, then run `npm test`
*   When all tests pass, commit and push your code to GitHub (we'll go over this soon)
*   Open a Pull Request and submit a link to the PR on Canvas (we'll go over this soon)

Equipped with this knowledge, you are now ready to tackle greater challenges!
