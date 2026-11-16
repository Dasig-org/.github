<p align="center">
  <img src="https://bayanihan.dasig.org/emblem.png" alt="" width="72">
</p>

<h1 align="center">Bayanihan, an open initiative by Dasig</h1>

<p align="center">
  <b>Not everyone can run the whole thing. Everyone can take one step.</b><br>
  Open tools for volunteer groups and civic organizations, built in the Philippines.
</p>

<p align="center">
  <a href="https://bayanihan.dasig.org">Website</a> ·
  <a href="https://volunteer.dasig.org">Try Dasig</a> ·
  <a href="https://github.com/search?q=org%3ADasig-org+is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22&type=issues">Good first issues</a> ·
  <a href="mailto:hello@dasig.org">hello@dasig.org</a>
</p>

---

Every barangay has groups doing nation-building on weekends and goodwill: running clubs, feeding programmes,
tutoring circles, shore cleanups, animal rescues. Their plans live in group chats and in one tired coordinator's head.
When that person steps down, most of what the group learned leaves with them.

**Bayanihan** builds open foundations that let these groups plan, staff, run and report their work, on the phones
they already have, even with no internet. **Dasig** is the app that puts it in people's hands.

> **It's early.** The code started in late October 2026 and is in pilot with a small number of groups. Things change
> every week. That's also why it's a good moment to join.

## The pieces

| Repository | What it is | Licence |
|---|---|---|
| [**bix**](https://github.com/Dasig-org/bix) | **BIX, the Bayanihan Information Exchange.** An open format for civic work: groups, projects, teams, steps, needs, offers, and a signed record of who did what. Modelled on FHIR. | Apache-2.0 · spec CC BY 4.0 |
| [**bayanihan**](https://github.com/Dasig-org/bayanihan) | **Bayanihan Core and Bayanihan Server.** The rules engine that checks every change against BIX, and the reference server that stores records. Runs on a phone, a hub phone, or your own machine. | Apache-2.0 |
| [**bayani**](https://github.com/Dasig-org/bayani) | **Bayani**, a small language model for the civic sector. It runs on the phone and helps with a group's project memory. A person approves everything it suggests. | Apache-2.0 |
| [**dasig-app**](https://github.com/Dasig-org/dasig-app) | **Dasig**, the app for coordinators and volunteers, and the reference app for BIX. Android first, web for everyone else. | AGPL-3.0 |

```
           Dasig app  (or any app you build)
                │
      Bayani ───┤   small on-phone model: proposes, never decides
                │
   Bayanihan Core + Server   rules, permissions, signatures, storage
                │
               BIX   the open format everything speaks
```

## How you can help

- **Developers:** pick an issue labelled
  [`good first issue`](https://github.com/search?q=org%3ADasig-org+is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22&type=issues)
  or [`help wanted`](https://github.com/search?q=org%3ADasig-org+is%3Aissue+is%3Aopen+label%3A%22help+wanted%22&type=issues),
  and comment to claim it. Each repository's `CONTRIBUTING.md` explains setup.
- **Testers:** try [Dasig on the web](https://volunteer.dasig.org) or the Android APK from the
  [latest release](https://github.com/Dasig-org/dasig-app/releases/latest), and report what confused you. We need
  people with **iPhones** and **low-end Android phones** (4 GB) in particular.
- **Coordinators and volunteers:** tell us how your group really works. The format and the app are shaped with
  groups, not for them.
- **Standards and data people:** read the [BIX spec](https://github.com/Dasig-org/bix/blob/main/spec/BIX_v0.1.md)
  and open an issue where it's wrong, unclear or missing something.

## What we hold to

- **Privacy is part of the design.** People served are counts, never names. Photos of children never leave the group.
- **Plain words** for anyone who isn't a developer.
- **AI proposes, people decide.** No cloud AI in the product; the model runs on the phone.
- **The work belongs to the people who did it.** Records are signed, and anyone can check them.

Everyone taking part follows our [Code of Conduct](CODE_OF_CONDUCT.md). Report security or privacy problems privately,
as described in each repository's `SECURITY.md`.
