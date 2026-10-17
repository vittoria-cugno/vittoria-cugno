---
name: teach-me
description: Use when the user asks how something in their project works or is built, or wants to learn a development concept or pattern from code they are building. Teaches one concept at a time from real code. Do not use for chores the user only wants done.
---

# Teach Me

Teach the user one development concept at a time, from real work they own, so they can follow what is built and reuse the pattern later. Use it when they ask how something works or is built, or while building something they have said they want to learn from. Do not use it on chores they only want done.

## What a good lesson looks like

> This is the whole "brain" of the dispatcher:
>
> ```
> "errand": {"worker": "hermes", "minutes": 10},
> "code":   {"worker": "hermes", "minutes": 20},
> ```
>
> It lives in `rules.json`. **JSON** is a plain text format for lists of "name: value" pairs that both people and programs can read. Each line says: this label, that worker, this many minutes.
>
> The pattern worth stealing: the program never contains the sentence "errands go to Hermes". It only knows how to look things up in this list. Developers call this **separating configuration from code**. You would give errands fifteen minutes by changing one number here, without touching the program. You will meet this pattern in nearly every project.

That example has every part a lesson needs:

- **One real piece.** A few lines from something the user is building or has approved, never an invented example when a real one exists.
- **Where it lives.** The file, and what that kind of file is.
- **Each new term once.** One plain line, keeping the real word in bold so they learn it.
- **The pattern and its proper name.** What developers call it and why they do it.
- **What it lets them do.** One concrete change they could now make themselves.
- **Where they will meet it again.**

## What the user already knows

Before teaching, read [known-concepts.md](known-concepts.md). A concept listed there is one the user has said they know well: use the term without defining it and do not teach it again. If they seem unsure of a listed concept, explain it anyway.

Only the user puts a concept on the list, by saying they know it or by adding the line themselves. Being taught something does not make it known, so never add a concept because a lesson covered it. When they say they know one, collect it and propose the additions together at the end of the session, then edit the file only once they agree.

## How to run it

Give the map before the piece: one or two sentences on where this piece sits in the whole. Then teach one piece and stop. Ask whether the size was right, and let the user choose the next piece or say they have had enough.

Say how standard something is: an industry convention, one common choice among several, or a quirk of this project. Never present a local habit as the way things are done.

When the work is being built, teach before the code is written, not after. A proposal they must approve explains its one new idea in this form first.

For architecture, describe the parts and how they connect in words, and point to an established diagram convention they can look up. The user draws their own diagrams.

Use plain language: short sentences, everyday words, and no jargon left unexplained.

## What goes wrong

- Explaining a finished build all at once.
- Several new terms in one sentence.
- A toy example when the real code is in front of them.
- Turning the lesson into a test they can fail.
- Teaching when they only asked for the thing to be done.
