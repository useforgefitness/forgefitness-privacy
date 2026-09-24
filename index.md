# Forge Fitness Privacy Policy

**Effective date: September 23, 2026**

Forge Fitness is built on a simple principle: **your data stays on your
device.** The app has no servers, no accounts, and no analytics. We cannot
see your data. Not because we promise not to look, but because it never
leaves your phone in the first place.

## What the app stores, and where

Forge Fitness stores the following information **only on your device**:

- Your profile (name, birthday, height, weight, sex, preferred units)
- Your training split, workouts, sets, and workout notes
- Your calendar schedule and planned rest days
- Your nutrition goal, activity level, and calorie/macro targets
- Menstrual cycle dates and cycle settings, if you choose to log them

None of this is transmitted to us or to any third party. Deleting the app
deletes this data.

## Apple Health (HealthKit)

With your permission, Forge Fitness **reads** from Apple Health: heart
rate variability (HRV), resting heart rate, heart rate samples from your
sleep, sleep duration, and daily step count. These appear in the app's
recovery card, rest-day view, and insights. If you choose to use the cycle import (a separate permission,
asked only when you tap Import), the app also reads menstrual cycle dates
recorded by your cycle-tracking app.

- The app never writes to Apple Health.
- Health data is read on your device and displayed on your device. It is
  never transmitted anywhere.
- Health data is never used for advertising or marketing, never shared
  with third parties, and never used for any purpose other than showing
  you your own recovery information, as required by Apple's HealthKit
  guidelines.
- You can grant or revoke this permission at any time in the Health app
  under Sharing → Apps → Forge Fitness. The app works fully without it;
  recovery fields simply show a dash.

## Cycle tracking

If you log menstrual cycle information, it receives the same treatment as
everything else: **stored only on your device, transmitted nowhere,
visible to no one but you.** There is no server copy of your cycle data,
and we could not produce one if asked, because it does not exist.

## Oura Ring (optional)

If you choose to connect an Oura Ring, tapping Connect opens **Oura's own
sign-in in a secure window run by iOS**. You sign in to Oura there and
approve the connection. Forge Fitness never sees your Oura email or
password. Then:

- You approve exactly two permissions: your **daily** summaries and your
  **heart rate**. Nothing else is requested.
- The app talks **directly to Oura's API**, and to nothing else, to read
  your own nightly sleep summaries (HRV, lowest heart rate, sleep time)
  and daily step count.
- Oura issues a connection token to the app. It is stored **in the iOS
  Keychain on your device** and is sent only to Oura, only to read your
  data. We never see it: the app has no servers.
- The connection lasts about a month, then you reconnect. The app tells
  you several days beforehand rather than letting your readings quietly
  stop.
- Oura's handling of your data is covered by
  [Oura's privacy policy](https://ouraring.com/privacy-policy).
- Disconnecting (Profile, Connect Fitness Tracker, Oura Ring, Disconnect)
  deletes the connection from your device immediately.
- If you never connect Oura, the app makes **no network requests at all**.

## WHOOP (optional)

If you choose to connect a WHOOP, tapping Connect opens **WHOOP's own
sign-in in a secure window run by iOS**, exactly like Oura. Forge Fitness
never sees your WHOOP email or password. Then:

- You approve three read permissions: your **recovery** (HRV, resting
  heart rate), your **sleep**, and your **daily cycles**. Nothing else is
  requested, and the app reads only your own most recent night.
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
- Disconnecting (Profile, Connect Fitness Tracker, WHOOP, Disconnect)
  deletes the connection from your device immediately.
- If you never connect WHOOP, the relay is never contacted.

## The coach (optional)

Forge has a coach you can ask about your training. It is off until you
open it and read a short screen saying what it sends. When you send a
message:

- **What goes up:** your message, and a short summary in words of your
  program, your recent sessions (dates, exercises, sets and weights), and
  today's recovery band with Forge's own reasoning for it. If the coach
  looks something up, only what that lookup returns goes with it (for
  example, one exercise's last few sessions).
- **Only if you choose:** a photo, when you attach one to a message; and
  your recent HRV, resting heart rate, sleep and breathing-rate readings,
  plus your latest body weight, height, age and today's cycle phase (if
  you track it), only while "Let the coach see my readings and body data"
  is on (off by default). The coach can read these; it cannot change them.
- **What never goes up:** sleep stages, tape measurements, your period
  log itself, medication, your other photos, friends or friend codes, or
  anything about your device beyond a random id (below).
- **Where it goes:** to Forge's relay (a Cloudflare Worker that holds the
  API key and keeps no conversation and no message text), then to
  **OpenAI** to write the reply, under OpenAI's API data terms. Neither
  stores your conversation for us; the app keeps it only on your screen
  until you start a new chat.
