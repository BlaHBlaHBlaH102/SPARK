---

# SPARK

---

SPARK one-page demo for SPARK startup.

By Viraj Shah  
Coded in HTML using Visual Studio Code 05.26.2026

---

## In order to view this demo, please do either of the following:

### Option 1: Open Locally
1. Download the repository ZIP
2. Extract all files
3. Open `index.html` in any modern web browser

### Option 2: Open Hosted Demo
Navigate to:

https://sparkvs.vercel.app

---

In event of downtime that might be a result of Vercel, please use Option 1.

---

## What to pay attention to

---
### 1. Dual-state progress bar
The progress bar in this app renders two things at once. It has a solid fill for current completion, and translucent fill for projected weekly progress if the user stays on track. The translucent portion changes color to amber if some backend math detects if the user is behind schedule. This is custom code.

### 2. localStorage persistence
Everything within this demo (checked tasks, accent colors, theme, streak, logs, name) survives a refresh because it's all stored within the html file. May not work in Vercel due to throttling on my account (I have lots of vercel project on the free tier) but certainly will work locally on html. The photos and logos are encoded in base64 (done with AI)

### 3. Splash animation sequence
This was pretty hard to get working. The logo closes its eyes and sticks its tounge out, shakes, and explodes with particles (I used Canvas for this). There's also a white flash and the logo swaps to a smiling face. Spark letters fly in from random places and then they bloom by adjusting Helvetica font weight. Logo swap is done by reassigning src in the middle of the animation.

### 4. 7-segment countdown + epoch uptime
The "Time Until Next Session" counter uses a special 7-segment font (not a system font). Hovering the card does a buzz animation and glow intensification. The footer uptime counter counts elapsed time since the project epoch (2026-05-23 19:00 ET). An epoch is a fixed time after which elapsed time is measured. For example, the epoch for the gregorian calendar (modern calendar) is the birth of Jesus Christ.

### 5. Version-gated login
There's a version key in localStorage that forces reauth whenever I bump up the version. Good for security/demos and stuff

### 6. Photo uploads in journal + daily log
Both the journal milestones and daily log entries take image uploads via FileReader API. Photos persist across sessions (see no.2). Journal entries with photos show inline previews and the full journal view takes all milestone photos and log entries by date and time

### 7. Suggested tasks column
Task suggestions are project-specific (robotic arm specific in this demo) and disappear from the suggestions list once added to the main task list. Clicking a suggestion turns it to a real task easily.

### 8. Streak system
Compares today's date string to last visit date in localStorage. Consecutive days add up to the streak, a gap of more than one day resets to 1. Streak count turns up the fire glow on the badge at one week and two weeks.

### 9. Zero-dependency single file
The entire app, Helvetica Neue (Roman, Light, Medium, Bold, Black), 7-segment font, all three logo variants, all CSS, all JS is ONE HTML file. Easy setup

### 10. Cool UI
I used the colors, logos and brand guidelines from the planning doc. Pretty cool right?

---

## What this page represents
This is the core dashboard, the most visited screen.

## Fonts & Assets

This demo uses Helvetica, a licensed font from Monotype.

Please see all of the files used below.

### Helvetica Files Used
- HelveticaNeueBlack
- HelveticaNeueBlackItalic
- HelveticaNeueBold
- HelveticaNeueBoldItalic
- HelveticaNeueHeavy
- HelveticaNeueHeavyItalic
- HelveticaNeueItalic
- HelveticaNeueLight
- HelveticaNeueLightItalic
- HelveticaNeueMedium
- HelveticaNeueMediumItalic
- HelveticaNeueRoman
- HelveticaNeueThin
- HelveticaNeueThinItalic
- HelveticaNeueUltraLight
- HelveticaNeueUltraLightItalic

---

This demo also uses the 7-Segment Display Font by torinak.com:

http://torinak.com/font/7-segment

This font is distributed under the SIL Open Font License.

---

## Logo Notes

I have modified the logos which you have provided me with using Canva to add two face versions.

These have been encoded using Base64.

Logo naming convention:
- `1` = faceless
- `2` = smiling
- `3` = sticking its tongue out
