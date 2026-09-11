# python-gotcha-game

https://python-gotcha-game.netlify.app

<img width="1416" height="831" alt="Screenshot 2026-09-11 at 12 54 25" src="https://github.com/user-attachments/assets/08d40214-819c-440d-b015-753ede2e00b0" />

A self-contained, gamified web app for drilling Python fundamentals under timed exam conditions — built to prep Python skills assessments (career and education) 15 minutes, 2 minutes per question, no going back.

## Why this exists

Timed technical assessments reward pattern recognition and speed as much as raw knowledge. A lot of marks are lost to classic Python "gotchas" (mutable default arguments, is vs ==, shallow vs deep copy, generator exhaustion, late-binding closures) rather than genuine gaps in understanding. This tool was built to turn passive topic review into active, timed retrieval practice across the full breadth of a Python fundamentals syllabus, syntax and data types through to OOP, comprehensions, iterators, and the stdlib — so that by test day, none of it is a surprise.

## How it works

90 second timed drills — a Python code snippet is shown, you work out the output under time pressure, then reveal the answer and self grade
Reveal first grading — see the correct output and explanation before marking yourself right or wrong, so every question reinforces the concept regardless of outcome
Smart question selection — the picker prioritises topics with fewer attempts first (so nothing goes untested by chance) and cycles through every question in a topic before repeating any, guaranteeing exposure to the full easy-to-hard range
Topic mastery tracking — per-topic accuracy bars (Shaky / Getting there / Locked in) persist across sessions, so weak spots are visible at a glance
Daily + all-time stats — today's session resets independently from lifetime score and mastery data, so a "reset" never wipes long-term progress
Readiness goal — a configurable target (e.g. 95% overall accuracy, minimum reps per topic) that flags when every topic has been drilled enough, at high enough accuracy, to genuinely trust the number
Streaks & badges — lightweight gamification to keep repetition engaging over a multi-day prep sprint

## Topics covered

Basics & variables, data types & casting, booleans & operators, lists & tuples, sets & dictionaries, control flow (if/else, match, loops), functions & range, iterators & stdlib modules (math, json, re), string formatting, None & regex, match/dates, slicing, comprehensions, OOP fundamentals and deeper OOP (inheritance, polymorphism, encapsulation, classmethods, properties, inner classes) — plus a dedicated cluster of the highest-yield "gotcha" concepts: mutable default arguments, is vs ==, shallow vs deep copy, generator exhaustion, and closures/late binding.

## Tech

Single-file HTML/CSS/vanilla JavaScript — no build step, no framework, no backend. Progress is saved to the browser's localStorage, so it persists across sessions on the same device without needing an account or server.

## Running locally

Clone the repo and open index.html directly in a browser — that's it.

bash
git clone https://github.com/<your-username>/python-drill-game.git
cd python-drill-game
open index.html

## Deployment

Currently deployed as a static site via Netlify. Any static host (GitHub Pages, Vercel, Netlify) works identically since there's no server side component.

## fyi 
As long as you're on the same browser, on the same device, a normal refresh won't touch your stats so you can track your progress over time 👍🏽😌
