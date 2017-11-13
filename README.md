# Git for the Brave and Bold
A short introduction to git, GitHub and GitHub Enterprise

## What is git?

Git is a version control system. It is best used for simple text, meaning configuration files, source code, some touchy poetry and all else clear text.

It can work with binaries and other formats, you have git-lfs or Git Large-File-Storage, but git shines when it comes to text, we'll see how.

Git was developed by Linus Torvalds to better suit the development of the Linux kernel. It was hosted on a proprietary version control platform until 2005, but the company built a paywall around the service (quite ironic when thinking about the Open Source Linux kernel..)

When using git, you know who has done a change on a set of text, when was it done, what where the changes before that. You cn even jump back in time, refer to an older version of the text, start a whole different piece of text based on that historical set.

Git is decentralized, so unlike CVS and Subversion, you get to work alone (don't cry), but you can rapidly share your changes with colleagues and other like minded people without the need of a specialized server somewhere, if you're point A and your developer friend is point B, you don't need an intermittent point.

Git can also be used for centralized colaboration, where you don't need to send the updated version of a document across half the company, the updated document can reside on one place with all the historical changes (and older versions) kept safe for generations to come.

## Why using git?

Git can help you document your steps of work, whether development (as in writing and refactoring code), but also purely logical, when developing documentation, writing configuration files etc. You can take a look back and gain some insights on how a project / specific work started and how it developed.

You can colaborate with your co-workers a lot easier, sharing a code is not zipping a directory and sending it via e-mail across the internet, it is more pointing to a colleague at a repository which he/she can clone and later contribute to (more on that later).

Version control is starting to become a part of all things IT, from infrastructure to development - at times it is highly recommended to use it, as other profesionnals use it already, at other times it is expected you use it, such as with newer programming languages and their build tools (think Rust's cargo, Elixir's mix etc.).

Git can offer you control over what is being changed in your network, think infrastructure, configuration management, application configuration, source code - it let's you have clear and centralized insights on what has been done when and by whom.

## How to use git?

The basic workflow is pretty simple, let's start with a single branch on a local machine. You would need to initialize a repository where you track and commit your work.

    mkdir new_project
    cd new_project
    git init #this initializes our new git repo

From here, every file you create or modify, you need to add to the staging area for a commit. Let's create a new file and add it.

    echo "# My first repository" > README.md
    git add README.md
    git commit -m "Initial commit" # -m stands for commit Message

OK, that is the basic flow when working with local git directories, you should be fine on your own with these three commands if nothing goes wrong (but we'll see what to do when things go wrong as well).


