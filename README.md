# Introduction

This repo generates a docset in the [Kapeli Dash Mac App](https://kapeli.com/dash) for the Swift Programming Language v5.1

![](swift.gif)

## Getting Started

You can simply clone the repo and double click the Swift.docset file to start using in Kapeli Dash.  
If you want to manually build the docs you can follow the steps below.

## Installation

1. If you don't have brew installed first install [brew](https://brew.sh/). Enter this into your terminal:  
`/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`

2. Once you have you brew, you need to install [dashing](https://github.com/technosophos/dashing#readme). Enter this into you terminal:  
`brew install dashing`

3. Then you'll need to install [wget](https://pypi.org/project/wget/#description). Enter this into your terminal:  
`brew install wget`

## Manually Building Swift Docset

1. Clone the repo.

2. In the project directory run:  
`wget -k -r -p -np https://docs.swift.org/swift-book/LanguageGuide/TheBasics.html`

3. Open a text editor (ie. VSCode), and do a search and replace for all paragraph markings (). Replace the () with nothing (ie. "").

4. Once complete run:  
`dashing build`

5. This create a Swift.docset file. You can then doubleclick this icon and it will be in Dash.
