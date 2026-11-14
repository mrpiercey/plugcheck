# The PLUG Check

**Plug in, blend, or unplug?** Four quick questions that help **elementary teachers** decide when classroom tech is worth it.

**Live:** https://mrpiercey.github.io/plugcheck/
**Printable:** [PLUG-Check.pdf](PLUG-Check.pdf) (2 pages, US Letter)

Inspired by Mary Mitchelson's Edutopia article, [Adapting Instruction as 1:1 Technology Access Shrinks](https://www.edutopia.org/article/adapting-less-tech-access-schools) (November 10, 2026), which is written from a middle school classroom. This tool is adapted for elementary, where tech use looks very different: centers and rotations, logins small hands can't manage yet, students who are still learning to read and write, and a room full of manipulatives, books, and pencils that often teach better.

## The mnemonic

| | Ask | Research behind it |
|---|---|---|
| **P** Purpose | Can you name the learning goal without naming an app? | Backward design (Wiggins & McTighe, 2005); TPACK (Mishra & Koehler, 2006) |
| **L** Leverage | What can students do with the tech that they can't do without it? | Four pillars of educational apps (Hirsh-Pasek et al., 2015); manipulatives (Carbonneau et al., 2013); handwriting (James & Engelhardt, 2012); paper vs. screen storybooks (Furenes et al., 2021) |
| **U** Universal | Can every student do it with minimal assistance from the teacher? | UDL Guidelines 3.0 (CAST, 2024); NAEYC & Fred Rogers Center (2012) |
| **G** Groundwork | Is the learning worth the minutes it takes to set up? | Short elementary blocks; AAP (2016) on balancing media use |

**Grade bands.** The app asks whether the lesson is for K-2 or 3-5 and changes its examples and suggested moves to match. All band-specific wording lives in the `STEPS` and `TIPS` objects in `index.html` as `{k2:'...', g35:'...'}`.

**How the call is made**

- **Plug in** if Leverage, Universal, and Groundwork are all a strong yes.
- **Unplug** if Leverage is "nothing new," or if Universal and Groundwork are both a flat no.
- **Blend** for everything else. Blend is the default and where most lessons land.

Purpose never sends a lesson to Unplug. A "not yet" just asks the teacher to write the goal first.

PLUG is a planning habit built on the research above. It has not been tested as a program on its own.

## What's in this folder

| File | What it does |
|---|---|
| `index.html` | The web app: the interactive check, the full flowchart, and the research notes. |
| `flow.css` | The flowchart styles, shared by the app and the printable. |
| `printable.html` | The source for the 2-page PDF. |
| `PLUG-Check.pdf` | The printable guide. Page 1 is the flowchart. Page 2 is a fill-in planner, a moves menu with room to add your own, and the sources. |
| `edu_bug.png` | The Edutopia "edu" bug. |

Nothing a teacher types leaves their browser. There is no sign-in and no tracking.

## Rebuilding the PDF

After editing `printable.html`, run this from the folder:

```
"/Applications/Google Chrome.app/Contents/MacOS/Google Chrome" --headless=new --no-pdf-header-footer --virtual-time-budget=8000 --print-to-pdf=PLUG-Check.pdf "file://$PWD/printable.html"
```

Or open `printable.html` in Chrome and print to PDF with margins set to None and background graphics on.

## Brand

Follows the Edutopia brand guidelines and shares its design system with [Class Jobs Maker](https://mrpiercey.github.io/edutopiaclassjobs/) and [Authentic or AI?](https://mrpiercey.github.io/aiedutopia/).

- **Fonts.** Poppins (the Google-safe stand-in for Gotham) for all body and interface text. Zilla Slab stands in for Museo Slab on headlines.
- **Colors.** Only the Edutopia palette. P is Tech Blue, L is Light Purple, U is Light Teal, G is Sunshine.
- **Electric Orange (#FF4C00)** is used sparingly: the edu bug and one primary button per screen.
- The printable is mostly white with light tints so it prints cleanly and leaves room to write.
