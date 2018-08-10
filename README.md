[![MELPA](http://melpa.org/packages/pivotal-tracker-badge.svg)](http://melpa.org/#/pivotal-tracker)

# Pivotal Tracker mode for Emacs

Pivotal Tracker Mode (`pivotal-tracker`) provides an Emacs based user
interface for [Pivotal Tracker](https://www.pivotaltracker.com).  It's
designed to give the most relevant functionality to a developer or pair
working on stories.

Please note, it's not an attempt to replace all the features of the
web interface.

## Installation

You can install via [MELPA](http://melpa.milkbox.net/#/pivotal-tracker)

## Initial Setup

Before using the tracker you must store your Pivotal API key somewhere Emacs
can find it. Because your API key is sensitive information it must not be
stored in clear text. Using the [auth-source] library Emacs can retrieve your
API key from `~/.authinfo.gpg`. Retrieve your API key from the
[Profile](https://www.pivotaltracker.com/profile) page and add a new entry in
`~/.authinfo.gpg`

```
machine pivotal-tracker.com password <your-api-key>
```

Once you've done that you'll be able to use `pivotal-tracker`.

## Usage

- <kbd>M-x pivotal</kbd> Start pivotal-tracker and view your current projects list

### Key bindings

- <kbd>p</kbd> Move up one line
- <kbd>n</kbd> Move down one line

#### Projects list view

- <kbd>RET</kbd> or <kbd>.</kbd> Load the current iteration for the given project
- <kbd>o</kbd> Open the given project in the default OS browser

#### Current project view

- <kbd>TAB</kbd> Toggles expanded/collapsed view for a story
- <kbd>g</kbd> Refresh the project view
- <kbd>^</kbd> Go back to your projects list
- <kbd>N</kbd> Go to the next iteration
- <kbd>P</kbd> Go to the previous iteration

- <kbd>s</kbd> **Story popup menu**
    - <kbd>e</kbd> Estimate
    - <kbd>c</kbd> Comment
    - <kbd>s</kbd> Set status
    - <kbd>o</kbd> Set owner
    - <kbd>t</kbd> Add task
    - <kbd>v</kbd> Check task

- <kbd>o</kbd> **Link popup menu**
    - <kbd>o</kbd> Open story in external browser
    - <kbd>l</kbd> Copy story URL to kill-ring / clipboard
    - <kbd>p</kbd> Open current project in the default OS browser

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
