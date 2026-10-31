# Church Communications Agent

**Prepared for:** Lorenzo  
**Prepared by:** Parag and the development team  
**Target:** Ready enough to launch in January / Q1  
**This document:** Please mark anything missing or anything you want moved between Phase 1 and Phase 2.

---

## 1. Why this, and why now

Parish clergy spend at least two hours every week on work that has to get done but is not why they were ordained: assembling the Sunday leaflet, hunting lectionary readings, fitting hymn scores, and writing announcements.

You called this the unholy work of being a priest. The point of this agent is to take that work so the priest can do the holy work: hospital visits, blessing people, and being with the congregation.

A lot of church people are wary of AI, and even more wary of agents that can actually do things. The way in is not theology or sermon writing. It is one small, repetitive, weekly task that already eats time. If that task is dependable and the priest stays in control, they get more comfortable handing the next task over.

That first task is the Sunday bulletin.

We are calling this a **Communications Agent**, not a bulletin maker. The bulletin is the first job. The name leaves room to add the newsletter, a press release, and Sunday sermon clips once clergy trust it.

Phase 1 is Episcopal and Revised Common Lectionary first. That is the calendar and the leaflet you walked through on the call. Other denominations can come later.

We already have liturgical-date groundwork from related church work. That covers dates only. The bulletin, the liturgy templates, and the weekly communications workflow are new.

---

## 2. What we need from you before build

You offered to send sample bulletin PDFs so we can see how congregations actually put everything on the page. We should start from those, not from a generic booklet.

Please send **4 to 6 real bulletins** before kickoff, ideally:

- an ordinary-time Sunday
- a feast that falls on Sunday (All Saints is the example from the call)
- a Sunday in Advent or another season with no proper / feast choice
- a bilingual English / Spanish leaflet, if you have one
- any leaflet that uses a layout you would want as a default

Those samples become the Phase 1 template. A real Episcopal bulletin is the order of service, not only readings, cover, hymns, and announcements. The static liturgy stays in the template. The weekly variables are the ones you named: the day's readings, the cover image, the music, and the announcements.

---

## 3. Phase map

| Phase 1 — January lock | Phase 1 stretch — you can pull forward | Phase 2 — after the bulletin is trusted |
| --- | --- | --- |
| Weekly conversational assistant | Bilingual English / Spanish template | Sermon video ingest from YouTube or Facebook Live |
| Episcopal RCL engine (Years A, B, C) | Suggested liturgical cover-art library | AI clips with captions and light music |
| Feast vs proper, only when the calendar actually forks | Public-domain hymnal inserts | Drafts-first social posting, then optional auto-post |
| Track 1 / Track 2 stored as a season setting | Parish website or Google Calendar ingest | Newsletter from that week's approved bulletin |
| Cover image upload | Extra layouts beyond the first sample-based template | Conversational press-release helper |
| OneLicense hymn drop-zone | Full split-screen layout editor | |
| Announcement polish from bullet points | | |
| Preview, light edit, print-ready PDF | | |
| OneLicense footer and AI disclosure footer | | |

If something in the stretch column belongs in January, say so. If something in the lock feels too much, we will move it.

---

## 4. Phase 1 — the weekly Sunday bulletin

Phase 1 does one job well enough to put in front of clergy in January: produce next Sunday's leaflet, with the priest approving it before anyone prints.

### 4.1 One-time parish setup

At the start, the priest (or parish administrator) enters the things that should not be retyped every week:

- church name
- OneLicense number
- preferred Bible translation (Episcopal default: NRSV, unless you tell us otherwise)
- default template, taken from the sample bulletins you send
- Track 1 or Track 2 for the current ordinary-time season

The license number is reused every week in the required music footer.

### 4.2 Weekly conversation

The weekly flow is short and only asks questions that matter that Sunday.

1. **What Sunday is this?**  
   The agent already knows the Episcopal liturgical calendar. In ordinary time, if a major feast overlaps a Sunday, it asks the question you used on the call: *This Sunday is November 1. Are we doing All Saints' Day or Proper 26?*  
   Outside ordinary time — Advent, Christmas, Lent, Easter — there is no fork. It confirms the day and moves on. It does not ask Track 1 vs Track 2 every week. That lives on the parish profile and is changed when the season starts.

2. **Cover image**  
   Upload a parish photo, a youth-ministry graphic, or last year's cover. A suggested art library can come later if you want it in January.

3. **Music**  
   The priest names the hymns the way they already do: *Opening 287, Sequence 620, Offertory 293, Closing 625.*  
   OneLicense does not offer a public developer API, and logging in with a parish password would break publisher terms. So Phase 1 does what you described on the call: the priest downloads the JPEG from OneLicense and drops it into the reserved slot. Titles, authors, and the license footer are filled in for them. Public-domain scores can insert automatically later if we build that catalog.

4. **Announcements**  
   The priest pastes rough notes (*vestry tues 7pm, apple picking sat 9am, feeding of the hungry*). The agent turns them into clear parish notices. Calendar ingest from the church website or Google Calendar is available if you want it in Phase 1. Otherwise it waits.

