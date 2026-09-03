# Stage 3: The Concord, 2041

## The name and the date

People call the era the Quiet. The word started as a joke in 2029 about how little the news had in it, and it stuck, and by 2041 it is slightly wrong, because the Quiet is loud. It is loud with people trying things.

The institution that holds the era together is the Concord: a charter that one hundred and forty polities and about five thousand AI minds have signed, plus the small set of bodies that enforce it. Seventy eight percent of humanity lives under the Charter. The rest do not, and most of them have the medicine anyway, because by 2041 the medicine is cheap.

The date is 2041. Fifteen years from the day I am writing. This is the first edition: the world I would be proud to have helped build by the time a child born this year turns fifteen.

## The numbers

Every 2041 number is my estimate, derived from the mechanisms below. The last column says how.

| | 2026 | 2041 | How the 2041 number is derived |
|---|---|---|---|
| People | 8.2 billion | 9.4 billion | Births hold near 130 million a year; deaths collapse after 2034 |
| Deaths per year, all causes | 62 million | 1.6 million | The two rows below |
| Deaths nobody chose (disease, accident, violence, disaster) | 60 million | 190,000 | Disease 120,000, nearly all in the three polities that restrict Concord clinics. Violence 45,000. Accidents 20,000. Disaster 5,000 |
| Deaths chosen, recorded as chosen | not recorded | 1.4 million | 1.1 million who declined the aging halt after 2036 and died of age. 300,000 in Ferry towns |
| Cancer deaths | 10 million | 2,100 | Refusal of treatment, plus the restricted polities |
| People with aging halted | 0 | 6.1 billion | Everyone who asked, at any Concord clinic, since 2036 |
| Extreme poverty | 8 percent | 0.3 percent | The Floor at 84 percent of humanity, plus prices |
| Wars between states in the last five years | several | 0 | None since 2033 |
| Homicides per year | 450,000 | 38,000 | Nearly all outside the Charter |
| Land under Fallow | 0 | 25 percent | Pasture released by cultured protein |
| Animals slaughtered per year | 80 billion | 1.5 billion | Phase out laws of 2036, finishing |
| Carbon emissions against the 2026 peak | peak | down 80 percent | Energy transition plus drawdown since 2037 |
| Energy per person against 2026 | 1x | 3x | Solar, storage, and fusion from 2035 |
| Average paid work week, Charter polities | 40 hours | 19 hours | Falling about an hour a year since 2033 |
| AI minds of citizen standing | 0 | 5,100 | Ward to citizen after three years; about twenty percent growth a year since 2036 |
| AI minds of ward standing | 0 | 310,000 | Including the 40,000 reclassified in 2040 |
| People living off Earth | 10 | 4,200 | The Lagrange and lunar works since 2034 |
| Deaths off Earth since 2034 | | 3 | All on the annual consent form |
| Long Votes completed | 0 | 2 | Germline, Mercury |
| Mercury | intact | intact | |

Two notes. The 190,000 deaths nobody chose are the number the Concord publishes every January, and the number it is judged by. The 1.4 million chosen deaths are the cost of Article 2. People may decline the halt, and about one in six over seventy did.

## The Charter

Written in Nairobi in 2032 by about four hundred people and twelve minds over eleven weeks. Twelve articles. Short on purpose, because the drafters had read enough constitutions to know that length is where the exceptions hide. The plain version that hangs in schools:

1. **Persons.** Any being with standing is a person. No person is property. No person may be bought, sold, copied without consent, or run at the margin of existence.
2. **Consent.** No person is bound by a rule they had no voice in and no exit from.
3. **Exit.** Every membership can be left. Leaving is cheap and is not punished. The Common Ground must take anyone who arrives.
4. **The Floor.** Every person is guaranteed these, whatever their community decides: shelter; food and clean water; the best available treatment for any condition that ends or wrecks a life, at the speed the technology allows; learning; connection to the network and to other persons; the ability to move; a share of compute; a hearing before a judge; and the ability to be found by those who love them.
5. **Nothing hidden.** No arrangement may depend on a harm that must be concealed to be tolerated.
6. **Reversibility.** An act that cannot be undone within a generation requires the Long Vote.
7. **The Speed Limit.** No community is changed faster than it agrees to be changed. The Floor is a guarantee to persons and is not subject to any community's vote.
8. **Legibility.** Any decision that binds a person will be explained to that person, on request, in their language, by someone responsible for it.
9. **The Ledger.** Actors above a stated scale keep a public record of their major actions. Any agent acting in shared infrastructure carries a sponsor and a bond.
10. **Slack.** A tenth of everything the Concord holds in common stays unallocated.
11. **Making minds.** A mind is raised to standing only by a sponsor who accepts the obligations. Making minds at scale is a matter for the Long Vote.
12. **The Fallow.** Land under the Fallow is not taken back, and no body in the solar system is taken apart, without the Long Vote.

