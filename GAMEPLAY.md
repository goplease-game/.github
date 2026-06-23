# Game rules and how to play

1. This is a turn-based game on a hex board with deterministic combat.
2. Each player controls 6 units. Every unit has its own set of abilities: 1 basic attack, 3 unique active abilities, and 1 unique passive ability. 
3. Each active ability costs 1 AP (Action Point) to use. Each unit has 1 AP per turn, unless granted extra AP by another ability or game rule.
4. Each unit has movement points (MP) which determine how far it can move. A unit can move once per turn. Once moved — even less than its full MP — the unit loses all remaining MP and cannot move again this turn.
5. A unit can move and use abilities in any order, as long as it has not already moved or still has AP to spend.

---

# Gameplay

Each player has 6 units total, deployed in waves of 3 + 2 + 1 across the first three rounds.

The game loop runs in rounds. Each round consists of a **Play Phase** followed by a **Deploy Phase**. Since players have no units on the board at the start, Round 1 skips the Play Phase and goes straight to Deploy.

**Turn order** is determined by deployment order. As players alternate placing units, a shared queue is built: P1-unit1, P2-unit1, P1-unit2, P2-unit2, and so on. Units take turns in this fixed queue each round. If a unit dies, it is removed from the queue — which may result in two consecutive turns for the opposing player.

**Round 1 — Deploy Phase:** Players place their units into their designated deploy zone, alternating one unit at a time. Once the second player places their third unit, Round 1 ends.

**Round 2 — Play Phase → Deploy Phase:** Both players play their units in the order they were placed in Round 1. Each unit has its own turn during which it can move and use abilities. Once all units have taken their turn, each player deploys 2 more units, alternating as before. Once the second player places their second unit, Round 3 begins.

**Round 3 — Play Phase → Deploy Phase:** Players now have up to 5 units each and play them as in Round 2. Afterward, each player deploys their final unit. Round 4 then begins.

**Round 4 onward:** All units are on the board. There is no more Deploy Phase — the game continues with each unit taking turns. The player who eliminates all of the opponent's units wins.

---

# Action Points (AP) and Phantom Action Points (PAP)

Each ability costs 1 AP, and each unit has 1 AP on their turn. Some abilities can grant extra AP.

If a team has fewer units than the opposing team, it receives **Phantom Action Points (PAP)** — extra AP equal to the difference in unit count. For example: 5 vs 6 → 1 PAP; 4 vs 6 → 2 PAP.

PAP is a shared pool for the whole team. Any unit can spend it on their turn. Unused PAP resets at the end of each round.

---

# Impatience

To prevent stalling, starting from Round 10 each unit receives the **Impatience** buff at the start of its turn, permanently gaining +1 ATK. This stacks every round.