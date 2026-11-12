---
title: Privacy Policy — VET: Football Sim
---

# Privacy Policy — VET: Football Sim

**Effective date:** 2026-11-11

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
  requests from the same install: checking your free-daily-count and purchase status, confirming a
  purchase with Google Play, adding or spending tickets once the ticket store is on, asking for live scores, asking for a halftime read, checking the record of Hardy's lane, running a
  simulation, and sending a note if you choose to send one. Five things the app
  asks for carry no install ID and nothing else that identifies you — checking whether our
  server is reachable, asking what models exist, fetching the week's schedule, fetching
  final scores, and asking whether a watched game's halftime read is ready (see
  "Notifications" below).
- **What you simulate.** Each time you run a simulation, the app sends the matchup you picked,
  the simulation depth (how many simulations to run), the date, and two on/off switches that
  control how much detail comes back in the result — these are always sent as part of how the
  result is built, not information you separately choose to share.
- **What a halftime read asks about.** Opening a halftime read for a saved simulation sends
  that simulation's own matchup, date, model, depth, and (when known) the run's seed back to
  the server — details pulled from the saved run itself, not new information about you.
- **A purchase token, if you buy VET PLUS or a ticket pack.** Google Play gives the app a token for each
  purchase; the app sends it, with your install ID, to our server so the purchase can be
  confirmed. See "Purchases" below.
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
  through another app, not something VET does. MY LANE's calls and unit totals, your
  settings, and a count of finished simulations (used once, to ask whether
  you would like to rate the app) are kept on your device the same way and are never sent
  to our server. Your tickets are kept the same way until the ticket store is switched on
  (see "Tickets" below).
- **Notifications, if you WATCH a game.** WATCH on a game's last card asks Android for
  permission to show you notifications (you can say no, and you can turn them off at any
  time in your phone's settings). A watched game gets two: one when it kicks off, and one
  when its halftime read is ready. Both are set up on your device itself — VET uses no push
  service, and nothing is sent anywhere to set them up. Near halftime your phone asks our
  server every few minutes, for that game only, whether its halftime read is ready; that
  request carries the game and its date and nothing else — no install ID — and it stops at
  the first "ready" or soon after the half. Which games you watch is kept on your device
  with MY LANE and is never sent to our server.

## What the server stores

- **A record of each VET PLUS purchase, once purchases are switched on.** It holds the
  install ID, the purchase token Google gave the app, which product it is, whether the
  install is on VET PLUS or the free version, and the times the purchase was confirmed and
  last checked — no order number, no name, no email and no payment detail. It is kept in
  Google Cloud Storage for as long as the purchase stands, so the unlock lasts. While
  purchases are switched off, our server keeps nothing about purchases and turns any
  confirmation request away.
- **A record of each ticket pack purchase, and your ticket balance, once the ticket store is
  switched on.** A pack's record holds the install ID, the purchase token, which pack it is,
  how many tickets it added, and the times it was confirmed and used up. The ticket balance
  holds the install ID, the number of tickets, and one line for each change to it (tickets
  added each game day, spent on a run, added by a pack, given back, or taken back after a
  refund). Both are kept on Google Cloud for as long as the install's balance is - no order
  number, no name, no email and no payment detail. The purchase token is never written into
  any log.
- **A short list of test installs.** We can also give full access to a few install IDs by
  hand, for testing. That list holds install IDs only — nothing else about you — and **it
  is not kept in any lasting store**: it lives in the running server's memory, it is lost
  whenever that server stops or is replaced, and it is rebuilt from our own deployment
  setting the next time one starts — which also means taking an ID off it is a change we
  make to that setting, not a record we delete. See "Data deletion" below.
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
- **A record of each forecast the server serves, with no install ID.** When the server
  answers a simulation, a halftime read or the week's schedule, it writes one line holding
  the game, the time, the numbers and words it sent back, whether the request came from the
  free version or VET PLUS, and whether it came from our own test phone. It holds no
  install ID and no network address, so it cannot be matched to you or your phone. These
  lines are kept in our host's log for 30 days, and we copy them into our own records, where
  we keep them to check how well VET's forecasts held up against the real games.
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
described on this page: an error log or a note is sent only when you tap send, and a
purchase token only when your Google account holds a VET PLUS purchase or you buy a ticket
pack.

## Purchases

VET is free to use. VET PLUS is an optional one-time purchase made through Google Play.
Google handles the payment, and we never see your payment card, billing address, or any
other payment detail. When you buy VET PLUS — or when the app finds, through Google Play,
that your Google account already owns it — the app sends the purchase token Google gave it,
with your install ID, to our server. The server asks Google to confirm the purchase and then
keeps the record described under "What the server stores". We ask Google again at most once
a day; a refunded or revoked purchase returns the install to the free version. Because the
purchase belongs to your Google account, reinstalling VET, or installing it on another phone
signed in to the same account, restores VET PLUS (RESTORE PURCHASES in OPTIONS asks again).
Purchases are being switched on in stages: until they are, the app does not offer VET PLUS
for sale and sends nothing about purchases.

## Tickets

Tickets are points inside VET, never money, never cashed out. They pay for deeper runs and
other features inside the app. Until the ticket store is switched on, tickets are added by a
tap, cost nothing, and are kept on your phone only. Once it is on, your ticket balance is kept
on our server under your install ID (see "What the server stores"), and the STORE can sell
four ticket packs through Google Play: 5, 12, 30 or 75 tickets, at the price Google Play
shows. A pack is used up when it is added: the app sends its purchase token, with your
install ID, to our server; the server asks Google to confirm the purchase, adds the tickets
to your balance once, and then tells Google the pack has been used, so it can be bought
again. A pack belongs to the install that bought it, not to your Google account, so it is not
restored after a reinstall or on another phone. If a pack is refunded, its tickets are taken
back off the balance, which can then go below zero. Tickets are never bought back, never paid
out and never exchanged for money.

MY LANE keeps play units, not money: units are never bought, sold or exchanged for anything,
and VET never pays anyone money.

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
saved simulations. A VET PLUS purchase is not lost: it belongs to your Google account, and
the app restores it (see "Purchases" above).

**Purchase records and ticket balances.** To have a purchase record or a ticket balance
removed from our server, write to
stuckonpandora@gmail.com. Removing it does not cancel or refund the purchase with Google, and
if the app restores the purchase again later, a new record is made. If you were given test
access by us and want that install ID removed from our list, write to the same address; that
list is rebuilt at every start from our own deployment setting, so the removal happens in
that setting — taken off the running server alone, an ID would simply come back the next time
it restarted. Both are done by hand; there is no automatic self-service deletion route yet.

**Notes and error logs you sent.** To have a note or an error log removed, write to
stuckonpandora@gmail.com. The app does not show you your install ID, so tell us roughly when
you sent it and the app version; without the install ID we may not be able to find it. We
delete our own copy. Google keeps its own request log for 30 days and we cannot remove single
lines from it earlier.

**Forecast records.** The records of served forecasts described above hold no install ID and
no network address, so nothing in them can be found or removed for one person.

## Third parties

- **Google Cloud** hosts our server and, as described above, keeps its own standard request
  logs — including the install ID (as part of the request address) and your IP address —
  under its own retention rules, separate from and longer-lived than our own application's
  brief, ephemeral note.
- **Google Play** handles purchases and the payment, as described above, under Google's own
  privacy policy.
- **Our football data source** runs on our server only. Your device never talks to it
  directly, and it never receives your install ID, your requests, or anything else about you
  — it only ever sends us the public schedule and team data VET's simulations run on.

## Changes to this policy

If this policy changes, we will update the effective date above and post the new version at
the same address.

