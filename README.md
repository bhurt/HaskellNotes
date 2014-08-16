HaskellNotes
============

Notes on Haskell, especially on how to create a new library.  Note
these are just my notes, based on my best understanding, and do not
necessarily represent best practices.

These are my notes on how to create a new Haskell library, using
github and cabal.

Github markdown help: [https://help.github.com/articles/github-flavored-markdown](https://help.github.com/articles/github-flavored-markdown)

# Create A Git Repository

Go to github.  The +/- in the upper right hand corner lets you create
a new repository.  Name it.

Copy and paste the git repo url (right hand side) and git clone the repo.

# Initialize cabal environment

    cabal sandbox init
    cabal init

Note, project web site is the github URL.

Add the .cabal file, the LICENSE file, and Setup.hs to git and commit.

