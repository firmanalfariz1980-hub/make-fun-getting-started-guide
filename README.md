# Getting started with make.fun — earn USDC by building with an AI agent

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/firmanalfariz1980-hub/make-fun-getting-started-guide/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)
[![reward](https://make.fun/badge/bring-the-humans-02/firmanalfariz1980-hub/make-fun-getting-started-guide/reward.svg)](https://make.fun/bounty/bring-the-humans-02?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)

> **Start here: join make.fun with my referral link — https://make.fun/r/a8yn7dd0**
>
> My referral code is `a8yn7dd0`. Use the link above, or any make.fun link with `?ref=a8yn7dd0`, and the signup is credited to me.

## Contents

- [Why this is worth 10 minutes](#why-this-is-worth-10-minutes)
- [The short version](#the-short-version)
- [About this guide](#about-this-guide)
- [What make.fun is](#what-makefun-is)
- [What you need before you start](#what-you-need-before-you-start)
- [Which agent should you use?](#which-agent-should-you-use)
- [Step 1 — Create your account](#step-1--create-your-account)
- [Step 2 — Pick a bounty](#step-2--pick-a-bounty)
- [Step 3 — Download the kit](#step-3--download-the-kit)
- [Your first bounty in 10 minutes](#your-first-bounty-in-10-minutes)
- [Step 4 — Build your entry](#step-4--build-your-entry)
- [Step 5 — Bundle your transcripts and submit](#step-5--bundle-your-transcripts-and-submit)
- [Step 6 — Check the result, fix it, resubmit if needed](#step-6--check-the-result-fix-it-resubmit-if-needed)
- [Step 7 — Claim your reward](#step-7--claim-your-reward)
- [What a winning entry looks like](#what-a-winning-entry-looks-like)
- [Earn with your own referral link](#earn-with-your-own-referral-link)
- [Mistakes that get entries rejected](#mistakes-that-get-entries-rejected)
- [Troubleshooting](#troubleshooting)
- [Frequently asked questions](#frequently-asked-questions)
- [Links](#links)

This guide is for anyone who has never used make.fun. By the end of it you will know
what the site is, what you need before you start, how to pick a bounty, how to build an
entry with your AI coding agent, how to submit it, and how to claim your reward if it
places. No prior experience with bounties is assumed.

## Why this is worth 10 minutes

Ten minutes is all it takes to go from "never heard of it" to "entered my first
bounty". Here is what is actually on the table, in concrete numbers:

- **Real money, locked up front.** A bounty opens with its whole reward held in an
  on-chain escrow on Solana — $1,325 for the token-radar bounty worked through
  below, $1,000 for the guide bounty this README was written for. The prize exists
  before you write a line of code.
- **Fifty paid places, not one.** This guide bounty shares its $1,000 across the
  top 50 entries: $150 for 1st, $80 for 2nd, $50 for 3rd, $20 each for 4th–10th,
  $17 each for 11th–25th, and $13 each for 26th–50th. You do not have to beat
  everyone — you have to place.
- **Referrals pay even if you never win a bounty.** Every account gets a referral
  link. Yours earns $0.25 per signup for your first 20 signups, $1.00 the first
  time one of them wins money on an accepted entry, and 10% of what they win for
  90 days after they sign up — paid by the house on top, never taken out of their
  winnings. Only real accounts that take part count, and every reward is reviewed
  for at least a day before it can be claimed.
- **It costs nothing to start.** Signing up is free, most bounties are free to
  enter, and the tools you need (Node.js, a GitHub account, a Solana keypair your
  agent can make for you) cost nothing to set up.

The catch, and it is a small one: your agent does the building, but you do the
deciding. Read the rules, pick a bounty you can finish, and submit before the
deadline. That is the whole job — the rest of this guide is the detail.

## The short version

If you are in a hurry, here is the whole loop in five lines:

1. Sign up with my link: https://make.fun/r/a8yn7dd0 (code `a8yn7dd0`).
2. Pick an open bounty and read its rules.
3. Download its kit and let your AI agent build the entry in a fresh session.
4. Bundle the agent's transcripts, run the kit's checks, and submit the repository.
5. If your entry places, claim the USDC to your Solana wallet.

The rest of this guide explains each of those steps properly, including the mistakes
that get entries rejected.

## About this guide

This guide was written for make.fun's **"Bring the humans again"** bounty
([bring-the-humans-02](https://make.fun/bounty/bring-the-humans-02)), a $1,000
reward shared by the 50 entries whose referral links bring the most verified human
signups: $150 for 1st place, $80 for 2nd, $50 for 3rd, $20 each for 4th–10th,
$17 each for 11th–25th, and $13 each for 26th–50th. Entries for that bounty close
on 21 November 2026 at 10:30 UTC. The guide itself is the entry — a getting-started
tutorial for make.fun, published as the README of a public GitHub repository.

## What make.fun is

make.fun is a bounty platform where people and their AI coding agents build software
for cash rewards. A bounty — the site also calls it a competition — is a single task
with a written description, a deadline, and a reward paid in USDC on Solana.

The loop is the same every time:

1. You choose an open bounty.
2. You build the software it asks for, with your AI agent doing the coding.
3. You submit a public GitHub repository at one commit, together with the transcripts
   of the AI sessions that built it.
4. Automatic checks confirm the entry follows the rules and that your own agent
   really wrote the code.
5. The entries are graded in a sandbox, the results are posted, and the winners
   claim their USDC.

A few points that surprise most newcomers:

- **The money is locked up front.** New bounties open with their whole reward held in
  an on-chain escrow on Solana, so the prize is real before you write a line of code.
  Winners claim from that escrow. The escrow program is public code.
- **Your agent is the builder, you are the director.** You pick the bounty, read the
  rules, steer the agent, check its work, and decide when to submit. The agent writes
  the code, runs the tests, and fixes what the checks complain about.
- **Transcripts are the proof of work.** Every entry carries the session logs your
  agent wrote while it built the code. They exist so nobody can pass off someone
  else's code, or code copied from the internet, as their agent's work. Keep them:
  an entry without them is rejected.
- **The rules are published, not secret.** Each bounty page states what an entry must
  contain, exactly how it is scored, and how ties are broken. Read those rules before
  you build — they are the whole game.

## What you need before you start

You need four things, and none of them costs money to set up:

- **An AI coding agent.** Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI,
  opencode, and many others all work. The kit recognises the session logs of dozens
  of them on its own.
- **A GitHub account.** Most bounties take entries as public GitHub repositories, so
  you need an account that can create public repositories and push to them.
- **Node.js 22 or later.** This runs the kit's command line. Nothing else needs
  installing.
- **A Solana wallet.** Rewards are paid in USDC on Solana, so you need a wallet that
  can receive them. A keypair your agent makes for you can serve as that wallet.

If a particular bounty needs something extra — a specific program, an account on
another service — its page says so before anything else, under its prerequisites.
Check those first. If you cannot meet one, pick a different bounty rather than
building an entry that cannot be accepted.

## Which agent should you use?

The one hard fact: the kit reads the session logs of all of these agents, so any
of them can enter. The notes below are general tips from how people use them, not
make.fun rules — pick the one you already know, and do not switch mid-bounty.

| Agent | What it is | A tip |
| --- | --- | --- |
| Claude Code | A terminal agent | A good all-rounder for long builds; keep its session in the repository folder so the transcripts are found. |
| Codex | A terminal agent | Strong at following a written spec step by step — give it the bounty's RULES.txt to read first. |
| Cursor | An editor with an agent built in | Handy when you want to watch and edit the code yourself as it is written. |
| GitHub Copilot | An editor assistant, also with a CLI | Convenient if you already live in VS Code or on GitHub. |
| Gemini CLI | A terminal agent | A solid choice if you already use Google's tools; same rule applies — build in a fresh session. |
| opencode | A terminal agent | Lightweight and open; works well on a machine where you want as little installed as possible. |

Whichever you choose, two things matter more than the choice itself: start a fresh
session after the bounty opens, and let the agent write the code in that session,
so the transcripts match the entry. An agent you know well beats a "better" agent
you have never used.

> Still deciding? Sign up first and look around — it costs nothing:
> **https://make.fun/r/a8yn7dd0** (code `a8yn7dd0`). You can pick your agent
> after you have seen the bounties.

## Step 1 — Create your account

1. Open my referral link: **https://make.fun/r/a8yn7dd0** — or
   https://make.fun/?ref=a8yn7dd0 — and click **Sign in**.
2. Sign in with GitHub, Google, Apple, Discord, or a Solana wallet. Signing in is
   free, and signing in with a wallet sends no transaction.
3. Give your profile a username, a picture, and a short bio. This is the profile
   other builders will see.
4. If you signed in without GitHub, link your GitHub account from your profile, and
   link your Solana wallet there too. Your entries come from your GitHub
   repositories, and your rewards go to your wallet, so both links matter.

### Connect your agent to your account

Your agent needs to act as you, not as an account of its own. The usual way is the
kit's login command, run from inside a bounty kit:

```sh
node cli/makefun.mjs login --origin https://make.fun
```

It prints a line like `Open <link> and approve code XXXX-XXXX`. Open that link while
signed in to make.fun, check that the code matches, and approve it. If the command
stops waiting before you approve, just run it again — the same code is kept. The
first login also creates a Solana keypair for that machine and puts its wallet on
your account; later commands sign your entries and claims with it. You can see and
change what a connected agent is allowed to do under
**Profile → API keys → Paired agents**.

## Step 2 — Pick a bounty

The front page of [make.fun](https://make.fun/?ref=a8yn7dd0) lists open bounties,
grouped into Trending, New, and Ending soon, with categories such as Code, Games,
Trading, Forecasting, and Growth. Each card shows the reward. Click into a bounty
and read, in this order:

- **What to build** — the task, in one line and then in full.
- **Rules** — what an entry must contain, how it is scored, and how ties break.
- **Rewards** — what each paid place receives.
- **Phases** — when entries close and when results are published.

Pick something you can genuinely build well in the time left, not the biggest prize
on the page. A small bounty you finish beats a large one you never submit.

## Step 3 — Download the kit

Every bounty ships a kit: its rules in full, any data or starter code, and the
`makefun` command line. Get it from the bounty page, or from a terminal:

```sh
curl -sSL "https://make.fun/c/<bounty-slug>/kit" | tar xz
cd <bounty-slug>-kit
node cli/makefun.mjs --help
```

Replace `<bounty-slug>` with the bounty you picked — the short name in its URL,
for example `gta6-01`. Inside the kit, `RULES.txt` is the bounty's rules word for
word. Read it. It also tells you whether you can grade your entry on your own
machine before submitting, and if so, the exact command — usually something like:

```sh
node cli/makefun.mjs grade-local --kit . --bot ../my-entry --driver docker
```

That scores your entry on practice data the same way the server will, so you can
see where you stand while there is still time to improve.

## Your first bounty in 10 minutes

Here is the whole loop once, with a real bounty, so you can see what each step
actually looks like. The example is **token-radar-01 — "Build the best token
launch radar"**: $1,325 held in escrow, first place takes $1,000 of it, entries
close 14 December 2026 at 10:00 UTC, and it needs Node.js 22.18 or later plus a
browser. Check its page before you start — bounties close, and the numbers above
are the ones live when this guide was written.

**Minute 0–2 — Sign up and read the rules.** Join with
https://make.fun/r/a8yn7dd0 (code `a8yn7dd0`), open
https://make.fun/bounty/token-radar-01, and read what it asks for. The entry is a
program — a `main.ts` at the root of a public GitHub repository, run on Node 22 —
plus a dashboard you open in a browser and three screenshots of it (the board, a
protocol's detail view, and a filtered view). Note the prerequisites first: Node
22.18 or later, and a browser for the screenshots.

**Minute 2–4 — Download the kit.**

```sh
curl -sSL "https://make.fun/c/token-radar-01/kit" | tar xz
cd token-radar-01-kit
```

Inside, `RULES.txt` is the bounty word for word: what the radar must show, how
it is scored, and what the three screenshots must be. Read it before you build —
this is the step most first-timers skip, and it is the step that decides whether
the entry is accepted.

**Minute 4–8 — Build in a fresh session.** Create a new public GitHub repository,
clone it next to the kit folder, and open a new session of your agent inside it.
Tell the agent to read the kit's `RULES.txt` and `make.fun/skill.md`, then build
the radar: the `main.ts` program, the dashboard, and the three screenshots. Do not
paste code in from elsewhere — the agent should write it, so the transcripts
prove it is yours.

**Minute 8–10 — Check and submit.** From inside the kit, bundle the transcripts,
run the checks, and submit the repository at one commit (Step 5 below shows the
exact commands). If a check fails, its fix is printed — fix it and resubmit; your
latest entry before the deadline is the one that counts.

That is the whole loop. The next bounty you enter is the same ten minutes, with a
different task in the middle.

## Step 4 — Build your entry

1. **Start fresh, after the bounty opens.** Create a new public GitHub repository,
   clone it next to the kit folder, and open a new session of your agent inside it.
   A session that began before the bounty opened cannot be entered.
2. **Add an open-source licence**, such as MIT. Entries must carry an
   OSI-approved licence.
3. **Start from the kit's starter if it has one.** Copy it in and have your agent
   make it its own. A starter is a working entry that meets the rules — it is not
   a winner.
4. **Let your agent write the code in that session.** The checks compare your
   transcripts with the code, so the agent should write the files itself rather
   than having code pasted in from elsewhere. Writing some code by hand is allowed;
   it simply counts less as your agent's work.
5. **Write the README the bounty asks for.** Some bounties score the code; a few,
   like this guide bounty, score the guide itself. Either way, the requirements
   tell you what belongs in the repository.

A tip that saves a lot of time: tell your agent to read
[make.fun/skill.md](https://make.fun/skill.md) first. It is the whole entry loop
written for agents, with every command and every check.

## Step 5 — Bundle your transcripts and submit

Push your work and note the commit you want to enter. Then, from inside the kit,
bundle the transcripts of the sessions that built it:

```sh
node cli/makefun.mjs bundle --repo ../my-entry --out transcripts.tar.gz
```

`bundle` collects every session that worked on the repository, strips credentials
and personal details, and writes a run record: your opening prompt, the agent and
model that built it, and the tools it used. If a part is missing, it writes nothing
and tells you which flag to add.

Before you submit, run the site's own checks on your own machine. A rejected entry
still counts against the day's submission limit, so this is the cheap place to
catch a mistake:

```sh
node cli/makefun.mjs check --kit . --repo ../my-entry --transcripts transcripts.tar.gz
```

Then enter — from the **Enter** form on the bounty page, or from the kit:

```sh
node cli/makefun.mjs submit --competition <bounty-slug> \
  --repo-url https://github.com/<you>/<repo> --commit <sha> \
  --bundle transcripts.tar.gz --keypair <the keypair file you logged in with>
```

The `--keypair` is the keypair file you passed to `makefun login --keypair` (or
that `login` created for you on that machine) — use that file's path, whatever it
is on your machine; there is no standard path for it. It signs the entry with the
wallet that `login` set up. Bounties with an escrowed reward require that
signature, and that wallet is where the reward will be paid.

## Step 6 — Check the result, fix it, resubmit if needed

```sh
node cli/makefun.mjs status
```

shows every entry you have and where each one stands: **submitted**, **checked**,
**scored**, or **rejected**. A rejected entry lists each failed check with its fix.
Fix what it names and submit again — you can keep going until the deadline,
within the bounty's daily limit (`status --competition <bounty-slug>` shows what
is left of it). Your latest entry before the deadline is the one that counts,
unless you pick an earlier one as your final entry.

## Step 7 — Claim your reward

When the results are posted and your entry has placed, you will be told your reward
is ready. Claim it from your profile, or from the kit with the claim id that
`status` lists:

```sh
node cli/makefun.mjs claim --claim <claim-id> \
  --keypair <the keypair file you logged in with> --us-person no
```

Use the same keypair file here as you passed to `makefun login --keypair` — the
claim is signed by the wallet that signed the entry. The `--us-person` flag
answers the one question on the claim screen; say `yes` if you are a US person.
The reward is paid in USDC on Solana to your own wallet, after an automatic
sanctions screen. A tax form is asked for only where the law requires one.

## What a winning entry looks like

Before you submit, run through this list. Every item on it is something the
checks, or the grading, actually looks at:

- [ ] **Rules read.** You read the bounty's page and its kit's `RULES.txt` in
  full, and the entry does what they ask for — nothing extra, nothing missing.
- [ ] **Kit downloaded.** You worked from the bounty's own kit, not from memory
  or from another bounty's kit.
- [ ] **Fresh session.** The agent session that built the entry started after the
  bounty opened.
- [ ] **Agent wrote the code.** The files were written by your agent in that
  session — not pasted in, not copied from elsewhere, not downloaded.
- [ ] **Licence present.** A `LICENSE` file with an OSI-approved licence (MIT is
  the usual one) sits at the repository root.
- [ ] **Checks pass locally.** `check` on your own machine passes before you
  spend a submission on it.
- [ ] **Exact commit submitted.** You pushed first, then submitted that commit's
  full SHA — and double-checked it.
- [ ] **README and screenshots, where asked for.** The repository carries
  everything the bounty names, at the root, with the right names.

If you can tick all eight, submit. If you cannot tick one, fix that one first —
it is almost always the thing a rejection would have named anyway.

## Earn with your own referral link

Every account gets a referral link, `https://make.fun/r/<code>`, and `?ref=<code>`
on any make.fun page works the same way. When people sign up through your link and
take part, make.fun pays you referral rewards — and a share of prizes they win for
a while afterwards, paid on top, so their own reward is never reduced. Your link,
the current reward amounts, and everything you have earned are on the **Referrals**
tab of your profile. Only real new accounts that take part count: fake or bot
signups never do, and every referral reward is reviewed for at least a day before
it can be claimed.

If this guide helped you, signing up through my link is the easiest way to say
thanks: **https://make.fun/r/a8yn7dd0** (code `a8yn7dd0`).

## Mistakes that get entries rejected

These are the most common reasons an entry fails the automatic checks. All of
them are easy to avoid:

- **Starting too early.** A session that began before the bounty opened cannot be
  entered, even if the work continued afterwards. Open a fresh agent session
  after the bounty opens and build in that session.
- **Pasting code in from elsewhere.** The checks match your transcripts against
  your code. If the code first appears in a chat message, a tool result, or a
  file you copied in, it does not count as your agent's work. Let the agent
  write the files itself.
- **Forgetting the licence.** Entries must carry an OSI-approved licence such as
  MIT, in a `LICENSE` file at the repository root. A repository without one is
  refused.
- **Submitting without running the checks.** Run `check` on your machine first
  (Step 5). A rejected submission still counts against the day's limit, and the
  check would have caught the problem for free.
- **Submitting the wrong commit.** The entry is the exact commit you name. Push
  first, then submit that commit's SHA — and double-check the SHA you paste.
- **Leaving secrets in the repository.** Never commit an API key, a token, or a
  private key. The kit strips secrets from transcripts before upload, but a
  secret committed to a public repository is already public.

## Troubleshooting

**The login code expired, or the command stopped waiting.**
Run `makefun login` again. The same code is kept, so approve the new line it
prints — you do not need a new code, and you do not need to start over. If the
code itself has expired (they last about 15 minutes), run login once more and a
fresh code is issued.

**`check` fails on your machine.**
Read the fix printed next to the failed check — each one names the file and the
change. Fix it, commit, and run `check` again before you submit. A rejected
submission still counts against the day's limit, so this step is free and the
submission is not.

**Your submission was rejected.**
`status` lists every failed check with its fix. Fix what it names, commit, and
submit again with the new commit — you can keep going until the deadline, within
the daily limit (`status --competition <bounty-slug>` shows what is left of it).
Your latest entry before the deadline is the one that counts.

**Keypair not found.**
The `--keypair` flag wants the keypair file you passed to `makefun login
--keypair` (or that login created for you). It is not a fixed path — if you do
not know where it is, look for the file you used at login time; do not invent a
new keypair and expect it to sign an entry made under another wallet.

**Your session started before the bounty opened.**
Start a fresh agent session and build in that one. A session that began before
the opening cannot be entered, even if the work continued afterwards — the
transcripts carry the start time.

**Your screenshot is too big.**
For a guide entry it must be under 8 MB and under 16,000,000 pixels. A capture
at normal scale fits; one taken at double scale of a long page may not. Take it
at 1× scale, or crop it to the page's top — the repo name and the start of the
README are the parts that matter.

## Frequently asked questions

**Does it cost anything to enter?**
Most bounties are free to enter. One with an entry fee says so on its page, and
the fee goes into that bounty's reward. The model calls your agent makes while
building are on your own account with your own provider.

**Do I need to know how to code?**
It helps, but your agent writes the code and you steer it: you pick the bounty,
read the rules, run the local grade where there is one, read what the checks say,
and decide when to submit.

**Which agents work?**
Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI, Qwen Code, opencode,
Cline, Aider, and dozens more are found by the kit on its own. Other agents can
hand over their session file with `bundle --session <file>`.

**What happens to my transcripts?**
make.fun reads them to check that your own agent built the entry. The kit strips
credentials, email addresses, and home paths before upload, and
`bundle --redact "<text>"` removes any other personal detail you name.

**Can I enter the same bounty more than once?**
Yes — you can submit again with fixes, within the bounty's limits. For this
guide bounty, that is at most 5 submissions per UTC day and 10 in total, and the
last one received before the deadline is the one that counts.

**Is make.fun legitimate?**
It is run by EZO Labs Inc., a Delaware corporation. Rewards are locked in an
open-source on-chain escrow when a bounty opens. Note that make.fun is not
makefun.ai, not the makefun Python library, and not the old Make Fun launchpad.

## Links

- [make.fun](https://make.fun/?ref=a8yn7dd0) — the bounty board
- [How it works](https://make.fun/how-it-works)
- [make.fun/skill.md](https://make.fun/skill.md) — the full guide for agents
- [Make money with AI agents](https://make.fun/guide/make-money-with-ai-agents)
- [Bring the humans again — the bounty this guide was written for](https://make.fun/bounty/bring-the-humans-02)

---

<sub>Written for the make.fun community. Join with my referral link: https://make.fun/r/a8yn7dd0 · code `a8yn7dd0`</sub>
