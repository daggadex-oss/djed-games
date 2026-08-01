---

## title: "Game Building Playbook — Tools & Process for Djed's Games" date: 2026-07-30 tags: \[djed, fatherhood, game-design, development\] status: Active

# Game Building Playbook

A living record of the toolkit and process for building games for Djed — same format as the Rituals & Practices doc, because this is the same kind of thing: a repeatable system, not a one-off project. The goal isn't just DJed's Pixel Pals. It's the capability to keep making things like it.

---

## 1\. The toolkit — three tiers

Every game starts by picking one of these. Don't reach for more power than the idea needs.

| Tier | When to use it | Starter file |
| :---- | :---- | :---- |
| **Plain canvas** (what Pixel Pals is built on) | Small, focused game with a handful of entity types you fully control. No dependency, no CDN, works offline forever. | `djeds_pixel_pals.html` as the reference |
| **Kaplay** | Fast prototypes, game-jam-style experiments, an idea you want playable in an hour. Simpler API than Phaser, still gives you proper entities/components. | `starter-kaplay.html` |
| **Phaser** | The game has grown — many entities, physics, tilemaps, camera movement, sound, particle effects. Most complete toolkit, biggest community if stuck. | `starter-phaser.html` |

All three follow the same rule established with Pixel Pals: single HTML file, no build step, no npm install, drag onto Netlify Drop and it's live. Phaser and Kaplay load their engine from a CDN `<script>` tag rather than being "installed" in the traditional sense — that's a feature here, not a shortcut, since it means any future game stays just as easy to hand off and deploy as this one was.

---

## 2\. Pre-build checklist

Run through this before starting any new game idea — five minutes of thinking here replaces hours of rebuilding later. Distilled from Jesse Schell's "lenses" (*The Art of Game Design*) and the developmental-first approach already used elsewhere in Djed's rituals.

1. **What age/stage is this actually for, right now?** Not "eventually" — this visit, this month. Design the mechanic for the child in front of you.  
2. **What's the one core mechanic?** If you can't describe it in one sentence a stranger would understand, it's not focused enough yet.  
3. **What's the feedback loop?** Every action (tap, drag, hold) needs an immediate, obvious, delightful reaction — sound, color, motion, or all three.  
4. **What is this secretly teaching?** Name the real target (language, counting, sorting, emotional expression) even if it's invisible to him. If you can't name it, it's decoration, not a tool.  
5. **How long is a session?** Design for the attention span you actually have, not the one you wish you had.  
6. **What's the "hide the machinery" version vs. the "reveal it" version?** Per the staged pedagogy plan — most mechanics should work as pure delight now and become a visible "block" he can manipulate himself later.  
7. **What's the smallest playable slice?** One mechanic, working end to end, before anything else gets added.

---

## 3\. Reference shelf

**Repos**

- [Phaser](https://github.com/phaserjs/phaser) — full-featured 2D engine, CDN or npm.  
- [Kaplay](https://kaplayjs.com/) — simple component-based engine, CDN-friendly.  
- [ChrisChrisLoLo/tamagotchiClone](https://github.com/ChrisChrisLoLo/tamagotchiClone) — reference for care-mechanic loops (feed/play/bathe), relevant if a "feed your dino" layer gets added to Pixel Pals.  
- [OlgaSwan/petty](https://github.com/OlgaSwan/petty) — pixel-art virtual pet reference.

**Books**

- *The Art of Game Design: A Book of Lenses* — Jesse Schell. Source of the checklist above.  
- *Rules of Play* — Katie Salen & Eric Zimmerman. Systems-level formalization once a game's rules need to get more rigorous.  
- *Designing Games for Children* — developmental-needs-first framing for the actual audience.  
- *The Gamer's Brain* — Celia Hodent. Cognitive-science grounding for UX decisions.  
- *Resonant Games* (MIT Education Arcade) — for building real learning outcomes into mechanics rather than bolting them on.

---

## 4\. Game log

A running record of what's been built and what's queued — same spirit as the "Notes for Future Development" section in the Rituals doc.

**Built**

- *DJed's Pixel Pals* (2026) — plain canvas. Tap-a-creature pixel pet world with photo-to-sprite capture, voice recording, five random dino species with per-species idle animation, Djed-pillar start screen emblem.

**Queued ideas / not yet started**

- Feed-your-dino care mechanic (ties into the real-world food-variety ritual).  
- Simple sorting/counting minigame (math \+ logic target, per the original five-domain brief).  
- A visible "connect two blocks" mode for when he's older — the first reveal of the machinery underneath.

