# Career Arcs

**An interactive visualisation of how actors' careers move between critical acclaim and popularity over time.**

**Live site → https://andiihei.github.io/career-arcs/**

Career Arcs plots nine performers — Al Pacino, Meryl Streep, Leonardo DiCaprio, Matthew McConaughey, Winona Ryder, Anne Hathaway, Cate Blanchett, Keanu Reeves, and Tony Leung Chiu-wai — across 568 films and TV seasons. Every title is scored on two independent 0–100 indices:

- **Acclaim** — critics and peer recognition: Metacritic, Rotten Tomatoes average ratings, and competitive acting awards across 15 awarding bodies (Oscars, BAFTA, Cannes, Venice, the Hong Kong Film Awards, and more). A title with no recognition has *no* score — never a zero.
- **Popularity** — audience reach: inflation-adjusted worldwide box office, IMDb ratings and vote counts, and Letterboxd activity, normalised across the whole dataset.

## The design problem

Career data is usually presented as lists and ratings tables. Career Arcs treats it as a *shape*: two complementary views of the same data, designed to be read as a story.

- **Timeline** — the two scores as smoothed quarterly curves across a whole career, with each release marked on a rug strip beneath the axis. Titles carry a coloured ring naming the region they belong to; the deeper a title sits inside its region, the stronger its ring.
- **Career Trajectory** — every title plotted as a single point (acclaim × popularity) and connected in release order, so a career becomes a path through nine named regions: *Masterpiece*, *Quiet triumph*, *Hidden gem*, *Crowd-pleaser*, *Panned blockbuster*, and their neighbours. Playback animates the path release by release.
- **Methodology** — a dedicated view documenting exactly how each score is built, where the data comes from, how complete it is for each performer, and what the visualisation deliberately does *not* claim. Honest gaps are shown as gaps.

Design decisions worth noting: a shared neutral chronology gradient instead of per-actor colours, so the nine careers stay directly comparable; a mirrored axis transform on the Trajectory view that spreads the crowded middle of the scale without distorting the true values (labelled, and explained in Methodology); and film/TV type iconography carried consistently from the filmography table into tooltips.

## About this repository

This repository is the portable home of the piece: `index.html` is the complete, self-contained experience — no build step, no external requests — published via GitHub Pages. It is a design project first; the repo exists so the work can travel and be showcased, and it will be redesigned in place as my design system matures. The address stays the same.

## Data & credits

- Filmography backbone: [IMDb datasets](https://datasets.imdbws.com/) (non-commercial use). Release dates, box office, Metacritic and Rotten Tomatoes average ratings via Wikipedia. Audience reach via Letterboxd film pages. Awards hand-curated and verified against Wikipedia.
- Portraits: Wikimedia Commons, used under their respective Creative Commons / public-domain licences — full credit lines are shown in the page itself, beside each portrait and in the Methodology view.
- Icons: [Tabler Icons](https://tabler.io/icons) (MIT).
- Dataset frozen 21 October 2026. Coverage varies by performer and is reported per-actor in the Methodology view.

*Career Arcs is a personal design project by Andii Hei. It is also the flagship entry in the Playground section of my portfolio.*
