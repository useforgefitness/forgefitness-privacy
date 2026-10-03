# Forge Fitness Privacy Policy

**Effective date: October 2, 2026**

Forge Fitness is built on a simple principle: **your data is yours.**
There are no accounts and no ads. Your training lives on your phone and
in your own iCloud, where we cannot see it. The app checks with
RevenueCat for Forge Pro each time it opens (see Forge Pro purchases),
and a few optional features send specific things elsewhere, only when
you use them. Each one is described below. Two of them use AI: the coach
and food photos, both answered by OpenAI's AI models.

Forge Fitness is made by **Aitken Enterprise LLC**, a Florida limited
liability company. "We" and "us" in this policy mean Aitken Enterprise LLC.

## What the app stores, and where

On your device, and synced to **your own iCloud** (see iCloud sync):

- Your profile (name, birthday, height, weight, sex, preferred units)
- Your training split, workouts, sets, and workout notes
- Your calendar schedule and planned rest days
- Your running answers and running plan
- Your nutrition goal, activity level, calorie and macro targets, and the
  meals you log
- Your recovery log (the readings shown on your recovery card)
- Menstrual cycle dates and cycle settings, if you choose to log them

On your device **only**, never synced:

- Workout and progress photos
- Night-by-night temperature readings used for cycle estimates, symptom
  and birth-control notes, and any weight-management medication you note
- Your last few coach conversations, and the record of changes the coach
  made
- The time zone your phone was in on each day you opened Forge, your
  approximate location once a day if you turn that on, and the time of
  any Airplane Mode note your own Shortcuts automation leaves, used only
  to ask whether you're traveling (see Travel Mode)

None of this is sent to us. We have no server that could receive it.

## Apple Health (HealthKit)

With your permission, Forge Fitness **reads** from Apple Health: heart
rate variability (HRV), resting heart rate, heart rate during sleep,
breathing rate, sleep, steps, VO2 max, body weight, height, date of
birth, biological sex, and workouts recorded by your watch or other apps
(to bring in your cardio and to time your lifts). If you track your
cycle, it can also read menstrual flow and sleeping wrist temperature,
asked for separately.

With your permission, it **writes** one thing: each workout you finish in
Forge (strength training for a lift, or the kind of cardio you logged),
with its start time and length and never calories, so it counts in the
Health app. If your watch already recorded the session, Forge does not
write a second one.

- Health data is used to show you your own training and recovery. It is
  never used for advertising or marketing, and never sold.
- It leaves your device only in your own iCloud sync and, when you turn
  them on, in the optional features below: recovery you share with a
  friend, readings you let the coach see, and recovery you share with a
  trainer.
- You can change these permissions at any time in the iPhone's Settings
  app under Privacy & Security, Health, Forge Fitness. The app works
  without them; recovery fields show a dash.

## Cycle tracking

If you log menstrual cycle information, it is stored on your device and
in your own iCloud with the rest of your log, and is visible to no one
but you. It is never shared with friends or a trainer. The coach sees
only today's cycle phase, and only while you allow it to see your
readings and body data. We have no copy of your cycle data and could not
produce one if asked.

## Oura Ring (optional)

If you choose to connect an Oura Ring, tapping Connect opens **Oura's own
sign-in in a secure window run by iOS**. You sign in to Oura there and
approve the connection. Forge Fitness never sees your Oura email or
password. Then:

- You approve exactly two permissions: your **daily** summaries and your
  **heart rate**. Nothing else is requested.
- Your readings travel **directly from Oura's API to your phone**: your
  nightly sleep summaries (HRV, lowest heart rate, sleep time), readiness
  temperature, daily steps, and cycle data if Oura has any. The first time
  you connect, up to six months of past nights come in so your normal is
  ready from the start.
- Oura requires that the key which turns your sign-in into a connection is
  kept off phones, so Forge Fitness runs **one small relay** (a Cloudflare
  Worker) that passes your one-time sign-in code to Oura, hands Oura's
  connection tokens back to your phone, and renews them the same way.
  **The relay stores nothing, logs nothing, and never sees a reading.**
- The tokens are stored **in the iOS Keychain on your device** and sent
  only to Oura, and to the relay when they are renewed. The connection
  renews itself; you reconnect only if it is revoked.
