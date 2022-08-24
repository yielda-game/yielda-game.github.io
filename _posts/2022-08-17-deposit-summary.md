---
title: "Deposit Summary Explained"
excerpt: "An explanation of all the real-time stats and graphs displayed in the ponziFarm deposit summary panel."
header:
  teaser: /assets/images/deposits.png
categories:
  - Blog
tags:
  - instructions
  - stats
toc: true
---

<figure class="align-left" style="margin-top: 10px; margin-bottom: 10px; width: 150px;">
    <img src="{{ site.url }}{{ site.baseurl }}/assets/images/depossits.png">
</figure>

Once you have deposited to a **ponziFarm** game, the game dashboard will display a list of your deposits to the game just below your [Player Summary](/blog/player-summary).

This list will track all of your deposits, giving your details of their performance as well as controls to let you withdraw your deposits at maturity or eject them from the game.

<figure>
    <a href="{{ site.url }}{{ site.baseurl }}/assets/images/my-deposits.png"><img src="{{ site.url }}{{ site.baseurl }}/assets/images/my-deposits.png" class="shadow"></a>
    <figcaption>Player Deposit List</figcaption>
</figure>

## Sorting

Your deposit list is sortable. 

By default, it is sorted by **Maturity**, with mature deposits (meaning ready to withdraw) at the top and the ones closest to maturity just below them. For clarity, in this view deposits that have already been withdrawn or ejected from the game will be sorted to the bottom of the list.

You  can also sort your list by **Creation**. In this case, the most recently created deposits will move to the top of the list, whether or not they have been withdrawn.

## Contract Link

Each deposit to a **PonziFarm** game is represented by a smart contract on the relevant blockchain. Each deposit in your list features a link to the deposit's smart contract in the relevant blockchain explorer. 

## Action Button

Each deposit in your list features a button that will withdraw the deposit at maturity, or eject it from the game if ejections are enabled and the deposit is not yet mature.

Don't waste any time using this button once your deposit matures! Remember, once the game balance hits zero, the game ends and all remaining outstanding deposits are forfeit, _whether or not they have already matured_. 

Don't lose your deposit just because another player was quicker on the draw!

## Deposit Stats

Each deposit in your list features stats that reveal the performance of that deposit.

### Deposited

This is the initial value of your deposit, and is the basis for calculating management fees, instant rebates, referral fees, and your daily returns.

Another way to think about it: this is the amount you initially placed at risk for this deposit.

### Lockup

This is the lockup period you chose for this deposit. The lockup timer starts as soon as you complete the deposit, so it will mature at the same time of day as the deposit was created.

### Daily Rate

This is the daily rate of return your deposit will receive at maturity, based on the lockup period you chose. This rate is compounded daily, so even a slightly higher rate can result in a much larger overall return!

### Rebate

This is the instant rebate you received, if any, at the time of your deposit. Note that this rebate _does not_ alter the basis for calculating your daily returns. It is effectively a grant out of the game balance, and serves to reduce the amount you have at risk for your deposit.

### Withdrew

This is the amount you actually withdrew from the game! 

Obviously this will be zero until you either withdraw or eject your deposit. If you withdraw your deposit at maturity, this amount will include your accumulated earnings on your initial deposit. If you ejected your deposit early, this amount will reflect your ejection penalty.

### Cleared

This is the net value you have secured from risk wit this deposit.

Initially, this value will be negative: the initial value of your deposit is completely at risk, less any instant rebate.

After withdrawing your deposit at maturity, ejecting early, or losing your deposit at game end, this number will reflect this deposit's final net profit or loss.
