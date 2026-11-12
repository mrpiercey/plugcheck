# The PLUG Check

**Plug in, blend, or unplug?** Four quick questions that help teachers decide when classroom tech is worth it, built for schools where one-to-one devices are shrinking to a shared cart.

**Live:** https://mrpiercey.github.io/plugcheck/
**Printable:** [PLUG-Check.pdf](PLUG-Check.pdf) (2 pages, US Letter)

Inspired by Mary Mitchelson's Edutopia article, [Adapting Instruction as 1:1 Technology Access Shrinks](https://www.edutopia.org/article/adapting-less-tech-access-schools) (November 10, 2026).

## The mnemonic

| | Ask | Research behind it |
|---|---|---|
| **P** Purpose | Can you name the learning goal without naming a tool? | Backward design (Wiggins & McTighe, 2005); TPACK (Mishra & Koehler, 2006) |
| **L** Lift | What does the tech add that paper and talk can't? | SAMR (Puentedura, 2006); PICRAT (Kimmons, Graham & West, 2020); Triple E (Kolb, 2017); OECD (2015); Delgado et al. (2018) |
| **U** Universal | Can every student get to it and through it? | UDL Guidelines 3.0 (CAST, 2024); Pew Research Center (Anderson & Perrin, 2018) |
| **G** Go time | Is the learning worth the minutes it takes to get going? | Mitchelson (2026); ICAP (Chi & Wylie, 2014) |

**How the call is made**

- **Plug in** if Lift, Universal, and Go time are all a strong yes.
- **Unplug** if Lift is "nothing new," or if Universal and Go time are both a flat no.
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