- Oura's handling of your data is covered by
  [Oura's privacy policy](https://ouraring.com/privacy-policy).
- Disconnecting (☰ menu, Fitness tracker, Oura Ring, Disconnect) deletes
  the connection from your device immediately.
- If you never connect Oura, nothing is sent to Oura or to its relay.

## WHOOP (optional)

If you choose to connect a WHOOP, tapping Connect opens **WHOOP's own
sign-in in a secure window run by iOS**, exactly like Oura. Forge Fitness
never sees your WHOOP email or password. Then:

- You approve three read permissions: your **recovery** (HRV, resting
  heart rate), your **sleep**, and your **daily cycles**. Nothing else is
  requested. The first time you connect, up to six months of past nights
  come in so your normal is ready from the start; after that, each new
  night.
- WHOOP requires that the key which turns your sign-in into a connection
  is kept off phones. So Forge Fitness runs **one small relay** (a
  Cloudflare Worker) that does that single job: it passes your one-time
  sign-in code to WHOOP and hands WHOOP's connection token back to your
  phone. **The relay stores nothing and logs nothing.** It never sees a
  reading; your recovery and sleep data travel **directly from WHOOP to
  your phone**.
- The connection token is stored **in the iOS Keychain on your device**
  and is sent only to WHOOP, only to read your data. When it expires the
  app renews it through the same relay, which again keeps nothing.
- WHOOP's handling of your data is covered by
  [WHOOP's privacy policy](https://www.whoop.com/privacy/).
- Disconnecting (☰ menu, Fitness tracker, WHOOP, Disconnect) deletes the
  connection from your device immediately.
- If you never connect WHOOP, the relay is never contacted.

## The coach (optional)

Forge has a coach you can ask about your training. It is off until you
open it and read a short screen saying what it sends. When you send a
message:

- **What goes up:** your message, and a short summary in words of your
  program (every day's exercises), this week's progress, your running
  plan and today's run, any workout you have open, what Forge is
  currently offering you (such as an easy week), your recent sessions
  (dates, exercises, sets and weights), today's recovery band with
  Forge's own reasoning for it, and the changes the coach itself made in
  the last two weeks. If the coach looks something up (for example where
  a setting is, or one exercise's last few sessions), only what that
  lookup returns goes with it.
- **Only if you choose:** a photo, when you attach one to a message;
  your recent HRV, resting heart rate, sleep and breathing-rate readings,
  plus your latest body weight, height, age and today's cycle phase (if
  you track it), only while "Let the coach see my readings, body and
  cycle data" is on; and your nutrition targets and today's meal totals,
  only while "Let the coach see my food and nutrition targets" is on.
  Both are off by default. The coach can read these; it cannot change
  them.
- **What never goes up:** sleep stages, tape measurements, your period
  log itself, medication, your other photos, friends or friend codes, or
  anything about your device beyond a random id (below).
- **Where it goes:** to Forge's relay (a Cloudflare Worker that holds the
  API key and keeps no conversation and no message text), then to
  **OpenAI**, whose AI model writes the reply. Under OpenAI's API terms it
  does not use what we send to train its models, and it keeps it for no
  more than 30 days, only to check for abuse, unless the law requires
  longer. Neither stores your conversation for us.
- **If you mention hurting yourself:** the app shows you how to reach the
  988 Suicide & Crisis Lifeline. That check happens on your phone and
  sends nothing extra anywhere.
- **On your phone:** your last few exchanges stay on this phone and go
  with your next question, so follow-ups make sense. Clear them any time
  from the chat's menu (Forget earlier conversations).
- **The random id:** the app makes a random id once, stores it in the
  Keychain, and sends it so the relay can limit how many messages a phone
  sends per day. It is tied to no account, no health data and no friend
  code, because none of those exist together anywhere.
- **Changes:** anything the coach suggests changing is a card you
  confirm. Each change you apply is recorded on this phone, under the
  chat's menu (Changes the coach made), with a way to undo it. Nothing in
  the app changes on its own.
- **Turning it off:** simply do not use it. Nothing is sent unless you
  send a message.

## Sharing with a trainer (optional)

If you choose to share your training with a trainer (☰ menu, Personal
Training), the app writes one record to Apple's iCloud infrastructure for
this app containing only the categories you tick: your program, upcoming
sessions, recent sessions, every set, effort (RPE), adherence, progress,
your notes, and, only if you turn it on separately, last night's sleep,
HRV and resting heart rate with the recovery band. Recovery is off by
default.

The record is encrypted on your phone with a key made from a
ten-character trainer code that only you and the person you give it to
hold. Nobody else, including us, can read it. Your trainer reads it in
their own copy of Forge Fitness and can change nothing on your phone.
Turning a category off rewrites the record without it. A share runs until
you stop it or your trainer disconnects, and either one deletes the
record. Your trainer can remember or screenshot what they saw; ending the
share removes it from Forge, not from them. Never shared this way: your
body weight and measurements, cycle log, progress photos, medication
context, nutrition targets, or who your friends are. Don't share, and
nothing is ever written.

## Food photos (optional)

If you choose to log a meal from a photo, the photo is sent once, through
the same relay the coach uses, to **OpenAI**, whose AI model estimates
what is on the plate. The photo is not stored by us, and OpenAI handles
it under the same API terms as the coach (not used for training, kept no
more than 30 days to check for abuse). What comes back is an estimate
of the foods, calories, protein, carbohydrates and fat, which you can
change before saving. Only the numbers you save are kept, on your device
and in your own iCloud with the rest of your log. Food data is never
shared with friends or with a trainer; the coach sees your targets and
today's totals only while its food switch is on. Don't use the feature,
and no photo is ever sent.

## Voice logging (optional)

If you log a set by voice, Apple's speech recognition turns what you say
into text, on your iPhone where the phone supports it; otherwise Apple
processes the audio under
[Apple's privacy policy](https://www.apple.com/legal/privacy/). Forge
keeps only the set it logs.

## Calendar (optional)

If you turn on calendar sync (☰ menu, Settings, Calendar), Forge adds
your training days as events to the calendars you choose. Those calendars
(iCloud, Google or another account on your phone) store and sync the
events like any other.

## Travel Mode (optional)

When your phone's time zone changes, Forge asks whether you're
traveling, and keeps that record of time zones on this phone.

If you turn on "Trips in your own time zone" (☰ menu, Settings, Noticing
a trip), Forge also checks your **approximate** location once a day when
you open it, to tell home from away. It never tracks you in the
background, keeps these places on this phone only, and never sends them
anywhere. Turning the switch off deletes them, and you can also turn
location off for Forge in the iPhone's Settings.

If you set up a Shortcuts automation for Airplane Mode, it leaves Forge a
timestamp and nothing else. Travel Mode turns on only when you say yes.
Workouts logged in Travel Mode are filed under "Travel" and sync with the
rest of your log.

## Forge Pro purchases

Forge Pro is sold through the App Store, and the app uses **RevenueCat**
(RevenueCat, Inc.) to handle the purchase. So that the app knows whether
you have Forge Pro, it checks with RevenueCat each time it opens.

- **What RevenueCat receives:** a random ID made on your phone for this
  purpose (not your name, email or Apple ID); your Forge Pro purchases,
  trials and renewals as Apple reports them; which Forge Pro page you were
  shown and whether you bought; and the technical details every request
  carries: the app version, your iPhone model and iOS version, your App
  Store country and language, and an identifier Apple gives this app on
  your device.
- **Never** your training, recovery, health, cycle, food or friends data.
- **Why:** to unlock Forge Pro, to restore it on a new phone, and to
  compare versions of the Forge Pro page (for example two prices, or two
  headlines) by how many people start a trial, stay and pay.
- Apple takes the payment. Neither we nor RevenueCat ever see your card.
- RevenueCat keeps this under its own
  [privacy policy](https://www.revenuecat.com/privacy/).

## Friends leaderboard (optional)

If you choose to join the friends leaderboard, the app publishes a small
"card" so friends who have your code can see it: the display name you
pick (it does not need to be your real name), your current streak, your
weekly totals (sessions, volume, and PR days), how many of your planned
lifting days (and, with a running plan, runs) you have done this week,
your personal records
from the last week, your all-time heaviest sets, and the top set of each
exercise in your last few workouts.

**Recovery readings are shared with named friends, one at a time, and
never on that card.** Last night's sleep duration, heart-rate
variability (HRV), resting heart rate, breathing rate, and the recovery
status Forge gave you can each be shared, each one its own switch for
what is shared, and a separate switch per friend for who receives it.
When you add a friend, Forge shows you what would be shared and offers
the choice before the friendship is made; you can decline it there, and
you can turn it off for any friend afterwards, at which point what they
could see is deleted immediately. A reading is sent only to the friends
you have chosen, in a record only that friend can read, and only when
it is last night's. Your workouts travel as each exercise's top set;
every set and your effort ratings travel only if you turn those on.
Nothing else ever joins the card: your notes, your food, and every
other health reading stay on your device.

**While Forge is in beta,** a TestFlight build may turn recovery sharing on
with all of your friends so the feature can be tested. The notes for that
build say so.

Cheers and nudges you send to a friend are small records stored the same
way and found by your friend's code; a nudge carries the message you pick
or write. You can stop friends nudging you in Privacy & sharing. Only
people on your list reach you: removing a friend also stops their cheers
and nudges. To report someone, tap Report on their page in the Friends
tab; it drafts an email to us with their friend code, and we can remove a
card that breaks our Terms. Names and written nudges containing slurs,
sexual words or threats are not sent.

Cards are stored in Apple's iCloud infrastructure for this app and are
findable only by your six-character friend code, which you share
yourself. Don't join, and nothing is ever published.

## Sharing a workout card

When you share a workout or a record, the card is made on your phone and
goes only where you send it (Photos, Messages, or another app such as
Snapchat), under that app's own terms. Nothing is sent until you choose
where.

## Our websites

useforgefitness.com and this policy's site set no cookies and run no
analytics, tracking or ads. They are hosted by Cloudflare and GitHub,
which, like any web host, receive your IP address to deliver the page,
and the main site loads its typeface from Google Fonts, so Google
receives your IP address too.

## What we don't do

- **No accounts.** There is nothing to sign up for and no login.
- **No tracking.** No advertising identifiers and no tracking of any
  kind. The one thing Forge measures is the Forge Pro page itself,
  through RevenueCat (see Forge Pro purchases): which version was shown
  and whether it sold. Nothing about how you train.
- **No selling, no advertising.** Your data is never sold or used for
  advertising. The only outside companies that ever receive any of it are
  the ones named above, for the feature you are using: Apple (iCloud,
  Health and speech recognition), Oura and WHOOP (your own data, at your
  request), OpenAI (the coach and food photos), and RevenueCat (Forge Pro
  purchases).
- **No network activity beyond** iCloud sync, the Forge Pro check, and
  the optional Oura, WHOOP, coach, food photo, friends and trainer
  features above. The pieces of
  ours on the internet are three small relays (the Oura sign-in, the WHOOP
  sign-in, and the coach and food photos); none of them keeps your data.

## Backups and iCloud

Like most apps, Forge Fitness's data is included in your device backup
(iCloud backup or computer backup) if you have backups enabled. Those
backups are managed by Apple under your Apple ID and covered by
[Apple's privacy policy](https://www.apple.com/legal/privacy/). We have
no access to them.

## iCloud sync

Forge Fitness syncs your data to **your own private iCloud account** so
it survives a lost or replaced phone. There is no account to create and
no password: syncing uses the Apple ID already on your device, and the
data goes into your personal iCloud storage, which Apple encrypts and we
cannot access. If you are not signed into iCloud, the app simply works
locally. Your recovery log is part of this sync; beyond your own iCloud,
readings go only where the optional features above say, and only when you
turn them on.

## Notifications

The app can show local notifications (for example, when your rest timer
ends, or a reminder before a free trial ends if you ask for one). These
are generated entirely on your device. We do not send push notifications
and have no ability to.

## Children

Forge Fitness is a fitness tool intended for teens and adults and is not
directed at children under 13. We don't knowingly collect information
from children under 13. If you believe a child under 13 has joined the
friends leaderboard, email us and we will remove their card.

## Deleting your data

Delete any workout from Workout history (☰ menu) or from its day on the
Today screen. Deleting the app removes everything on that phone. Your
iCloud copy stays in your own iCloud until you delete it there, from your
iPhone's iCloud storage settings. Stopping a trainer share deletes that
record, and turning recovery sharing off deletes what friends could see.
Removing a friend (on their page in the Friends tab) takes them off your
list and deletes the recovery you shared with them.

Your friend card, and any cheers and nudges you sent, stay in Forge's
shared database after you delete the app, because they are not stored on
your phone. To have them deleted, email **useforgefitness@gmail.com** with
your friend code (shown on the Friends tab) and we will delete them within
30 days.

## Changes to this policy

If the app's data practices ever change, this policy will be updated and
the effective date revised before the change takes effect.

## Contact

Questions about privacy in Forge Fitness: **useforgefitness@gmail.com**

Aitken Enterprise LLC, Florida, United States