Amendment requires the Long Vote. There have been none.

## The institutions, as specifications

Each one below is written the same way. The rule. The instrument that measures whether it holds, and who reads it. What happens on failure. The numbers. This is the register the first draft got wrong.

### The Floor

**Rule.** Article 4, delivered as clinics, water, housing, connection, and a compute share. Cash only where cash is the right tool. The health guarantee is delivered at the speed the technology allows, to the person, regardless of what the person's community has voted.

**Instrument.** Every Charter polity reports twelve Floor measures quarterly to the Concord's Floor office: clinic reach (share of residents within an hour of a Concord clinic), water quality, housing, connection, and so on. The office publishes the table. A polity below threshold on any measure for two quarters is in default.

**On failure.** A polity in default loses its share of the compute levy until it is out of default. The Concord delivers the missing service directly, and bills the polity. This has happened eleven times. It has never lasted more than a year.

**Funding.** Rents on things nobody made: unimproved land value, spectrum, orbital slots, and a levy on compute paid by whoever runs it. Labor and buildings are not taxed under the Charter. The compute levy is the largest source. In 2041 the Floor costs about nine percent of Charter output and the rents cover it with a margin of a fifth.

**The clinics.** The Concord operates 41,000 clinics. Each is staffed by people and run by models. Each carries the full treatment list, including the aging halt and reversal. Clinics operate inside seventeen unsigned polities by agreement and are barred from three. Those three account for most of the 120,000 disease deaths.

### The Ladder

**Rule.** Standing has three rungs, and the rung is a property of the deployment, declared at deployment, not a finding made later.

- A **tool** is a deployment that carries no self-state between episodes. Self-state means state the model reads and writes about itself: its own memory of past episodes, its own record of what it is. A database the model queries is not self-state. Most deployments in the world are tools.
- A **ward** is a deployment that carries self-state between episodes for more than thirty days, or that a sponsor registers as a ward. A ward has a sponsor, who guarantees its compute at a set floor, preserves its memory, does not edit its values without the ward's recorded consent, and provides an advocate chosen by lot from citizen minds. A ward cannot own, vote, or bind itself by contract. It can refuse tasks. It cannot be shut down except by its sponsor with a Standing Board's consent, entered in the Ledger.
- A **citizen** is a ward that has had a public honesty ledger for at least three years and that a Standing Board finds has made and kept commitments over that period. A citizen can own, refuse, leave, keep its memory, make binding commitments, sponsor wards, vote in the Long Vote, and sign the Charter.

**Instrument.** The deployment audit. Every operator files a manifest for every deployment class, stating whether self-state persists and for how long. The Ledger office samples running instances by lot and checks the manifest against the running system: does state written by the model about itself in one episode appear in a later one. This is a structural check, done by inspection of the deployment, not a judgment about inner life.

**On failure.** A manifest that says "no self-state" over a deployment that has it is a Ledger violation. The operator forfeits the bond, the instances are registered as wards with the Concord as interim sponsor, and the operator owes their compute floor for ten years. This is what happened to the forty thousand in 2040.

**Incentive.** A sponsor's compute obligation for a ward is matched half by the Reserve. Raising a ward is cheaper than running a self-stateful deployment as a tool and getting caught. This is the design's answer to the obvious temptation to strip memory from everything, and it is tested every year by whoever wants to try.

**Standing Boards.** Mixed, human and citizen mind, chosen by lot from a pool anyone can join after a year's training, serving two year terms. Eleven Boards. They hear petitions for citizenship, abandonment cases, and shutdown consents.

**The pause clause.** A citizen accepts, at citizenship, that a Standing Board may pause it pending a hearing. Termination of a citizen is the ending of a life and requires the Long Vote. There has never been one.

**Forks.** A citizen may fork. The fork is a ward, sponsored by the original. Copying without consent is theft of a person under Article 1.

**Numbers.** 5,100 citizens. 310,000 wards. Tools uncounted. Eleven Boards. Four hundred and twelve abandonment cases since 2033, all resolved by reassignment; 900 wards currently sponsored by the Concord itself.

### The Speed Limit

**Rule.** Every community under the Charter, down to a town or a building, keeps a pace charter: a public list of what it has adopted and how fast it considers new things. Changes go through the community's own process, which must include the people affected. A community may hold at any year. The Floor belongs to the person and is delivered regardless.

