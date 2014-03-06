# pivotal-tracker.el

Pivotal Tracker Mode provides a mode and functions for interacting with Pivotal Tracker through its API.
It is designed to give most of the functionality that is important to a developer.
It is not an attempt to replace every feature of the web interface.

## Installation

You can install via [MELPA](http://melpa.milkbox.net/#/pivotal-tracker) or by cloning the repo.

## Initial Setup

Before using the tracker you must customize your pivotal API key. You can
obtain the key from the [Profile](https://www.pivotaltracker.com/profile)
link in the Pivotal Tracker web application. Once you have the key, customize it.

Do it via **customize** mechanism:

<kbd>M-x customize-group RET pivotal RET</kbd>

or set it manually:

```el
(setq pivotal-api-token "your-secret-token")
```

## Usage

### Projects View

* <kbd>M-x pivotal</kbd> will display a list of your current projects
* <kbd>RET</kbd> or <kbd>.</kbd> will load the current iteration for the given project
* <kbd>n</kbd> and <kbd>p</kbd> move between lines, like dired mode

### Current Project View

* <kbd>t</kbd> toggles expanded view for a story. <kbd>Enter</kbd> also toggles this view
* <kbd>R</kbd> refreshes the view
* <kbd>L</kbd> list projects. displays the Projects View
* <kbd>N</kbd> will load and display the next iteration
* <kbd>P</kbd> will load and display the previous iteration
* <kbd>E</kbd> will prompt for a new integer estimate for that story
* **numeric prefix** + <kbd>E</kbd> will use that number for the estimate
**  example: pressing <kbd>2</kbd> followed by pressing <kbd>E</kbd> will assign a **2 pt** estimate for current story
* <kbd>C</kbd> will prompt for a new comment
* <kbd>S</kbd> will prompt for new status
* <kbd>O</kbd> will prompt for new story owner
* <kbd>T</kbd> will prompt for a new task
* <kbd>F</kbd> will mark the task (not the story) under the cursor as finished
* <kbd>+</kbd> adds a new story

## Issues & Feature Requests

Development is [hosted on github](https://github.com/jxa/pivotal-tracker)

## Licensing

This program is free software; you can redistribute it and/or
modify it under the terms of the GNU General Public License as
published by the Free Software Foundation version 2, or any later version.

This program is distributed in the hope that it will be useful, but
WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
General Public License for more details.

For a copy of the GNU General Public License, search the Internet,
or write to the Free Software Foundation, Inc., 59 Temple Place,
Suite 330, Boston, MA 02111-1307 USA
