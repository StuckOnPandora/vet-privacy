---
title: Privacy Policy — VET: Football Sim
---

# Privacy Policy — VET: Football Sim

**Effective date:** 2026-10-27

## Who we are

VET is a football simulation app made by TNT Productions. Questions about this policy or your
data go to stuckonpandora@gmail.com.

## What the app is

VET runs Monte Carlo simulations of real college football matchups and shows you a win
probability, a projected score, and a volatility read. It is a simulation of football games,
not a way to risk real money on an outcome. **NFL is planned but not in the app yet** — the
sport picker shows an NFL button that says so on its face and does nothing else until that
work lands.

## What the app collects

- **A random install ID.** The first time VET runs, it generates a random identifier on your
  device and stores it there. It does not contain or derive from your name, email, contacts,
  or any other identity information. **We keep no ledger tying it to you** — we hold no name,
  address, account or payment record it could be matched against, because we never collect
  one. One thing that promise does not stretch to, and we would rather say so plainly than
  let you find it for yourself: the company that hosts our server keeps its own automatic
  record of incoming requests, and on four of them that record holds the install ID and your
  device's network address together, for as long as it keeps that log. "What the server
  stores" below says exactly which four, and for how long.
- **The install ID goes out with most requests to our server**, so it can recognize repeat
  requests from the same install: checking your free-daily-count and purchase status, asking
  for live scores, asking for a halftime read, checking the record of Hardy's lane, running a
  simulation, and sending a note if you choose to send one. Four things the app
  asks for carry no install ID and nothing else that identifies you — checking whether our
  server is reachable, asking what models exist, fetching the week's schedule, and fetching
  final scores.
- **What you simulate.** Each time you run a simulation, the app sends the matchup you picked,
  the simulation depth (how many simulations to run), the date, and two on/off switches that
  control how much detail comes back in the result — these are always sent as part of how the
  result is built, not information you separately choose to share.
- **What a halftime read asks about.** Opening a halftime read for a saved simulation sends
  that simulation's own matchup, date, model, depth, and (when known) the run's seed back to
  the server — details pulled from the saved run itself, not new information about you.
- **A note, if you choose to send one.** OPTIONS has a SEND A NOTE box. If you type something
  and tap SEND, the app sends your words (up to 500 characters), your install ID, the app's
  version, and the screen you sent it from. Please do not put your name, email or any personal
  detail in it — the app does not ask for them and the box says so. The note is kept as a line
  in our server host's log (Google keeps it for 30 days) and in a copy we keep to read and
  answer feedback, which we delete on request.
- **An error log, if you choose to send it.** The app keeps its own short list of its last
  errors on your device (the time, the screen, and what went wrong, with your install ID,
  device folder names and anything shaped like an email address removed). It stays on your
  device unless you tap SEND THE LOG in OPTIONS, which sends it as a note in the same way,
  with your install ID and the app version.
- **Saved simulations, kept on your device.** When a simulation finishes, VET saves a local
  copy on your device: the matchup and the full result, plus a set of identifiers and
  provenance details saved alongside it — a run ID VET mints for that save, which tier you
  were on at the time, and which engine version and data freshness produced the result — and
  any note you write about your own read of the game, so you can reopen it later. **VET itself
  never transmits this saved copy or its card image anywhere.** If you use the SHARE button, a
  copy of the card image is placed in your device's shared Pictures folder (see "Data
  deletion" below) — from there, sending that copy anywhere else is something you do yourself,
  through another app, not something VET does.

## What the server stores

- **A list of install IDs marked as having full access.** Today this list is set by us,
  directly, when the service starts — **not through an in-app purchase yet** (Google Play
  Billing is not built into VET; see "Purchases" below). The list holds install IDs only —
  nothing else about you. **It is not kept in any lasting store.** It lives in the running
  server's own temporary storage, it is lost whenever that server stops or is replaced, and it
  is rebuilt from our own deployment setting the next time one starts — which also means
  taking an ID off it is a change we make to that setting, not a record we delete. See "Data
  deletion" below.
