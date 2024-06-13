---
title: Home
description: 
published: true
date: 2024-06-13T12:21:35.062Z
tags: 
editor: markdown
dateCreated: 2024-06-12T13:17:20.314Z
---

# Welcome to Dragon Guide
We aim to be a repository of information to the dragonkin community. Our goal is to set outselves apart in the following ways.

- A community-guided website to which anyone can contribute.
- A resistant artictecture to ensure content will stay around for decades to come.
- A modern, easy-to-navigate interface to help you find the things you need.
- A safe space to document and share your personal draconic experiences.

We are currently working on setting up the site, and adding as much content as possible. Contributions would very much be appreciated!

## Contributing
Contributions to the Dragon Guide are always welcome. The most useful thing to contribute would be wisdom, which comes in many forms. Whether you have something on the history of the dragonkin community, or are sharing your personal draconic experiences, your countributions are appreciated and will be kept safe. To get started, please read the contribution guide (this will be published at a later point).

Another way to contribute, would be through a donation. This will become an option at a later point in time. Any money we receive will be invested exclusively into the website. Examples would be server hosting, file storage and back-up strategies.

## Resilliant architecture
> "Time, the devourer of all things." - Ovid

Over the last few decades, we have seen the rise of many fantastic resources for dragonkin. Unfortunately, many of them have also gone offline for various reasons. Think of a hosting company going out of business, a site owner no longer able to do maintanace or older resources becoming hard to access due to the advancement of technology. With the help of a resilliant architecture, we aim to make Dragon Guide resistant to the obstacles of the future.

### Comprehensive back-up strategy
Back-ups are important, we all know that. But back-ups can also be hard to get right. Storing back-ups in the same physical location as the original data is unwise in case of a fire or natural disaster. However, with multiple back-ups in different locations, there is still the risk of being hacked. And what about all the metadata, such as which people contributed to pages and which changes they made?

To address all these potential pitfalls, we came up with a distributed back-up strategy. The idea is that as many varying back-ups are used so that the short comings of any one particular strategy are adequately addressed by other strategies. For example, the Wayback Machine is able to retain a snapshot of the site that looks and feels just like the original site, but the actual content can be hard to navigate and extract. A different back-up strategy like GitHub is good for retaining textual data and keeping a precise history of edits that have been made, but falls apart when trying to view the website in its original form. Combining all these strategies is what allows the entire history and content of Dragon Guide to be accessible far into the future, even if something were to happen to the main site.

#### Official Archives
Official archives are back-ups that are maintained by the Dragon Guide team.

- GitHub
	Includes textual content, files and media. It is [publically accessible](https://github.com/dragonguide/dragonguide).
- GitLab
	Includes textual content, files and media. It is [publically accessible](https://gitlab.com/dragonguide/dragonguide).
- Wayback Machine
	Currently being considered. In the meantime, the Wayback Machine can still elect to take snapshots of the site on its own. It is [publically accessible](https://web.archive.org/dragon.guide).
- Archive.org
	Currently being considered,
- BitBucket
	Currently being considered.
- SourceForge
	Currently being considered.

#### Community Archives
Community archives are back-ups maintained by the community. There are none as of yet. If you want to help us out, please contact the team.

### Open license
Though content may be ressiliant on a technical level, any wisdom contained on this site still risks being lost if it cannot be spread around. To encourage and enable this, all content (except where otherwise noted) is licensed under an open license (which one has yet to be determined). Though we will do everything in our power to keep the site up until the heat death of the universe, an open license will give anyone the power to take up the torch in case something were to happen.

### Standard formats
All content on the website is saved in a standard format. Technology advances at a rapid pace, so to content will be easy to access in the future, we need to decouple our content from any underlying software as much as possible. There are many different kinds of software out there that a web administrator could use to set up a wiki, but in our case we had to pick one with resiliancy as a top priority.

A lot of the wiki software available stores content in a unique fashion. This could be a database formatted in a specific way, or text using a special mark up language. However, what this does is tie the future of your content together with the future of the software you are using. To prevent this, we need to choose wiki software that can interface with a standard format, rather than use one of its own. This format needs to be easy to convert into other formats, and it should be compatible with a large range of different available software.

We eventually settled on Wiki.js, which makes use of Markdown under the hood. These files are simple text files with characters used to formatting. You may not have heard of it, but you might already be using it. Modern messaging platforms such as Discord, for example, use the Markdown syntax to allow you to make text `**bold**` or `*cursive*`. Because the syntax is so simple, and because they are just text files, the contents can be easily read with any text editor. This includes very simple ones such as Notepad.

```
# This is a header
And here is some normal, *cursive* and **bold** text. You can also embed code: `console.log("Hello dragon!")`. Let's also not forget [links](https://example.com) and images: ![A description for the visually-impaired.](https://example.com/image.png).

## This is a second level header
The header above is going to appear smaller than the first header at the top. To go down a header level, simply add another hashtag. Below is a list!

- # Header 1
- ## Header 2
- ### Header 3

You can also do numbered lists.

1. Hello!
2. Hallo!
3. Bonjour!

Or even a table!

| Feature     | Humans | Dragons |
|-------------|--------|---------|
| Mythical    | No     | Yes     |
| Drives Cars | Yes    | No      |
```

## Contact
For any inqueries, you may contact us by sending a mail to `contact@[domain of this website]`.  We aim to respond in 1 to 2 days.