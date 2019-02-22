# homebrew-qt

Tap and Formula to install Qt5 with QtWebKit.

## Why?

We need to use Qt5 with Webkit on MacOS.

As of Nov 2017, Homebrew-core are drop `with-qtwebkit` option from qt formulae currently.
It resulted from that there are no official upstream release which corresponds to Qt 5.9.2 or later from Webkit community.
Maintainer's decision should be respected indeed, however we need to installation of Qt with Webkit right now.

## What's this?

Tap includes formulae which installs `QtWebKit` and `QtWebKitWidgets` modules.

## How it use?

    brew tap uncovertruth/qt
    brew install qt5-webkit  # `qt` will installed automatically, because formula depends on it.

## About

This tap is currently maintained by [uncovertruth](https://uncovertruth.co.jp/en/)