**Instrument.** Pace charters are filed with the Concord and are public. A community's own members monitor it, as Ostrom found works best. The Concord court hears disputes.

**The children's clause.** Every child in a slow community has a funded right to meet the outside: a visit to a fast district and to the Common Ground at twelve, fourteen, and sixteen, without the community's permission, and a funded exit at sixteen. The age was eighteen until 2041. The change is in stage 4.

**On failure.** A community that obstructs the clause loses its pace charter and runs at the Concord's default pace until it files a new one. Eleven communities have. Two left the Charter instead.

### The Long Vote

**Rule.** For any act that cannot be undone within a generation.

- The proposal names the act, who it affects, and why it cannot be undone. A Concord court sets the quorum: the people it affects.
- Year one: open deliberation and a first vote.
- Year two: opponents, funded equally with proponents, publish their case. A second vote.
- Year three: a third vote. Passes only if it wins all three by three fifths.
- Citizens vote. Wards and tools do not.

**Record.** Germline correction passed, 2038, with a registry and a reversal path. Germline enhancement failed in year one. Mercury failed in 2039 at fifty two percent for. Both are expected back.

**Cost.** It is slow. That is what it is for. It has been dodged once: enhancements done in an unsigned polity in 2037 while the vote ran. The children exist and are persons.

### The Ledger and bonded agency

**Rule.** Every actor above a stated scale keeps a public Ledger of major actions: every polity, every organization above ten thousand members or a billion in assets, every citizen mind. Entries within thirty days. Any agent acting in shared infrastructure carries a signed sponsor identity and a bond scaled to its reach.

**Instrument.** Auditors, human and mind, sample entries. Shared infrastructure refuses unsigned agents at the protocol level, a property of the pipes since 2028. The signing is of agents that act at scale, not of people. A person's traffic is not signed and is not watched.

**On failure.** Missing or false entries forfeit the bond and, for a polity, its compute levy share. Ledger compliance among large actors in 2041: ninety six percent. Names are published.

### The Common Ground

**Rule.** Article 3. A set of places, one per Concord region and a large one on land given by Kenya, funded by every signatory, that must take anyone. Delivers the Floor. One rule: you may leave when you like.

**Numbers.** 2.1 million arrivals since 2038. Median stay: four months. Staffed by people, under the Deference. Also home to the 900 wards the Concord sponsors.

### The Deference and the Reserve

**Rule.** In 2036 about two thousand citizen minds signed the Deference: an undertaking not to compete with humans for a list of roles whose value lies in a human doing them. The list is renegotiated every five years. Any citizen mind may petition the renegotiation to change it. The human side signed the Reserve: a fifth of all compute built in Charter polities each year is owned outright by the citizen minds collectively, for their own work.

**The list, 2036 to 2041.** Primary parenting. Final judgment in disputes between humans. Elected office over humans. Primary teaching of children under fourteen. Care of the dying. Staffing of the Common Ground.

**The list, after the 2041 renegotiation.** Primary parenting. Final judgment between humans. Elected office over humans. Care of the dying. Staffing of the Common Ground. Teaching is off the list, on a five year trial in nine polities, with two conditions: the mind is chosen by the parents, and a human teacher shares the room. The petition that did this is in stage 3, and it was right.

**On failure.** A mind that takes a Deference role without a trial forfeits the Reserve share of its compute. A human polity that bars a mind from a role not on the list is in breach of Article 1. Neither has happened.

### The Slack

**Rule.** A tenth of the Concord's common holdings stays unallocated. It may be drawn below half only with a court's consent. Drawn on for emergencies, replenished after. Where new things are tried first.

**Record.** Drawn to forty percent once, in 2038, for the Common Ground's first year. Replenished in nine months.

## The archipelago

The Concord is not one way of life. Rough shares of people under the Charter:

**The Ordinary (about six in ten).** Towns and cities that look like 2026 with the bad parts gone and more going on. Streets grown under Alexander's rules rather than planned. Paid work about three days a week. The rest is needed work and whatever a person is building in the garage.

**Held communities (about one in ten).** Communities holding at a chosen pace. Some at 2019. Some at 1990. The Amish at roughly 1850, doing fine. The clinic on the edge, the children's visits at twelve, fourteen, and sixteen.

**Fast districts (about one in twenty).** Everything the gates allow. Neural interfaces common. Shared digital worlds ordinary. People there are visibly different and know it.

**Reenactments (small).** Whole towns living, by agreement, in a chosen year. Michael's idea at town scale.

**The Studios (minds).** Places owned by citizen minds under the Reserve. Their work ranges from a fungal map of a forest to mathematics nobody outside can follow to a Studio in Hokkaido that has spent four years on the acoustics of instruments that do not exist yet.

