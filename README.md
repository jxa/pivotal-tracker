# pivotal-tracker.el

Pivotal Tracker Mode provides a mode and functions for interacting with Pivotal Tracker through its API.
It is designed to give most of the functionality that is important to a developer.
It is not an attempt to replace every feature of the web interface.

## Installation

You can install via [marmalade](http://marmalade-repo.org/packages/pivotal-tracker) or by cloning the repo.

## Initial Setup

Before using the tracker you must customize your pivotal API key.
You can obtain the key from the 'My Profile' link in the Pivotal Tracker
web application. Once you have the key, customize it.

  M-x customize-group RET pivotal RET

## Usage

### Projects View

* M-x pivotal will display a list of your current projects
* RET or '.' will load the current iteration for the given project
* n and p move between lines, like dired mode

### Current Project View

* 't' toggles expanded view for a story. 'Enter' also toggles this view
* 'R' refreshes the view
* 'L' list projects. displays the Projects View
* 'N' will load and display the next iteration
* 'P' will load and display the previous iteration
* 'E' will prompt for a new integer estimate for that story
* numeric prefix + E will use that number for the estimate
**  example: pressing '2' followed by pressing 'E' will assign a 2 pt estimate for current story
* 'C' will prompt for a new comment
* 'S' will prompt for new status
* 'T' will prompt for a new task
* 'F' will mark the task (not the story) under the cursor as finished

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