- **The random id:** the app makes a random id once, stores it in the
  Keychain, and sends it so the relay can limit how many messages a phone
  sends per day. It is tied to no account, no health data and no friend
  code, because none of those exist together anywhere.
- **Changes:** anything the coach suggests changing is a card you
  confirm. Nothing in the app changes on its own.
- **Turning it off:** simply do not use it. Nothing is sent unless you
  send a message.

## Sharing with a coach (optional)

If you choose to share your training with a coach, the app writes one
record to Apple's iCloud infrastructure for this app containing only
the categories you tick: your program, upcoming sessions, recent
sessions, every set, effort (RPE), adherence, progress, and, only if
you turn each one on separately, last night's sleep, HRV and resting
heart rate with the recovery band, and your notes. Recovery and notes
are off by default.

The record is encrypted on your phone with a key made from a
ten-character coach code that only you and the person you give it to
hold. Nobody else, including us, can read it. Your coach reads it in
their own copy of Forge Fitness and can change nothing on your phone.
Turning a category off rewrites the record without it. Stopping the
share, or your coach disconnecting, deletes the record. A share can
also be set to end on its own after twelve weeks. Your coach can
remember or screenshot what they saw; ending the share removes it from
Forge, not from them. Never shared this way: your body weight and
measurements, cycle log, progress photos, medication context,
nutrition targets, or who your friends are. Don't share, and nothing
is ever written.

## Food photos (optional)

If you choose to log a meal from a photo, the photo is sent once, through
the same relay the coach uses, to the service that estimates what is on
the plate, and is not stored by us or by that service. What comes back
is an estimate of the foods, calories, protein, carbohydrates and fat,
which you can change before saving. Only the numbers you save are kept,
on your device and in your own iCloud with the rest of your log. Food
data is never shared with friends or with a coach. Don't use the
feature, and no photo is ever sent.

## Friends leaderboard (optional)

If you choose to join the friends leaderboard, the app publishes a small
"card" so friends who have your code can see it: the display name you
pick (it does not need to be your real name), your current streak, your
weekly totals (sessions, volume, and PR days), your personal records
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

Cards are stored in Apple's iCloud infrastructure for
this app and are findable only by your six-character friend code, which
you share yourself. Don't join, and nothing is ever published.

## What we don't do

- **No accounts.** There is nothing to sign up for and no login.
- **No analytics or tracking.** The app contains no analytics SDKs, no
  advertising identifiers, and no tracking of any kind.
- **No third parties.** No data is shared with, sold to, or processed by
  anyone. (The optional Oura and WHOOP connections above talk only to
  Oura or WHOOP, at your request, about your own data.)
- **No network activity beyond the optional Oura and WHOOP connections,
  iCloud sync, the optional friends leaderboard, the optional coach, and
  the optional share with a coach.**
  Readings go only to your phone from Oura, WHOOP or Apple. The two
  pieces of ours on the internet are the WHOOP sign-in relay and the
  coach relay described above; neither holds your data.

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
locally. Your health readings (from Apple Health or Oura) are displayed
from your device and included in this sync only as part of your recovery
log; they are never sent anywhere else.

## Notifications

The app can show local notifications (for example, when your rest timer
ends). These are generated entirely on your device. We do not send push
notifications and have no ability to.

## Children

Forge Fitness is a fitness tool intended for teens and adults and is not
directed at children under 13.

## Deleting your data

Delete any workout from the History tab, or delete the app to remove
everything. Because no copies exist anywhere else, deletion is complete
and immediate.

## Changes to this policy

If the app's data practices ever change, this policy will be updated and
the effective date revised before the change takes effect.

## Contact

Questions about privacy in Forge Fitness: **useforgefitness@gmail.com**