- **Google Cloud's own request logs.** Google Cloud, which hosts our server, automatically
  keeps its own record of every request any of its servers receives — this is Google's
  infrastructure working as it always does, not something we built or configured to collect
  more than the default. That record includes your device's IP address on every request, and
  the full address of each request — which, for checking your status, getting live scores,
  asking for a halftime read, and checking the record of Hardy's lane, includes the install ID, because on those it travels as a
  visible part of the address. Running a simulation sends the install ID a different way (as
  part of the request's contents rather than its address), which this kind of log does not
  record. Google keeps that log for 30 days, and we have not asked for it to be kept any
  longer.
- **Separately, our own application briefly notes** each request it handles, for
  troubleshooting. That note holds seven things and nothing else: the time, the method, which
  feature was asked for, whether it succeeded, how long it took, the install ID, and the
  simulation depth — and of the install ID it keeps only the first eight characters. "Which
  feature was asked for" is the bare route — not the rest of the address — so that shortened
  install ID appears there once, in its own field, and never twice. What you
  send in a request is never written into it. This note is not the same thing as Google's
  own log above: it is stored on the individual Cloud Run instance's in-memory filesystem and
  is lost when that instance stops — it is not durable, and it is not shared between instances
  — so it is never collected into any long-term store.

## What is NOT collected

VET does not collect or ask for: a name, an email address, a phone number, your location,
your contacts, an advertising identifier, or any account at all — there is no sign-up and no
login, and the app never asks your age. The app has no analytics software and no third-party
crash-reporting software. Nothing about your use of the app is sent anywhere except what is
described on this page, and an error log or a note is sent only when you tap send.

## Purchases

Purchases will be handled entirely by Google Play, and we will never see your payment card,
billing address, or any other payment detail. **This is not built yet.** Right now, VET has no
purchase flow at all — no Google Play Billing integration, and no way for the app or our
server to verify that a purchase happened. Full access is currently granted by us by hand, to
a short list of install IDs, for testing. Until the real purchase flow ships, and until it
can recognize a returning paying install, a reinstall does not carry a purchase
forward — see "Data deletion" below.

## Children

VET is for adults 18 and over; it is not designed for or directed at children. There is no
age gate anywhere in the app and it does not ask for or collect your age — "for adults" is a
design and content decision on our part, not something the app checks or enforces.

## Data deletion

Uninstalling VET deletes everything the app stored in its own private storage on your device
— your install ID, your preferences, and every saved simulation — nothing is recoverable
after that, on our side or yours. **One exception:** if you used the SHARE button on a saved
simulation, a copy of that card image was placed in your device's shared Pictures folder,
outside the app's own storage; uninstalling VET does not remove that copy, and you delete it
the same way you would delete any other photo.

**Reinstalling VET is not the same install as before.** The app has no way to recover your old
install ID — reinstalling mints a brand-new random one — so a reinstalled app starts with no
saved simulations and, today, cannot be recognized as a previously-unlocked install either
(see "Purchases" above; this is expected to improve once a real purchase flow exists). If you
were given full access by us for testing and want that install ID removed from our server-side
list, write to stuckonpandora@gmail.com. Today this is done by hand, and it is worth knowing
what that means: the list is rebuilt at every start from our own deployment setting, so the
removal has to happen in that setting — taken off the running server alone, an ID would simply
come back the next time it restarted. There is no automatic self-service deletion route yet.

**Notes and error logs you sent.** To have a note or an error log removed, write to
stuckonpandora@gmail.com. The app does not show you your install ID, so tell us roughly when
you sent it and the app version; without the install ID we may not be able to find it. We
delete our own copy. Google keeps its own request log for 30 days and we cannot remove single
lines from it earlier.

## Third parties

- **Google Cloud** hosts our server and, as described above, keeps its own standard request
  logs — including the install ID (as part of the request address) and your IP address —
  under its own retention rules, separate from and longer-lived than our own application's
  brief, ephemeral note.
- **Google Play** will handle purchases once that feature ships, as described above.
- **Our football data source** runs on our server only. Your device never talks to it
  directly, and it never receives your install ID, your requests, or anything else about you
  — it only ever sends us the public schedule and team data VET's simulations run on.

## Changes to this policy

If this policy changes, we will update the effective date above and post the new version at
the same address.

