---
title: "Game Summary Explained"
excerpt: "An explanation of all the real-time stats and graphs displayed in the ponziFarm game summary panel."
header:
  teaser: /assets/images/search-stats.png
categories:
  - Blog
tags:
  - instructions
  - stats
toc: true
---

<figure class="align-left" style="margin-top: 10px; margin-bottom: 10px; width: 150px;">
    <img src="{{ site.url }}{{ site.baseurl }}/assets/images/search-stats.png">
</figure>

The top of your **ponziFarm** game dashboard displays summary stats of the currently selected game. 

If the game is live, these stats will be updated in real time as players interact with the game. Once the game has run for a few days, this summary will also display interctive graphs of game statistics over the life of the game.

<figure>
    <a href="{{ site.url }}{{ site.baseurl }}/assets/images/game-summary-panel.png"><img src="{{ site.url }}{{ site.baseurl }}/assets/images/game-summary-panel.png" class="shadow"></a>
    <figcaption>Game Summary Panel</figcaption>
</figure>

## Game Number

Each game is numbered by blockchain, beginning with #0. Only one game runs at a time on each blockchain, and there will always be a gap between games to allow time for promotion. Between games, the dashboard will display a countdown and [referral link](/blog/referrals) to the next game, as well as a summary of the previous one.

## Game Status

Every ponziFarm game has a status. It will be one of the following:

* **Current** - The ongoing game, or the upcoming one if the previous game has ended.
* **Ended** - Just what it sounds like.
* **Queued** - Games scheduled beyond the current one. Note that game end dates are not known in advance, so a game is "scheduled" to begin a certain number of days after the end o fthe previous one.

