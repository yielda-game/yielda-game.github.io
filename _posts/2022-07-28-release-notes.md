---
title: "Release Notes"
excerpt: "A list of stable PonziFarm releases. Try us out on your favorite testnet!"
header:
  teaser: /assets/images/release.png
categories:
  - Blog
tags:
  - preview
toc: true
---

<figure class="align-left" style="margin-top: 10px; margin-bottom: 10px; width: 150px;">
    <img src="{{ site.url }}{{ site.baseurl }}/assets/images/release.png">
</figure>

ponziFarm is a work in progress! We add new features regularly. Whenever we have a stable release, we deploy it first to our supported testnets so we can shake it out before we update our production application.

Every release is numbered like this: **0.1.6**. In order, the three numbers are...

- **Major Version** (0). These don't happen very often.
- **Minor Version** (1). Indicates a breaking change to our Solidity contracts. In preview, we'll release a new site at a new URL with a fresh set of games. In production, we will let all current games play out and then migrate all games & deposits to an upgraded farm at the same URL before kicking off any new games.
- **Patch Version** (6). This is a front-end change. In preview, we'll provide a new link to the release, but it will retain all games, deposits, etc. from the previous release. In production, there will be no interruption. New features will just show up and start working.

**Not all releases are stable!** Consequently, expect gaps in the release versions listed here.

## [Current Preview](https://preview.ponzifarm.com)

The most recent preview of the PonziFarm platform (i.e. running on testnets) is always available at [preview.ponzifarm.com](https://preview.ponzifarm.com). 

**Warning:** The Current Preview may be slightly in advance of the most recent stable release. Translation: *it might not be stable!*
{: .notice--warning}


## [Release 0.1.6](https://preview-0-1-6.ponzifarm.com)

This release is preview-only. We've created a game on each supported coin, and their start times are staggered so you can see the countdown timers operating. You can make deposits and see both the overall game stats and the stats associated with your account.

You can't yet **withdraw** your deposits. (This is fully supported by the back end but not yet by the UI.) Consequently, games in this release won't go broke and end, so you'll only ever see one game per supported coin.

The player-specific stats are still rudimentary. More to come.

Next feature in the queue is the graph that displays the game status over time. This is actually pretty interesting: there will come a point during game play where withdrawals will exceed deposits. This signals the beginning of the crash, and you'll be able to SEE it coming. Hopefully your deposits will unlock before the crash actually arrives! 😉