#Voter Sim

Create a REPL-driven voting simulation program. It should work like this.

This is the main menu:

`What would you like to do? Create, List, Update, or Vote`
When I type Create:

`What would you like to create? Politician or Person`
When I type Politician:

`Name?
Party? Democrat or Republican`
When I type Person:

`Name?
Politics? Liberal, Conservative, Tea Party, Socialist, or Neutral`
When creating something is done, return to the main menu.

When I type List, output a list of all the created characters.

List
* Politician, Marco Rubio, Republican
* Voter, Juha Mikkola, Socialist
When I type Update, allow me to update a character.

Update

//: Name?
//: Marco Rubio

//: New name?

//: New Party?    # if a politician
//: New Politics? # if a voter
When I type Vote, start the simulation. This simulation can happen in any number of ways, here is one example:

First, run a campaign. Every politician should visit every voter and do a stump speech.

If a politician is a Republican, he has a
- 90% chance of convincing a Tea Party voter to vote for him
- 75% chance of convincing a Conservative voter to vote for him
- 50% chance of convincing a Neutral voter to vote for him
- 25% chance of convincing a Liberal voter to vote for him
- 10% chance of convincing a Socialist voter to vote for him

If a politician is a Democrat, he has a
- 90% chance of convincing a Socialist voter to vote for him
- 75% chance of convincing a Liberal voter to vote for him
- 50% chance of convincing a Neutral voter to vote for him
- 25% chance of convincing a Conservative voter to vote for him
- 10% chance of convincing a Tea Party voter to vote for him

After every stump speech
- puts a comment from the Voter indicating whether or not he has changed his mind
- if the Voter is also Politician, puts a comment condemning what was said in the speech

The campaign is complete when every voter has listened to at least one stump speech. Feel free to use an alternative strategy for campaigns and stump speeches.

When the campaign is over, tally up the votes and determine the winner.

Politicians are also Voters, but they will always vote for themselves.

Some Notes:
- You should practice using TDD to help you manage this large project.
- If you complete the entire assignment, get creative with your reach goals!