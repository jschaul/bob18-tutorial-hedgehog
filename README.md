# A hedgehog tutorial

Course material for the [bobkonf course in Berlin on Feb 23rd,
2018](http://bobkonf.de/2018/fischmann.html).


### Setup

You will need an editor of your choice and the terminal to run ghc in
interactive mode.

Before you come to the course, you should:

```
stack upgrade  # (just in case, this has been tested with 1.6.3., and is known to fail with 1.5.1)
export PATH=$HOME/.local/bin:$PATH  # (just in case...  this is where stack just installed itself)
git clone https://github.com/fisx/bob18-tutorial-hedgehog
cd bob18-tutorial-hedgehog
stack setup
stack build --fast  # (in case you are in a hurry: `--fast` reduces compile time and increases run time.)
echo 'iAmReady' | stack exec -- ghci 01_Basics.hs
```

Give it some time, there are a lot of hidden dependencies in some of
the exercises.  Eventually you should see this on your terminal:

```
GHCi, version 8.2.2: http://www.haskell.org/ghc/  :? for help
[1 of 1] Compiling Basics           ( 01_Basics.hs, interpreted )
Ok, one module loaded.
*Basics> ━━━ Basics ━━━
  ✓ prop_const passed 100 tests.
  ✓ 1 succeeded.
*Basics> Leaving GHCi.
```

That's it!  You are ready for the tutorial.

If you are having difficulties getting this far, please check that
your local repository is in sync with github, then open an issue.