Once the first game (i.e. Game #0) has ended, the **All Games** link will appear in the sidebar. This page displays the full list of games visible to you. Unless you are an admin user, you will not be able to see Queued games.

## Game Contract Link

The game header features a link to the current game's smart contract on the relevant blockchain scanner. Currently this doesn't tell you much, but soon we intend to add contract source code validation features that will help certify the integrity of the **ponziFarm** application.

## Game Stats

Game stats are grouped at the top of the Game Summary panel. Hover over a stat to see additional info and a link to documentation. Once charts appear, click a stat to see how it evolves over time.

### Game Time

<figure class="align-left" style="margin-top: 0; margin-bottom: 0;">
    <img src="{{ site.url }}{{ site.baseurl }}/assets/images/game-stat-game-time.png" class="shadow">
</figure>

This stat displays the game's accumulated run time. Hover over this stat to see the actual starting date & time. Also displays ending date & time, if the game has ended.

### Deposits

<figure class="align-left" style="margin-top: 0; margin-bottom: 0;">
    <img src="{{ site.url }}{{ site.baseurl }}/assets/images/game-stat-deposits.png" class="shadow">
</figure>

This stat displays a running count of player deposits to the game, as well as the total value of all deposits. Once the game has run for a few days, click the **Deposits** stat to see a graph of both metrics over time.

### Mgmt Fees

<figure class="align-left" style="margin-top: 0; margin-bottom: 0;">
    <img src="{{ site.url }}{{ site.baseurl }}/assets/images/game-stat-fees.png" class="shadow">
</figure>

This stat displays the running total of management fees paid as a percentage of each deposit to the game. 

We vary the management fee and other game parameters from game to game in order to optimize the player experience, but the rate is fixed once the game starts. All game parameters are displayed in the Game Rules panel at the bottom of every game dashboard.

**Management fees are paid out of the _game balance_, not out of your deposit!** If you withdraw your deposit before the game ends, you will receive the full amount of your initial deposit, with your daily rate of return compounded daily over your lockup period. 
{: .notice--info}

Once the game has run for a few days, click the **Mgmt Fees** stat to see a graph of this metric over the life of the game.

### Rebates

<figure class="align-left" style="margin-top: 0; margin-bottom: 0;">
    <img src="{{ site.url }}{{ site.baseurl }}/assets/images/game-stat-rebates.png" class="shadow">
</figure>

Deposits with longer lockup periods earn rebates, which are paid instantly back to the depositing account. 

Rebate rules are another parameter that varies from game to game. All game parameters are displayed in the Game Rules panel at the bottom of every game dashboard.

This stat displays a running count of the rebates paid out in the selected game, as well as their total value. Once the game has run for a few days, click the **Rebates** stat to see a graph of both metrics over time.

### Referrals

<figure class="align-left" style="margin-top: 0; margin-bottom: 0;">
    <img src="{{ site.url }}{{ site.baseurl }}/assets/images/game-stat-referrals.png" class="shadow">
</figure>

Every **ponziFarm** player gets a referral link to share with friends. When your friend makes a deposit to any game, you earn a referral fee, paid instantly to your crypto wallet. Referral fees are shared up the referral chain, so it pays to build a network!

Referral rates and upline cuts vary from game to game. These and other game parameters are displayed in the Game Rules panel at the bottom of every game dashboard.

This stat keeps a running count of the number of direct and indirect referral fees paid during the game, as well as their total value. Once the game has run for a few days, click the **Referrals** stat to see a graph of both metrics over time.

Click [here](/blog/referrals) to learn more about **ponziFarm** referrals!

### Withdrawals

<figure class="align-left" style="margin-top: 0; margin-bottom: 0;">
    <img src="{{ site.url }}{{ site.baseurl }}/assets/images/game-stat-withdrawals.png" class="shadow">
</figure>

This stat counts the number of game deposits withdrawn at maturity, following expiration of their respective lockup periods. It also keeps a running total of the value of these withdrawals, which includes accumulated daily returns.

Once the game has run for a few days, click the **Withdrawals** stat to see a graph of both metrics over the life of the game.

### Ejections

<figure class="align-left" style="margin-top: 0; margin-bottom: 0;">
    <img src="{{ site.url }}{{ site.baseurl }}/assets/images/game-stat-ejections.png" class="shadow">
</figure>

Some **ponziFarm** games permit **ejection**: an early withdrawal of your deposit, prior to the expiration of its lockup period. Ejection can prevent a total loss of your deposit, but it comes at a price: you forfeit all of your deposit's daily returns, and also pay a penalty out of your initial deposit value. So choose wisely!

Ejection availability and the penalty paid vary from game to game. Check the Game Rules panel at the bottom of every game dashboard to see these and other game parameters.

This stat maintains a running count of game ejections as well as the total value of ejections paid out, after accounting for penalties. Once the game has run for a few days, click the **Ejections** stat to see a graph of both metrics over time.

### Unsettled

<figure class="align-left" style="margin-top: 0; margin-bottom: 0;">
    <img src="{{ site.url }}{{ site.baseurl }}/assets/images/game-stat-unsettled.png" class="shadow">
</figure>

This stat counts the deposits that remain at risk in the game, along with a running total of their initial values. These numbers will increase as players make new deposits, and decrease as deposits are withdrawn or ejected from the game.

Pay close attention to these numbers when considering a deposit! Over time, players will either withdraw these unsettled deposits at maturity or eject them from the game, driving the game balance to zero and the game to an end!

Once the game has run for a few days, click the **Unsettled** stat to see a graph of both metrics over time.

### Balance

<figure class="align-left" style="margin-top: 0; margin-bottom: 0;">
    <img src="{{ site.url }}{{ site.baseurl }}/assets/images/game-stat-balance.png" class="shadow">
</figure>

This stat reflects the balance of value remaining in the game. This number will increase as players make new deposits, and decrease as deposits are withdrawn or ejected from the game and as players earn referral fees. Once the game balance drops to zero, the game ends and all remaining unsettled deposits are lost forever!

Pay close attention to the current game balance when considering a deposit. Compare it with the total Unsettled value to get a sense of how close the game is to a crash.

Once the game has run for a few days, click the **Balance** stat to see this metric graphed over time.