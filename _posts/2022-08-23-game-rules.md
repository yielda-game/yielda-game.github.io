---
title: "Game Rules Explained"
excerpt: "PonziFarm game rules vary from game to game in order to optimize the player experience. Here is an explanation of each game parameter."
header:
  teaser: /assets/images/rules.png
categories:
  - Blog
tags:
  - rules
toc: true
---

<figure class="align-left" style="margin-top: 10px; margin-bottom: 10px; width: 150px;">
    <img src="{{ site.url }}{{ site.baseurl }}/assets/images/rules.png">
</figure>

Like any game, **ponziFarm** has rules.

Unlike most games, our rules are implemented as smart contracts. This creates a level of transparency and security you will never find in a bricks-and-mortar casino, much less any back-room poker game!

So play with confidence... and also with care. While the rules of **ponziFarm** can't be _broken_, they CAN be _exploited_. And players who figure out how to do that are going to play at a _very_ profitable advantage!

We hope you're one of them.

## General Rules

**ponziFarm is a GAME, not an INVESTMENT!** Some players will win big. Many will make a tidy profit. The rest will lose their deposits!

**ponziFarm is an exercise in game theory!** There is perfect transparency. Everybody knows the deal. Invite your friends help keep the game going! They will ALSO know the deal.

**Every ponziFarm game is alike!** Decide how much to deposit and how long to lock it up. Earn instant rebates and referral fees. The return on your deposit is compounded daily. If you withdraw your deposit before the game runs out of money, congrats! If not... GAME OVER.

**Every ponziFarm game is different!** We vary game parameters from game to game in order to optimize the player experience.

## Game Parameters

Every **ponziFarm** game is slightly different!

Each game has a number of parameters, which we vary from game to game in an effort to optimize the player experience. Once a game starts, its parameters are set in stone and can never be changed again!

See the Game Rules panel at the bottom of every game dashboard for a full list of the parameters set in that game.

<figure class="align-center" style="width: 384px;">
    <img src="{{ site.url }}{{ site.baseurl }}/assets/images/game-params.png" class="shadow">
    <figcaption>Game Paraameters</figcaption>
</figure>

### Minimum Deposit

Every deposit must be equal to or greater than the game's configured **Minimum Deposit**. 

Remember that each game is played in the gas currency of its respective blockchain. While we will vary the minimum deposit from game to game, in fiat terms it will almost always be under USD 100.

### Ejection

An **ejection** is the withdrawal of a deposit prior to the end of its lockup period.

Not all games permit ejection. When they do, there will be an associated **Ejection Penalty**: a percentage of the initial deposit value that is forfeit (along with accumulated earnings) when a player ejects a deposit from the game. 

### Management Fee

Every time a player makes a deposit, a **Management Fee** is subtracted from the overall game balance. This is how we finance and promote the game!

While management fees reduce the game balance, they do NOT affect the value of your deposit! On maturity, you can withdraw the _full initial value_ of your deposit, plus accumulated earnings!

### Referrals

Every new **ponziFarm** player gets a referral link to share with friends and on social media. This link is permanently connected with the crypto wallet you used to make your deposit.

When a friend clicks your link and makes a deposit, your wallet is permanently designated as their wallet's _upline_. From then on, every **ponziFarm** deposit from your friend's wallet will generate a referral fee, transferred instantly from the game to your wallet. The percentage of this fee is the game's **Referral Bonus**.

If your wallet _also_ has an upline, then this wallet will get a cut of the referral fee you received due to your friend's deposit. This pattern continues up the upline chain until the fee becomes smaller than the gas required to transfer it. The percentage of this cut is the game's **Upline Cut**.

### Daily Rates

Each deposit earns a rate of return that is compounded daily. This rate depends on the deposit's lockup period: the longer the lockup, the higher the daily rate. Daily compounding adds up quickly, so longer deposits can earn a _significantly_ higher overall return when they mature!

<figure>
    <img src="{{ site.url }}{{ site.baseurl }}/assets/images/lockup-vs-daily.png" class="shadow">
    <figcaption>Lockup Period vs. Daily Rate</figcaption>
</figure>

This curve is determined by five parameters:

* **Daily Min Rate** - The minimum daily rate paid to a deposit.

* **Daily Min Rate Lockup** - The game's minimum lockup period, which earns the **Daily Min Rate**.

* **Daily Max Rate** - The maximum possible daily rate paid by the game.

* **Daily Max Rate Lockup** - The shortest lockup period that earns the **Daily Max Rate**.

* **Daily Rate Scale Factor** - Higher values make this curve sharper, and lower ones make it smoother.

### Rebate Rates

Deposits with longer lockups earn a rebate paid instantly back to the wallet that made the deposit. The amount of this rebate increases with the length of your lockup.

<figure>
    <img src="{{ site.url }}{{ site.baseurl }}/assets/images/lockup-vs-rebate.png" class="shadow">
    <figcaption>Lockup Period vs. Instant Rebate</figcaption>
</figure>

Instant rebates _do not_ affect your deposit balance of your returns... but they _do_ affect the remaining game balance, so every instant rebate paid brings the game just a little closer to its final crash!

This curve is determined by five parameters:

* **Rebate Min Rate** - The minimum rebate rate paid to a deposit.

* **Rebate Min Rate Lockup** - The lockup period that earns the **Rebate Min Rate**. Can't be less than **Daily Min Rate Lockup**.

* **Rebate Max Rate** - The maximum possible rebate rate paid by the game.

* **Rebate Max Rate Lockup** - The shortest lockup period that earns the **Rebate Max Rate**.

* **Rebate Rate Scale Factor** - Higher values make this curve sharper, and lower ones make it smoother.
