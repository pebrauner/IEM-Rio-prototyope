# IEM Rio 2026 — rdy.gg Prototype

hey, quick heads up before anything else:

**i'm not a front-end dev, i'm not a programmer, i'm not a designer.** my coding experience is limited. i just had ideas about stuff i love (CS2, esports, live content) and wanted to put them somewhere visual so people could actually *see* what i was thinking instead of trying to explain it in a doc.

---

## what is this

this is a prototype for an **IEM Rio 2026 event hub** on rdy.gg. basically the idea is: what if rdy had a dedicated page for a CS2 major that actually had everything in one place? scores, bracket, teams, editorial, the onsite feed, shows — all of it, not scattered around.

there are two HTML files here:

### 1. `IEM_Rio_2026_Hub_Prototype_rdy_gg v4.html`
the main event hub. think of it as the homepage for the tournament on rdy.gg. it has:

- **live match section** — shows the current match happening with a round-by-round activity feed. like, you can see how each round ended (bomb exploded, defuse, elimination), who had what economy, player stats per map. basically everything happening live in one card
- **map veto** — shows how teams picked and banned maps before the match
- **watch live button** — direct link to stream, right there in the match card
- **groups & bracket** — standings table for group stage + the playoff bracket
- **schedule** — all matches for the event, past and upcoming
- **teams section** — each team is a collapsible row, click it and player cards expand with individual stats
- **editorial coverage** — news, articles, analysis pieces for the event
- **on-site feed** — the sidebar with real content coming from people actually at the venue (photos, quick updates, that kind of thing)
- **shows & podcasts** — rdy's own shows tied to the event (like a hub within the hub)
- **event info** — location, format, prize pool, dates — the basics

navigation has tabs at the top (Overview, Schedule, Standings, Teams, Maps, News) and a simplified mobile version too (Match Data, On-Site Feed, Schedule).

---

### 2. `Roles_Analysis_Prototype_rdy_gg.html`
this one goes deeper. it's a **match analysis page**, built around a specific matchup (FURIA vs Team Spirit as the example). the idea is a page dedicated to breaking down a match with actual tactical depth, not just the score.

tabs inside this page:
- **Overview** — live match feed + round timeline + economy panel + player stats
- **Roles & System** ⭐ — **this is the most important part of this whole prototype.** a table showing each player's role on both CT and T side (entry fragger, support, lurker, etc.) and their overall system. what makes it special is that it integrates rdy's own metrics and calculations directly into the page — which is exactly what we always wanted to do. this isn't just pulling data from somewhere else, it's our own stuff displayed in a way that actually makes sense for CS2 analysis
- **Performance** — per-player performance breakdown
- **Economy** — how teams managed money across rounds
- **Head-to-Head** — historical record between the two teams, map stats, previous meetings

---

## what's the overall idea / objective

rdy.gg covers esports and i think for events like a CS2 major, there's a real opportunity to go way deeper than just showing scores. the goal of this prototype is to explore what a **proper event hub** could look like — something that works for the casual viewer who just wants to know "who's winning" but also has enough depth for someone who actually plays the game and wants to understand *how* teams are playing.

the roles & system analysis piece is especially something i don't see done well anywhere. it's the kind of content a CS brain actually cares about.

---

## scope of the prototype

- **static only** — nothing here is connected to live data. everything is hardcoded as a visual mockup
- **placeholder numbers** — all the stats, ratings, and values you see in tables are made up. i don't have access to the actual databases, so the numbers are just there to show how the layout would work, not to be accurate
- **desktop-first** — there's basic mobile support but it wasn't the focus
- **CS2 only** — built specifically for IEM Rio, the nav has a sport switcher (CS2 / Valorant) but only CS2 is fleshed out
- **not a final design** — this is just to communicate ideas, not ship something

---

## assets

the `/assets` folder has placeholder images organized by type: editorial, event, feed, players, teams. just enough to make it look real.

---

that's it. if something looks weird or broken, it probably is — again, not a programmer. but hopefully the ideas land.
