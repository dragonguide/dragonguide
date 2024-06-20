---
title: Architecture
description: 
published: true
date: 2024-06-20T08:05:18.949Z
tags: 
editor: markdown
dateCreated: 2024-06-19T20:17:50.647Z
---

# Resilient "Hydra" Architecture
Dragon Guide is not the first site of its kind, as there have been many other sites aiming to catelogue information and history about draconity. The problem is that most of these sites are no longer around. There are many reasons a site could be going down. For example, the owner might no longer be able to maintain the site, the hosting provider might be going out of business, data loss has occured or the underlying technology becomes obsolete. In order for Dragon Guide to become a serious repository that will be able to serve its information to many generations into the future, we need a comprehensive strategy. To this extent, we came up with a so-called "Hydra Architecture", the many aspects of which we will explain below.

<figure>
  <img src="/hydra-architecture.jpg" alt="Screenshot of Dragon Vision"/>
  <figcaption>Even if one head is not able to, there will always be several other heads to give the information forth.</figcaption>
</figure>

## Back-ups and archives
A hard drive that failed, a hack or a piece of software that failed is enough to lose all data. That is why back-ups are important, but they are also very hard to get right. Storing back-ups in the same physical location as the original data is unwise in case of a fire or natural disaster. However, with multiple back-ups in different locations, there is still the risk of being hacked. And what about all the metadata, such as which people contributed to pages and which changes they made?

To address all these potential pitfalls, we came up with a distributed back-up strategy. The idea is that as many varying back-ups are used so that the short comings of any one particular strategy are adequately addressed by other strategies. For example, the Wayback Machine is able to retain a snapshot of the site that looks and feels just like the original site, but the actual content can be hard to navigate and extract. A different back-up strategy like GitHub is good for retaining textual data and keeping a precise history of edits that have been made, but falls apart when trying to view the website in its original form. Combining all these strategies is what allows the entire history and content of Dragon Guide to be accessible far into the future, even if something were to happen to the main site.

Lastly, it is important that at least some of these back-ups are publically accessible. If we force everyone to access our content through our website, that becomes a single point of failure. And though the maintainer of the site might be around to restore one of their many back-ups, if they aren't for any reason, that data still becomes lost to the public. This is exactly what public archives prevent. They provide a way for users to easily make their own copies of the site. With enough of these public archives around, and with enough people making copies of these, the content on Dragon Guide will always remain around even when the site ceases to operate and the owner is unable to restore or release their own back-ups.

### Official Archives
Official archives are back-ups that are maintained by the Dragon Guide team.

- GitHub
	Includes textual content, files and media. It is [publically accessible](https://github.com/dragonguide/dragonguide).
- GitLab
	Includes textual content, files and media. It is [publically accessible](https://gitlab.com/dragonguide/dragonguide).
- Wayback Machine
	Periodically takes snapshots of the website. Anyone can request a new snapshot by using the [Save Page Now service](https://web.archive.org/save). Make sure to enter `dragon.guide` as the URL and select "Save outlinks" for a complete snapshot. In the future, we aim to automate this process. It is [publically accessible](https://web.archive.org/dragon.guide).
- On-site Back-up
	A back-up of the site on the website host, on a different hard drive. Currently being looked into. It will not be publically accessible.
- Jottacloud
	Currently being looked into. It is not known whether it will be publically accessible.
- Archive.org
	Currently being considered. It would be publically accessible.

### Community Archives
Community archives are back-ups that are maintained by third-parties. If you would like to start maintaining one yourself, please let us know so we can list it here. There are currently no community archives.

## Future-proof storage format
All content on the website is saved in a standard format. Technology advances at a rapid pace, so to make sure our content will be easy to access in the future, we need to decouple our content from any underlying software as much as possible. There are many different kinds of software out there that a web administrator could use to set up a wiki, but in our case we had to pick one with resiliancy as a top priority.

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

## Licensing and legality
Though content may be ressiliant on a technical level, any wisdom contained on this site still risks being lost if it cannot be spread around. To encourage and enable this, all content (except where otherwise noted) is licensed under an open license (which one has yet to be determined). Though we will do everything in our power to keep the site up until the heat death of the universe, an open license will give anyone the power to take up the torch in case something were to happen.

## Site owner succession
In the future, we aim to have a clear plan in place to continue on the website even when the owner is no longer able to maintain it. 