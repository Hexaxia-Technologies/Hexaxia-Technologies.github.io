---
layout: post
title: "Our Open Source Has a New Home: Hexaxia Labs"
date: 2026-05-12 13:00:00 -0400
categories: announcements
tags: [open-source, hexaxia-labs, hexcms, hexops, github]
author: Hexaxia Technologies
excerpt: "We've moved our open source projects into their own GitHub organization. Same tools, same MIT license, one front door: Hexaxia Labs."
---

We've moved our open source projects into their own home. Going forward, the public tools we build live at [github.com/Hexaxia-Labs](https://github.com/Hexaxia-Labs).

Same tools. Same MIT license. Same people maintaining them. What changes is that they now have a front door of their own instead of sitting alongside the rest of our work.

## Why a Separate Home

When we started open-sourcing the tools we built for ourselves, they lived wherever it was convenient. That was fine when there were one or two of them. It stopped being fine once there were a handful, each with its own roadmap, its own issues, its own contributors.

A few things pushed us to give them a dedicated organization:

**A real front door.** If you want to see everything we've put out in the open, you should be able to land on one page and see it. Not dig through a profile that mixes public projects with internal repos and client-adjacent work.

**Their own audience.** These tools speak to developers, which is a different audience than the rest of what we do. Giving them a dedicated home means that someone who finds one of them can immediately see what else we've put out, without sifting through anything unrelated.

**A signal.** Spinning something out into its own org is a small act of commitment. It says these projects aren't experiments we'll quietly delete. They're things we maintain, in the open, with issues you can file and roadmaps you can read.

## What's There Now

Three projects have moved over, with more on the way.

**HexOps.** A dashboard for managing multiple local development servers from one place. Start, stop, and restart dev servers. Watch CPU, memory, and disk in real time. Stream logs per project. Check Git status, scan for vulnerabilities, batch your dependency updates, deploy to Vercel. If you've ever had a dozen terminal tabs open just to keep track of what's running, this is for you. [github.com/Hexaxia-Labs/hexops](https://github.com/Hexaxia-Labs/hexops)

**HexCMS.** A Git-based headless CMS. Write content as Markdown in a Git repo, push, and your site rebuilds, with database sync underneath so builds stay fast no matter how much content you have. Full-text search, tags, authors, structured data for SEO. [github.com/Hexaxia-Labs/hexcms](https://github.com/Hexaxia-Labs/hexcms)

**HexCMS Studio.** A local editor for Markdown content repositories. Visual WYSIWYG editing on one side, real Git version control on the other. Edit with a rich editor, fill in your frontmatter through a form, then commit and push without leaving the app. [github.com/Hexaxia-Labs/hexcms-studio](https://github.com/Hexaxia-Labs/hexcms-studio)

All three started the same way: we needed something, the thing didn't exist or didn't work the way we wanted, so we built it. Then we used it long enough to trust it, and put it out.

## What This Means If You Use Our Tools

Not much, honestly, and that's the point.

- **The GitHub URLs changed.** If you've starred or watched a repo under the old organization, GitHub redirects, but it's worth re-pointing your bookmarks at [github.com/Hexaxia-Labs](https://github.com/Hexaxia-Labs).
- **The license didn't change.** Everything stays MIT. Use it, fork it, modify it, ship it in something commercial. Your data stays yours.
- **Issues and pull requests still work the way they did.** File bugs. Request features. Send PRs. We review them. All skill levels welcome.
- **Watch the organization** if you want to know when something new shows up.

## What's Next

More of our internal tooling is heading to Hexaxia Labs over the coming weeks. We'll write about the ones worth writing about. We're not going to manufacture announcements for every minor release, but when something useful goes public, you'll hear about it here or by watching the org.

## Why We Bother

We're an IT consultancy. We could keep every tool we build to ourselves. We don't, for a few reasons that haven't changed since we [started this blog](https://www.hexaxia.tech/blog/hexaxia/why-were-blogging):

Good tools should be shared. If something made our work simpler, it might do the same for someone else. Open source builds trust. You can read exactly how we build things, which beats us telling you we're good at it. And community makes tools better. The contributors who file bugs and request features catch things we miss and surface use cases we never imagined.

It's also just good business, and we'd rather say that out loud than pretend otherwise. Developers who use our tools remember us. When they need help with infrastructure, security, or automation, we're already a known quantity. We'd rather earn that attention than buy it.

If any of these tools are useful to you, [Hexaxia Labs](https://github.com/Hexaxia-Labs) is the place to find them. And if you need more than tools, [that's what we do](https://hexaxia.tech).

**[Talk to us](https://hexaxia.tech/contact)**
