# Metaprogramming for Maniacs Live Coding materials

## Setup

[Slides](https://docs.google.com/presentation/d/1Ugq1LvLssx2dTQRGMWdXxJ0dkz4SuY36hfCVvbN_05Q/edit?usp=sharing)

This presentation makes use of git to jump between iterations of demos. For this reason the demos are individual git submodules. Take this into account when cloning:

```
# Clone with submodules
git clone --recurse-submodules git@github.com:gregmalcolm/metaprogramming-for-maniacs.git maniacs
```

The project code is initally at the "end of demo" state. Reset it if you want to take it back to the beginning:

```
cd maniacs
./reset
```

## Aliases

I use a series of aliases to move around during the demo. This is my person setup (on a mac),

```
# update accordingly
export MANIACS_PATH=~/git/maniacs

alias maniacs='cd $MANIACS_PATH'
alias unix='cd $MANIACS_PATH/unix_anywhere'
alias mcrails='cd $MANIACS_PATH/mcrails'
alias n='scripts/next'
alias b='scripts/back'
```

In mcrails and unix_anywhere folders demos these scripts are handling travel through the git shas:

```
scripts/next
scripts/back
```

I use git folders starting from 0 increasing in increments of 10

`./reset` resets everything back to the "0" starting branch