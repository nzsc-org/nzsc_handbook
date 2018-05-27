# Learn by doing: Play NZSC
The best way to learn NZSC is to play.
In this chapter, we will guide you through your first game of NZSC as you play against the computer.

## Opening the web page
To begin, open [this link](https://nzsc-org.github.io/nzsc_single_player_web/?seed=0xbabecaf3).

> Note: The above link will not take you to the true NZSC site.
> Instead, it will take you to a "training wheels" site, that is pre-seeded.
> You don't need to know exactly what this means; We'll explain more at the end of this chapter.
> It's just important that you know that the above link will not take you to the true NZSC.

You should see the following on your screen:

```text
Choose a character:
    Ninja
    Zombie
    Samurai
    Clown
```

If you don't see any text on your screen, it means your browser doesn't support WebAssembly, so you should get a new browser (Google Chrome is recommended) or update your current one.

## Choosing a character
Every game begins with each player choosing a unique _character_.
As shown on the screen, there are 4 characters to choose from: Ninja, Zombie, Samurai, and Clown.

Let's choose Ninja.
To do this, type `Ninja` and press the Enter key.

Now the screen should say:

```text
...

Both of you chose Ninja, so you must repick.
You have picked Ninja 1 times.
Computer has picked Ninja 1 times.

Choose a character:
	Ninja
	Zombie
	Samurai
	Clown

```

It looks like computer has also attempted to choose Ninja.
In NZSC, each player must have a **unique** character. Since you and the computer picked the same character, both of you will have to repick.

This time, let's try choosing Clown.
To do this, type `Clown` and press the Enter key.

Now the screen should say:

```text
...

You chose Clown.
Computer chose Zombie.
As a result, neither of you gets a headstart.
The score is now 0-0.

Choose a booster:
	Backwards
	Moustachio
	No Booster
```

Yay! You have successfully chosen a character.
Next, let's choose a booster.

## Choosing a booster
After the players have chosen their character, they will each select a _booster_ (or choose No Booster, but this is nearly always disadvantageous for them).

There are 8 boosters, but each player can only choose between 2 of them.
A player's character will determine what 2 boosters they can choose from.

As shown on the screen, Clown's 2 boosters are Backwards and Moustachio.

Let's choose Moustachio.
To do this, type `Moustachio` and press Enter.

Now the screen should say:

```text
...

You chose Moustachio.
Computer chose Regenerative.
Let the battle begin!

Choose a move:
	Juggling Knives
	Acid Spray
	Nose
	Mustache Mash
	Big Hairy Deal
```

You have now successfully chosen a booster.
Next, let's choose a move.

## The move-choosing stage
We have now begun the longest stage of NZSC: choosing _moves_.

In this stage of the game, each player will choose a move, and depending on which two moves are chosen, one of the players will score a _point_.
This step is repeated until one player wins the game by reaching 5 points.

There are 28 moves, but each player can only choose from 5 of them.
A player's character and booster will determine what those 5 moves are, as explained below:

Every character contains 3 moves, and every booster contains 2 moves.
Together, they determine which 5 moves a player can choose from.

In our case, Clown has: Juggling Knives, Acid Spray, and Nose; Moustachio has Mustache Mash and Big Hairy Deal.
As a result, those 5 moves are the ones we are allowed to choose from, as shown on the screen.

## Let's choose some moves!
Let's choose Big Hairy Deal.
To do this, type `Big Hairy Deal` and press Enter.

The screen should now say:

```text
...

You chose Big Hairy Deal. Computer chose Regenerate.
As a result, the computer gets a point.
The score is now 0-1.

Choose a move:
	Juggling Knives
	Acid Spray
	Nose
	Mustache Mash
	Big Hairy Deal
```

Oh no! The computer's move (Regenerate) _wins_ against your move (Big Hairy Deal), so the computer scores a point.
Don't worry, though. The game is far from over!

Next, let's choose Juggling Knives.
To do this, type `Juggling Knives` and press Enter.

The screen should now say:

```text
...

You chose Juggling Knives. Computer chose Rampage.
As a result, you get a point.
The score is now 1-1.

Choose a move:
	Juggling Knives
	Acid Spray
	Nose
	Mustache Mash
	Big Hairy Deal
```

Yay! Juggling Knives wins against Rampage, so this time you score a point.

Next, let's choose Mustache Mash.
To do this, type `Mustache Mash` and press Enter.

The screen should now say:

```text
...

You chose Mustache Mash. Computer chose Rampage.
As a result, neither of you gets a point.
The score is now 1-1.

Choose a move:
	Juggling Knives
	Acid Spray
	Nose
	Mustache Mash
	Big Hairy Deal
```

Wait, the score is still the same.
What happened?

Well, it turns out that it is possible for moves to _tie_ against each other, meaning neither player scores point.
In our case, Mustache Mash ties against Rampage, so nobody scores a point.

Next, let's choose Nose.
To do this, type `Nose` and press Enter.

The screen should now say:

```text
...

You chose Nose. Computer chose Rampage.
As a result, the computer gets a point.
The score is now 1-2.

Choose a move:
	Juggling Knives
	Acid Spray
	Nose
	Mustache Mash
	Big Hairy Deal
```

Owch! The Rampage wins against Nose, so the computer scores another point.

Next, let's choose Big Hairy Deal.
To do this, type `Big Hairy Deal` and press Enter.

The screen should now say:

```text
...

You chose Big Hairy Deal. Computer chose Zap.
As a result, neither of you gets a point.
The score is now 1-2.

Choose a move:
	Juggling Knives
	Acid Spray
	Nose
	Mustache Mash
```

Notice anything different about our list of available moves?
Instead of having 5 moves to choose from, we only have 4!
Somehow, Big Hairy Deal suddenly disappeared.
Why?

Well, it turns out that Zap is a _destructive move_, meaning when a player chooses it as their move, their opponent's move is "destroyed" and can't be used for the rest of the game.

There are 2 destructive moves in NZSC: Zap and Acid Spray.

Notice that one of our moves is a destructive move: Acid Spray.

Let's give the computer a taste of its own medicine by choosing Acid Spray.
To do this, type `Acid Spray` and press Enter.

The screen should now say:

```text
...

You chose Acid Spray. Computer chose Gravedigger.
As a result, neither of you gets a point.
The score is now 1-2.

Choose a move:
	Juggling Knives
	Nose
	Mustache Mash
```

Whoa, we lost yet another move: Acid Spray.
How come?

This is because Acid Spray is a _single-use move_, meaning it can only be used once per game.

There are 3 single-use moves in NZSC: Zap, Regenerate, and Acid Spray.

Notice that every destructive move is also a single-use move.

Next, let's choose Juggling Knives.
To do this, type `Juggling Knives` and press Enter.

The screen should now say:

```text
...

You chose Juggling Knives. Computer chose Muscle.
As a result, you get a point.
The score is now 2-2.

Choose a move:
	Juggling Knives
	Nose
	Mustache Mash
```

Yay!
Juggling Knives wins against Muscle, so we score a point.

Let's choose Juggling Knives again.
To do this, type `Juggling Knives` and press Enter.

The screen should now say:

```text
...

You chose Juggling Knives. Computer chose Muscle.
As a result, you get a point.
The score is now 3-2.

Choose a move:
	Juggling Knives
	Nose
	Mustache Mash
```

We score another point, taking the lead!

Let's choose Juggling Knives yet again.
To do this, type `Juggling Knives` and press Enter.

The screen should now say:

```text
...

You chose Juggling Knives. Computer chose Rampage.
As a result, you get a point.
The score is now 4-2.

Choose a move:
	Nose
	Mustache Mash
```

We're on a roll!
Only one more point until we win.

But wait, how come Juggling Knives is not on our list of available moves?

This is because NZSC has a rule known as the _three-in-a-row rule_.
This rule makes it illegal to play the same move more than three times in a row.

As a result, since our previous three moves were all Juggling Knives, we will have to choose a different move this turn.

Let's choose Mustache Mash.
To do this, type `Mustache Mash` and press Enter.

The screen should now say:

```text
...

You chose Mustache Mash. Computer chose Rampage.
As a result, neither of you gets a point.
The score is now 4-2.

Choose a move:
	Juggling Knives
	Nose
	Mustache Mash
```

Now that we have broken our three-turn Juggling Knives streak, we are allowed to choose it again.

Let's choose Juggling Knives.
To do this, type `Juggling Knives` and press Enter.

The screen should now say:

```text
...

You chose Juggling Knives. Computer chose Rampage.
As a result, you get a point.
The score is now 5-2.

You won 5-2 (Obliteration).


Play again? y/N
```

Yay, we won!
Congratulations on completing your first NZSC game!

## Recap
You now know the basics of NZSC:

1. Each player chooses a unique character.
2. Each player chooses a booster.
3. Each player chooses a move, and the player with the winning move scores a point (there can be ties).
    1. Single-use moves can only be used once.
    2. Destructive moves will destroy the opponent's move, making it unavailable for the rest of the game.
    3. The same move cannot be chosen more than 3 times in a row.
4. First to 5 points wins.

## Debrief and Next steps
Now that you have successfully completed your first game of NZSC, we encourage you to play some "real" games against the computer (we'll explain what that means in a second).

To play a "real" game, open [this link](https://nzsc-org.github.io/nzsc_single_player_web/).
**It is different than the link we provided at the beginning of the chapter.**

During your next few games, we recommend you try different characters and boosters so you can get familiar with all 28 moves.

### What's the deal with this "real" and "training wheels" stuff?
Normally, the computer makes its decisions randomly.
This is important because if the computer made the same decisions every time, you would quickly get bored of playing the same thing over and over.

However, in this tutorial, we obviously knew what the computer was going to choose ahead of time.

This was made possible by pre-seeding.
If you are not familiar with pseudorandom-number-generators, you can just think of this as a way of forcing the computer to behave the same way every time.

You might have noticed the `?seed=0xbabecaf3` in the URL of the link we provided you (`https://nzsc-org.github.io/nzsc_single_player_web/?seed=0xbabecaf3`).
If you ever see a `seed=` in the URL, you know the game is pre-seeded.

While consistency is essential for writing a walk-through like this one, you'll probably want the computer to make random decisions during normal games, so make sure you go to [https://nzsc-org.github.io/nzsc_single_player_web/](https://nzsc-org.github.io/nzsc_single_player_web/).

**Do not go to the link we provided at the beginning of this chapter.**
That will take you to a pre-seeded version of NZSC.

The "real", random NZSC is located at [https://nzsc-org.github.io/nzsc_single_player_web/](https://nzsc-org.github.io/nzsc_single_player_web/).

### A couple things we skipped
We covered most of the rules of NZSC in this tutorial, but there are a few rules we didn't discuss.
It is not absolutely essential to read this section, as you could figure out most of it on your own if you play enough games.

#### Headstarts
Remember at the beginning of the game, just after you chose your character, how it said:

```text
...

You chose Clown.
Computer chose Zombie.
As a result, neither of you gets a headstart.
The score is now 0-0.

Choose a booster:
	Backwards
	Moustachio
	No Booster
```

You might have been wondering what the sentence about the headstart meant.

A headstart is just a point scored by choosing a certain character against another character.

Ninja gets a headstart against Samurai.

Samurai gets a headstart against Clown.

Clown gets a headstart against Ninja.

Zombie never gets a headstart, and no character gets a headstart against Zombie.


#### Penalties
What happens if you type something that's not a valid choice and press Enter?

In NZSC, invalid choices are penalized by _waits_.

Each player begins with 4 waits.
Every time they make an invalid choice, they lose some waits.
If their waits falls below 0, their waits will be set back to 0, and their opponent will score a point.

For the list of penalties and how many waits they deduct, consult [the reference](./reference.html#penalties).

#### Outcome table
If you ever want to know if one move wins against another, you can consult [the reference](./reference.html#outcome-table-truth-table).
