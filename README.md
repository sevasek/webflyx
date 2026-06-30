# WebFlyx 🎬

> "You thought you knew what the web was capable of. You were *wrong*."

A fictional streaming-service catalogue built as a hands-on **Git fundamentals exercise** (Boot.dev course). The "product" is a curated movie list available on floppy disk — while supplies last.

## What This Repo Demonstrates

| Git Concept | Where to See It |
|---|---|
| Basic commits & messages | Commit history A → N |
| Creating & switching branches | `add_classics` branch |
| Merging branches | Commit F, D726da1 |
| Pull requests | PR #1 (`sevasek/add_classics → main`) |
| `.gitignore` | `.gitignore` (commit M) |
| Directory structure | `quotes/`, `secure/` |
| Multiple file types | `.md`, `.csv`, `.html`, `.txt` |

## Repository Structure

```
webflyx/
├── contents.md          # Index of the collection
├── titles.md            # Current movie titles (with genre links)
├── classics.csv         # Classic movies (title, director, year, genre, rating)
├── ratings.md           # Leaderboard ranked by personal rating (out of 10)
├── guilty_pleasures.md  # Secret favourites (tell no one)
├── advert.md            # Marketing copy
├── advert.html          # Rendered marketing page
├── genres/
│   ├── adventure.md     # Adventure movies
│   ├── comedy.md        # Comedy movies
│   ├── drama.md         # Drama movies
│   ├── horror.md        # Horror movies
│   ├── romance.md       # Romance movies
│   ├── sci-fi.md        # Sci-Fi movies
│   └── thriller.md      # Thriller movies
├── quotes/
│   ├── dune.md          # Memorable Dune quotes
│   └── starwars.md      # Memorable Star Wars quotes
└── secure/
    └── passwords.txt    # ⚠️ Example of what NOT to commit
```

## The Collection

**Classics** (from `classics.csv`):
- The Princess Bride (1987) · The Goonies (1985) · The Breakfast Club (1985)
- Monty Python and the Holy Grail (1975) · Willow (1988) · Psycho (1960)

**Featured Titles**: A River Runs Through It · Fight Club · 12 Years a Slave · The Big Short · 12 Monkeys · The Curious Case of Benjamin Button

**Guilty Pleasures** (classified): The Notebook · Sharknado · Troll 2 · and more

## Key Lessons Illustrated

- **Never commit secrets** — `secure/passwords.txt` exists purely to demonstrate why `.gitignore` matters and what _not_ to do in a real project.
- **Branching workflow** — the `add_classics` branch shows a clean feature-branch → PR → merge cycle.
- **Commit discipline** — alphabetically sequenced commits (A → N) make it easy to trace how a repo evolves step by step.

## 🚀 Roadmap & Future Releases

| Priority | Feature | Description |
|---|---|---|
| ✅ High | Genre tagging | Add `genres/` directory with markdown files per genre; each movie links to its genre |
| ✅ Medium | Rating system | Extend `classics.csv` with a `rating` column and a `ratings.md` leaderboard |
| Low | Search script | A simple Python or shell script to grep the collection by title, director, or year |

## Running Locally

No build step needed — this is plain markdown and CSV. Clone it and browse with any text editor or markdown viewer:

```bash
git clone https://github.com/sevasek/webflyx.git
cd webflyx
# View the collection
cat contents.md
cat classics.csv
```

## Learning Resources

- [Boot.dev Git Course](https://www.boot.dev/courses/learn-git) — the course this repo accompanies
- [Pro Git Book](https://git-scm.com/book/en/v2) — comprehensive free reference
- [GitHub Docs: About pull requests](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests)

---

*Available on Floppy Disk. While supplies last.*