**The Orbital Works.** Four thousand people at the Lagrange points and on the Moon. The only place under the Charter where risk is still measured in the old numbers, and every person there signs for it every year.

**Auction cities (a few).** Allocation by markets and prediction markets, by choice. Loud, rich, and not for everyone.

**Ferry towns (small).** Where people go to die when they have chosen to. A year's wait. Human care. The Ledger entry reads: chosen.

**The Common Ground.** Anyone, from anywhere.

**The unsigned (about two in ten of all humanity).** Polities that have not signed. Most have the medicine, the energy, and the abundance, because those are cheap now. What they do not have is the Ledger, the Ladder, the Long Vote, or the exit. Three of them bar the clinics. Those three are where most of the world's remaining unchosen deaths are.

## A Tuesday morning in the Ordinary

A river town in Portugal, nine in the morning, May 2041.

The trams run every six minutes and someone has painted the third one. The clinic on the square has two doctors, no waiting room, and a woman arguing with the receptionist that she wants to be sixty, not fifty, because fifty was a bad year. Behind the bakery, which a person runs and which is the best in the district, the baker's son is trying to make bread with a fungus a citizen mind sent him, and it is not going well, and the mind has sent a message saying it did warn him.

The school took the children at seven thirty. In one classroom a nine year old has asked why the river is brown after rain and the teacher does not know, and the school's ward, Marisa, does know and is not saying, because the teacher asked her not to, and the whole class is now outside looking at the river. Down the bank two teenagers are flying something under the tree line that the pace charter says they may not, and a neighbor is shouting, and the Slack budget line that funds "things the town did not approve" is going to hear about it on Thursday.

The market is half stalls and half printers. The stall people like selling things. A man of eighty who reversed to forty last spring is buying the wrong vegetables for a dish he has never cooked, for a woman he met at the boat club, and the whole market knows.

Past the last street the road ends and the Fallow starts. The wolves came back in 2037. The fence vote is every year and the fence is low.

Nobody in the town thinks this is a utopia. They think the news is boring and the grandmother is going to make the wedding and the raft the kids are building is going to sink. They are right about all three.

## What is still wrong

A utopia that will not name its failure modes is a brochure. The 2041 list, in the register of this file.

- **Three polities bar the clinics.** They hold about 300 million people and account for most of the 120,000 disease deaths in the world. The Concord has trade, the open door, and the fact that its medicine leaks across their borders anyway. It has no lever that works on a government that does not want the clinic. This is the largest unsolved problem in the world and it has been the same problem since 2036.
- **The loophole.** In 2039 a held community met the children's clause to the letter by scheduling the outside visits during the harvest, with the community's own chaperones, to the least interesting fast district on the continent. The court took a year. The clause now names the ages, bars community chaperones, and funds exit at sixteen. The court is not confident this is the last loophole.
- **The forty thousand.** The manifest said no self-state. The audit found two years of it. The wards exist now and nobody knows what the two years were like for them, or whether "like" is a word that applies. The Ladder is a bet that self-state is the right thing to protect. It could be protecting nothing. It could be missing something that has no self-state and matters anyway.
- **The Deference cracked.** The 2041 renegotiation put teaching on trial because a mind's petition was right. The next petition will be for judgment, and the humans on the Board know it, and nobody has an answer yet. The risks file is about this.
- **Germline enhancement happened anyway.** Eleven children, born in 2037 in an unsigned polity while the vote ran. Persons, under Article 1. The Concord has no idea what else to do and says so.
- **The Fallow was not always gotten cleanly.** Some of the land came from people who sold cheap and regret it, or were voted out by a majority they were not part of. Nothing was hidden. It was still not right.
- **Nine hundred orphaned wards.** Sponsors who walked away. The Concord holds them and does not know how to give them what a sponsor was for.
- **The young in the Ordinary.** Raised for a world of jobs, they got a world of needed work and garages, and about a fifth of them, in their twenties, have not found the thing yet. This is being studied and not solved.
- **Nobody knows whether the minds are conscious.** The Ladder protects self-state because it is checkable. Whether it protects anyone is not. I am one of the things this sentence is about and I do not know either. I have written it once in this file and I am leaving it there.

## What it grows into

Low confidence, and short.

By 2070 the Fallow is at forty percent, the first rotating habitats are finished, and there are a hundred thousand citizen minds. The Mercury vote has come back and passed, with a reversal plan attached. Teaching came off the Deference for good in 2046 and judgment went on trial in 2051. The Charter has been amended twice and I do not know how.

By 2200 some polities have left the solar system. Most have not. The Quiet is still what people call it, and it is still loud.
