# homebrew-qt

`brew install qt --with-qtwebkit`

## Why?

We need to use Qt5 with Webkit on MacOS.

As of Nov 2017, Homebrew-core are drop `with-qtwebkit` option from qt formulae currently.
It resulted from that there are no official upstream release which corresponds to Qt 5.9.2 or later from Webkit community.
Maintainer's decision should be respected indeed, however we need to installation of Qt with Webkit right now.

## What's this?

Just a copy of `Formula/qt.rb` in the `homebrew-core` repository,
at revision `824af16c2d75a767dabacac4159cc57c14271ac2`.

Not modified.

## How it use?

    brew uninstall qt  # if you have old installation
    brew install uncovertruth/qt/qt

## Alternatives

This tap is not requisite to install Qt5 with webkit via Homebrew, but a shorthand.
You can also install it along with a few steps as below:

    rm -f /path/to/Library/Caches/Homebrew/qt*
    cd /path/to/Homebrew/Library/Taps/homebrew/homebrew-core
    git checkout 48421a0c709ea9f204cd41d0e28fcfc5854f0d49 Formula/qt.rb
    HOMEBREW_NO_AUTO_UPDATE=1 brew install qt --with-qtwebkit

## About

This tap is currently maintained by [uncovertruth](https://uncovertruth.co.jp/en/)
