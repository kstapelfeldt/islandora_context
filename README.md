# Islandora Context

Provides a set of [Context](https://dupal.org/project/context) "conditions" and "reactions" for Islandora objects. Use cases are welcome.

## Introduction

This module provides the following Context conditions:

* Collection membership: Define a set of collections; if the current object is a member of a collection in this set, the condition is triggered.
* Object namespace: Define a list of PID namespaces; if the current object's namespace is in this list, the condition is triggered.
* Object relationships: Define a statement stored in RELS-EXT; if the current object's RELS-EXT contains the relationship, the condition is triggered.
* Keywords in datastream: Define a DSID and a list of keywords; if any of the keywords in the list is found in the designated datastream, the condition is triggered.

It also provides one Context reaction:

* Insert text into Islandora object's display: Lets you define the text of a message (such as a rights statement) which is appended to an Islandora object's display. The HTML containing the message is themeable.

## Requirements

[Context](https://dupal.org/project/context)

## Installation

Install as usual, see [this](https://drupal.org/documentation/install/modules-themes/modules-7) for further information.

## Usage

Install and configure. To create a context, go to Structure > Context and click on Add. The conditions and reactions listed above will appear in their respective sections of the context form.

One common use of Context is with the accompanying [Context Reaction: Theme](https://drupal.org/project/context_reaction_theme) module. As stated on that module's project page, "you can only use Context Reaction: Theme with the 'Sitewide' or 'Path' conditions." This means that the conditions defined by Islandora Context won't initiate theme switching. To switch themes for collections or for members of a collection, you should use the Path condition to match for namespaces or PIDs. You may also want to check out the [Themekey](https://www.drupal.org/project/themekey) module, althought it doesn't currently have any Islandora-specific functionality.

## Troubleshooting/issues/feedback

Feedback and use cases for Islandora-specific "conditions" and "reactions" are welcome.

* [Islandora Group](https://groups.google.com/forum/?hl=en&fromgroups#!forum/islandora)
* [Islandora Dev Group](https://groups.google.com/forum/?hl=en&fromgroups#!forum/islandora-dev)