The priest can still choose a different saved template for a special Sunday. The bilingual side-by-side English / Spanish layout is built if you pull it into January. Otherwise it is the first stretch item after the default leaflet works.

### 4.3 What actually goes on the page

From your samples we will lock:

- the static order of service and other liturgy that does not change every week
- the day's appointed readings from the Revised Common Lectionary, including the ordinary-time rule you described: Track 1 reads continuously, Track 2 is thematic, and the Epistle and Gospel stay the same
- the Collect of the Day and any other weekly proper that appears on the leaflets you send
- cover image
- hymns and scores
- announcements
- two footers on every bulletin:
  1. `Reprinted with permission under ONE LICENSE #[parish number]. All rights reserved.`
  2. `AI was used in the creation of this bulletin.`

### 4.4 Preview, edit, print

Before anything is final, the priest sees a preview and can fix a line, a title, or a date. Then the agent produces a print-ready PDF for the parish copier.

We are not promising a six-minute bulletin. The questions are quick. Licensed hymn images still take the usual OneLicense download. The saving is the assembly: readings, liturgy, layout, announcements, and the two required footers, without rebuilding the leaflet from scratch every week.

The priest always approves before print. That is the trust rule for Phase 1.

---

## 5. Phase 1 stretch

These are real, and they are not required to launch in January. Tell us which ones you want in Phase 1.

- **Bilingual template** — English and Spanish readings and liturgy side by side, as you described
- **Suggested cover art** — royalty-free liturgical images matched to the day's color and theme
- **Public-domain hymnal library** — classic scores that insert with no upload
- **Calendar ingest** — upcoming events pulled from the parish website or Google Calendar
- **Additional layouts** — extra folds or booklet styles beyond the first template taken from your samples
- **Richer layout editor** — a fuller split-screen editor if the simple preview is not enough

---

## 6. Phase 2 — after clergy trust the weekly job

Phase 2 is why it is a communications agent. None of this is required for the January launch.

### 6.1 Sunday sermon clips

Modeled on the Opus Clip workflow you showed, and on the Virginia priest who already uses it.

After a service that is already going out on YouTube or Facebook Live, the agent finds the sermon, pulls the strongest moments, adds captions, and can add a little music. Clips are saved as drafts. The priest reviews and posts.

When they trust it, they can let it post. You said he is not there yet. We will not start there.

### 6.2 Newsletter

Once that week's bulletin is approved, the same material can become an email newsletter.

### 6.3 Press release

A short interview — a few questions about the feeding program, the festival, the event — then a draft in the format they want, with the same AI disclosure.

---

## 7. What a Wednesday looks like

**One-time setup, already done:** Church of the example. OneLicense on file. Track 2 for this ordinary-time stretch. Default leaflet taken from the samples you sent.

1. The agent knows Sunday is November 1 and that All Saints and Proper 26 are both possible.
2. It asks: *Are we celebrating All Saints' Day or Proper 26?* The priest chooses All Saints.
3. It loads the All Saints readings and the other weekly propers that appear on your sample leaflets. It does not ask about Track 1 or Track 2.
4. The priest uploads a cover image, or reuses one.
5. The priest names the hymns. Public-domain scores fill in if we have them. OneLicense JPEGs are dropped into the reserved slots.
6. The priest pastes announcement bullets. The agent writes them in parish voice.
7. The priest opens the preview, fixes anything that is off, and approves.
8. The print-ready PDF includes both footers.

In Advent the same flow skips step 2. There is no choice to offer.

---

## 8. Timeline toward January

This is an eight-week build to a parish-ready Phase 1. It only works if the sample bulletins arrive at the start.

| Weeks | Work |
| --- | --- |
| 0 | You send sample bulletins. We lock the default template and the weekly variables from those pages. |
| 1–2 | Parish accounts, liturgical calendar, RCL database (Years A, B, C, propers, feast days, Track 1 / Track 2 as a season setting), scripture retrieval. |
| 3–4 | Weekly conversation, cover upload, hymn titles and OneLicense drop-zone, announcement writing. |
| 5–6 | Template from your samples, preview and light edit, print-ready PDF, both compliance footers. |
| 7–8 | Real bulletin tests with a few clergy, layout fixes, production deploy for January. |

Stretch items you pull into Phase 1 land in weeks 5–6 if they are small, or they get their own short pass after the first leaflet is stable.

---

## 9. How to mark this up

Please read this so you can see whether the pieces are right, and so you can move something into Phase 1 or out of it.

When you read it, it would help us to know:

1. Are the sample-bulletin types above the right set, or should we add another kind of Sunday?
2. What on the leaflet must be in the January lock besides readings, cover, hymns, announcements, static liturgy, and the two footers?
3. Which stretch items do you want in Phase 1: bilingual template, cover-art library, public-domain hymns, calendar ingest, extra layouts, richer editor?
4. Is newsletter a Phase 1 add, or does it stay in Phase 2?
5. Preferred default translation, if not NRSV.
6. Who are the first clergy you would want in the week 7–8 pilots?

Once you send this back, we will lock the Phase 1 set and put kickoff dates on it.

This is going to be good. The bulletin is the right first agent: weekly, familiar, and useful enough that people will try it.