
## [[Charon or Kharon]]
> *The ferryman of the dead*, an NPC that can be found in some places, and will become some kind of "transportation" 

## Ultimate role
> to defeat boss "faster" need to unleash ultimate (no ultimate is possible but it takes longer)
> ultimate will become "mandatory" in the second region as the boss has a mechanics that can only be bypassed by using the ultimate from the boss of region 1

## ~~Unlocking ultimate~~
> ~~After unlocking the first ultimate (the deflect spirit's), the next ultimate can only be accessed / obtained by doing the relevant spirit story quest~~

## ~~Spirit story (==POSTPONED==)~~
> ~~Every spirit will has it's own story quest, doing it will reward player their ultimate and other stuff.~~

## ~~AEther core fragment~~
> ~~Part of the AEther core that contains memory, collecting these will change **==*the boss fight feels*==**~~

## Progression
> After defeating [[Naita Putri]], defeat the other bosses to unlock next story chapter. After defeating [[Mary Alderton]], the last boss (main antagonist) will be unlocked

## Contracting Spirit
> Defeating the boss will not instantly unlock them / make a contract them, player need an "item" that resonate with the boss to form a contract

## Room Area Reference & Example

| Room ID                | Overview                                                                       | Objectives                                                         | Encounter/Gameplay                                                       | Notes                                                                  |
| ---------------------- | ------------------------------------------------------------------------------ | ------------------------------------------------------------------ | ------------------------------------------------------------------------ | ---------------------------------------------------------------------- |
| **R1: Entrance Hall**  | Player entry point, first taste of the manor's state. Connects to R2 and OR1.  | Navigate to next area. Introduce **Falling Rock** hazard mechanic. | Minor enemies (Spike variants). Tutorial area for environmental hazards. | Ensure audio cues for rocks are clear. Art: Dim lighting, dusty ruins. |
| **R2: Gallery**        | Main connector space. Introduces the quest’s central mystery (lore pickup).    | Read Journal Page [Lore-A]. Proceed to R3.                         | Medium enemy encounter. Uses cover points.                               | Ensure lighting highlights the interactable Journal item.              |
| **R3: Library**        | Key puzzle room required to unlock the Boss Door access. Connects to R4.       | Solve book puzzle to find [Library Key].                           | Puzzle focused, minimal combat.                                          | Puzzle logic detailed in a separate PDD (Puzzle Design Document).      |
| **R4: Antechamber**    | Pacing room before the main fight. Introduces the specific boss weakness clue. | Traverse the room to the Boss Door. Avoid **Spike** traps.         | Environmental traversal challenge using **Spike** traps.                 | QA: Test collision with spikes extensively.                            |
| **R5: Boss Door Hall** | Short hallway leading to the Boss Room (BR1).                                  | Unlock door with [Library Key].                                    | None (Pacing hall).                                                      | Door mechanism requires [Library Key] item check.                      |

# Map Area
> Area within the same region will be interconnected with each other. (Player need to "walk" to change to another city).

# Yogyakarta Progression
> Linear progression, other area to explore will be unlocked after getting the first contracted entity. 
#### Memento
> Can be found around ==Area 1== before the boss room, ==Will trigger a dialogue or something similar explaining about it to be a requirement for an entity to be contracted==.

# Jakarta Progression
> Open from the start, there's no limitation on how to proceed with the area
#### Memento
> Can be found within ==Area 1==

# Hokkaido Progression
> Linear progression, exploration is limited until progressing the story
> ex. A1 -> A2 -> {A3, B5(locked until progressing more)} -> A4 -> B1 -> etc.
#### Memento
> Can be found within ==Area 3==

# Tokyo Progression
> Open from the start, there's no limitation on how to proceed with the area
#### Memento
> After defeating [[Saigyouji Yuyuko ( 西行寺 幽々子 )]], she will not require a "Memento" in order to have a contract with her, since she is a "special entity"

# Pakistan Progression
> Open from the start, there's no limitation on how to proceed with the area
#### Memento
> Can be found within ==Area 2==.

# London Progression

### [[Naita Putri]] 
> Linear progression, exploration is limited. Will unlock other area after completing her story / defeating her
#### Memento
> Can be found within her area
### [[Mairi Chattan]]
> Open from the start, the only locked area are ==St. Etheldreda’s RC Church==.
#### Memento
> Can be found after defeating her first phase

### [[Mary Alderton]]
> The last area within London, exploring this area will require all other exploration ability
#### Memento
> Can be found within her area, but heavily infested with other hostile entity around it.


---
Designing Metroidvania-style levels requires blending exploration, player ability progression, spatial memory, and rewarding discovery. The goal is a coherent map that invites backtracking with new abilities while maintaining pacing, readability, and varied challenges. Practical steps, patterns, and pitfalls follow.

1. Define core mechanics and progression loop  
    - Inventory of tools: list platforming moves, combat abilities, traversal tools (double jump, dash, grappling, wall-cling, morph ball, keys).  
    - Progression gating: decide which mechanics unlock new areas. Keep gates visible or hinted from earlier sections.  
    - Rewards loop: exploration → reward (ability, item, shortcut, lore) → new access → expanded exploration.
2. Start with a macro map  
    - Sketch a node-and-connection map of major regions (hub, 4–6 themed zones). Nodes = distinct gameplay sets and puzzles.  
    - Establish chokepoints: bottlenecks that require specific abilities to pass.  
    - Arrange verticality and layers: Metroidvanias thrive on stacked areas; use vertical shafts, concealed platforms, and layered corridors.
3. Design ability-driven sequences  
    - For each ability, create 3 canonical uses:
	- Progression use: unlocks previously inaccessible area.
	- Exploration use: reveals optional secrets/shortcuts.
	- Combat/puzzle use: introduces new enemy interactions or puzzles.
	- Keep abilities complementary and avoid redundant mechanics. Introduce abilities early in simple contexts; expand complexity later.
4. Gate placement and signposting  
    - Clear visual gates: doors, cracked walls, high ledges, currents. Make the required action visually intuitive.  
    - Subtle hints: framing, distinct tiles, lighting, enemy placement, or environmental cues that imply a needed ability.  
    - Avoid opaque gating: don't force tedious pixel hunts. If a gate is hidden, give a credible in-world hint.
5. Create loops and shortcuts  
    - Design shortcuts that persist after opening (doors, elevators, one-way passages). They reduce backtrack tedium and reinforce the sense of progress.  
    - Ensure loops feel rewarding: a long detour should reveal a meaningful reward or a fast route back to hub.
6. Pacing and difficulty curve  
    - Alternate high-intensity combat/platforming rooms with quieter exploration sections.  
    - Layer optional areas for skilled players: place harder platforming or timed sequences behind optional gates.  
    - Use encounter variety: combine small enemy groups, minibosses, environmental hazards, and puzzles to avoid repetition.
7. Secrets and optional content  
    - Scatter secrets that use mastered abilities in clever ways. Use gating depth: easy secrets near start, complex multi-ability secrets late-game.  
    - Make some secrets meaningful: alternate endings, powerful upgrades, lore, or unique traversal toys.
8. Spatial readability and player guidance  
    - Distinctive landmarks: color palettes, silhouettes, unique architecture for each region to help navigation memory.  
    - Map system: provide a concise in-game map that fills in explored space; include markers for points of interest (shops, save points).  
    - Breadcrumbs: audio cues, NPC dialogue, simple map annotations, or environmental leading lines to prevent getting lost.
9. Encounter and boss design tied to space  
    - Boss arenas should reinforce mechanics learned in the region and use unique spatial features (cover, vertical zones, hazards).  
    - Place minibosses where they make a gating or narrative beat, not purely as filler.
10. Iterate with playtesting and telemetry  
    - Early playtests for clarity: can players recognize locked progression cues? Are shortcuts effective?  
    - Telemetry to find choke points: track time spent, repeated deaths, abandoned paths.  
    - Polish: tune jump distances, camera framing, collision boxes, and enemy placement to reduce frustration.
11. Common patterns and templates  
    - Hub-and-spoke with connected shortcuts: central hub linking themed spokes encourages organic return paths.  
    - Layered gate progression: A → B → C where ability from B opens new path in A, creating interdependence.  
    - Metroid style (open regions, hidden power-ups) vs Castlevania style (more linear with branching side areas); mix as needed.
12. Avoid these pitfalls  
    - Excessive opaque gating: don’t require pixel-perfect guesses to progress.  
    - Over-cluttering with abilities: too many traversal options can make level design ambiguous.  
    - Punishing backtracking: remove repetitive fetch quests that add little fun.  
    - Uniform visual design: homogeneous rooms hurt navigation.
13. Example design mini-flow (practical)  
    - Create region A with a high ledge visible but unreachable.  
    - Place ability X (double jump) in region B beyond a locked door in C.  
    - Design a path: find hint of high ledge in A → encounter puzzle/mini-challenge in C → acquire X in B → return to A using shortcuts opened on route.  
    - Reward return with meaningful loot and a new route to region D that was previously blocked.
14. Tools and prototyping tips  
    - Block out levels in greybox to validate movement and sightlines before art.  
    - Use modular tilesets and placeholder objects for quick iteration.  
    - Implement quick-teleport tool for testers to check backtracking flows.

Design goals checklist (final quick-reference)

- Clear gating tied to satisfying ability uses.
- Distinct region identities and readable landmarks.
- Useful shortcuts and non-tedious backtracking.
- Varied encounters and optional secrets.
- Continuous player feedback via map, cues, and reward pacing.

Applying these principles produces maps that feel coherent, rewarding, and worth exploring: players experience discovery, growth, and meaningful returns to previously seen spaces.

---