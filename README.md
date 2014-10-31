HaskellNotes
============

Notes on Haskell, especially on how to create a new library.  Note
these are just my notes, based on my best understanding, and do not
necessarily represent best practices.

These are my notes on how to create a new Haskell library, using
github and cabal.

# Important Links

* Cabal Guide: [http://www.haskell.org/cabal/users-guide/](http://www.haskell.org/cabal/users-guide/)
* Github markdown help: [https://help.github.com/articles/github-flavored-markdown](https://help.github.com/articles/github-flavored-markdown)
* Haddock Users Guide: [http://www.haskell.org/haddock/doc/html/](http://www.haskell.org/haddock/doc/html/)

# Initializing Cabal

You only need to do this once per system.  All of the folowing step should
take place in your home directory

* Install a native cabal and ghc (sudo apt-get install cabal-install or similar)
* Delete any fossil .ghc and .cabal directories in your home directory
* cabal update
* cabal install cabal-install
* Add the line:
    export PATH=~/.cabal/bin:$PAT
to .bashrc

TODO: figure out how to compile newer versions of ghc inside of cabal.

# Create A Git Repository

Go to github.  The +/- in the upper right hand corner lets you create
a new repository.  Name it.

Copy and paste the git repo url (right hand side) and git clone the repo.

# Initialize cabal environment

    cabal sandbox init
    cabal init

Note, project web site is the github URL.

Add the .cabal file, the LICENSE file, and Setup.hs to git and commit.

Edit the .cabal file, add an exposed module.  Commit.

# Add some source code

The exposed module helps.  Note that it expects module Foo.Bar to be
in file Foo/Bar.hs.

# Use cabal repl, not ghci

    cabal repl

instead of:

    ghci

# Creating documentation

    cabal haddock

* Cabal Guide: [http://www.haskell.org/cabal/users-guide/](http://www.haskell.org/cabal/users-guide/)


