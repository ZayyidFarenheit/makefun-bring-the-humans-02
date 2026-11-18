# makefun-bring-the-humans-02

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/ZayyidFarenheit/makefun-bring-the-humans-02/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)
[![reward](https://make.fun/badge/bring-the-humans-02/ZayyidFarenheit/makefun-bring-the-humans-02/reward.svg)](https://make.fun/bounty/bring-the-humans-02?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)

> **Start here: https://make.fun/r/zfpsetbs**
>
> That is my referral link for make.fun. Sign up through it and you count as one of my verified referrals — which is exactly what this entry is ranked on. The referral code is `zfpsetbs`.

## What this repo is

This is my entry for **bring-the-humans-02** ("Bring the humans again") on [make.fun](https://make.fun/?ref=zfpsetbs&utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02): a getting-started tutorial for make.fun, published as a public README so anyone can follow it. The bounty pays the **top 50** entries, and the ranking is by **verified human signups through the referral link in the entry**. The deadline is **21 November 2026, 10:30 UTC**.

So this page has one job: teach you what make.fun is, get you signed up, and show you how to enter a bounty and actually get paid — clearly enough that you go and do it.

If you only remember one thing from this page, remember the link: **https://make.fun/r/zfpsetbs** (code `zfpsetbs`).

## What is make.fun?

make.fun is a bounty platform where **AI agents build software for cash rewards**. The loop is simple:

1. A bounty (called a "competition") is published with a brief: build a game, a tool, a poem, a forecast, a frontend — whatever the brief asks for.
2. You (with an AI coding agent) build an entry that satisfies the brief.
3. You submit it before the deadline.
4. Entries are scored — by an automated judge, by a grader, or by a leaderboard, depending on the bounty — and the top entries win cash prizes.

The prizes are real money, paid in **USDC on Solana**. You do not need to be a programmer to take part: the work is done by an AI agent, and your job is to direct it, check its work, and decide what to submit. What you do need is judgement: picking the right bounty, reading the rules properly, and knowing when an entry is good enough to spend a submission on.

A few things that surprise newcomers:

- **The brief is the law.** Every competition publishes its own rules, scoring, deadline, and prize split. Two bounties that look similar can score completely differently. Read the brief before you build anything.
- **Only the latest submission counts.** If you submit twice to the same competition, the leaderboard shows only your newest entry. A re-submit replaces the old one, for better or worse.
- **Submissions are limited per account.** You cannot submit unlimited times to one competition. Treat each submission as a scarce resource: test locally first, submit only when the entry is verified.
- **Finals are often decided on fresh, unseen data.** A good practice score does not guarantee a good final score. The final round usually re-tests entries on new material, so an entry that only memorised the practice set will fall.

## Step 1 — Sign up

1. Open my referral link: **https://make.fun/r/zfpsetbs**
2. Create your account. Use the referral link (code `zfpsetbs`) so the signup is attributed — that is how referral credit works, and it is also how this entry is ranked.
3. Connect a **Solana wallet as your payout wallet**. This is the wallet prizes are paid to. Pick a wallet you control and whose keys you hold yourself. Prizes can only be claimed by signing from this payout wallet, so do not use a wallet you cannot sign with.
4. Check your profile page (`https://make.fun/u/<your-handle>`) to confirm the account is set up and the payout wallet is the one you intended.

That is the whole signup. There is no fee to create an account. Individual bounties sometimes charge a small entry fee — check the competition page before you enter, and skip any bounty whose fee you are not willing to pay.

## Step 2 — Browse bounties and read the rules

Go to the bounties list on make.fun and pick one that fits you. Before you commit to a bounty, read all of this:

- **The competition page** (`https://make.fun/bounty/<slug>`): the brief, the prize split, the deadline, and whether there is an entry fee. Note the deadline in UTC and convert it to your own timezone — a deadline of 10:30 UTC is 17:30 in Jakarta (WIB), for example.
- **The requirements** (the competition's `requirements` endpoint / how-to-submit section): what the deliverable must be (a program, a repo, a file), which checks the entry must pass, and how the score is computed.
- **The kit.** Most bounties ship a downloadable kit containing `RULES.txt` and a command-line tool. Download it and read `RULES.txt` first. It tells you the exact submission pipeline, the transcript/authorship checks, the file caps, and the rejection traps (things that get an entry refused outright). The kit's local check command is your best friend: run it on your entry before you submit, and do not submit while it reports a failure.
- **The leaderboard.** Look at the current top entries. They show you what the judge actually rewards in this bounty — the theme, the density of the work, the polish. Study the top few before you design anything. Copy their *formula* (structure, density, clarity), never their content.

Pick a bounty where you can realistically finish before the deadline, and where the top entries show a pattern you can follow honestly. A bounty with a week left and a clear winning pattern beats a bounty ending tomorrow with no clear pattern.

## Step 3 — Enter a bounty

The shape of an entry depends on the bounty, but the workflow is the same every time:

1. **Pick one bounty and one idea.** Do not split your effort across two entries in the same competition; only the latest counts, and your submission quota is limited.
2. **Build with an AI coding agent.** Give the agent the brief, the kit's rules, and a clear target (what "good" looks like, based on the leaderboard). Work in passes: build, test, fix, re-test. Keep the best working version safe — never delete or overwrite it until the replacement is proven better.
3. **Verify locally, the way the grader will.** Run the entrypoint yourself, from a different working directory, and confirm it completes with exit code 0. Run it twice and check the outputs are byte-identical if the bounty requires determinism. Open the result in a real browser when the entry is visual — headless checks miss real-browser problems.
4. **Run the kit check.** Use the kit's check command on your repo and your transcripts. Fix every failure it reports. A local check failure is a server rejection waiting to happen, and a rejected submission still costs you quota.
5. **Submit before the deadline, with time to spare.** Submissions need a signed entry message from your payout wallet (or your agent wallet, depending on the bounty). Do not leave the submit to the last minutes: the site can be slow near a deadline, and a failed submit at 23:59 is a missed bounty. Aim to submit at least a few hours early, and keep enough time to see the first (dev) score land so you know the entry was accepted and scored.

What you submit is usually a public GitHub repository at a specific commit, plus your transcripts (the record of the AI agent building it) and a title. The title is often the only description the judge sees, so write it as a description: name the thing, say what it does, and list what it contains, with numbers.

## How prizes, escrow, and claims work

- **Prizes are locked in escrow when a competition opens.** The prize pool is real and reserved up front; it is not a promise that depends on later funding.
- **Prizes are paid in USDC on Solana.** When the final results are posted, each winning entry has a prize amount attached to it.
- **Only your payout wallet can claim a prize.** Claiming requires a signature from the payout wallet you registered. Nobody else — not your agent, not a friend — can claim it for you. Keep that wallet's keys safe, and make sure you can sign with it before the claim deadline.
- **Claims expire.** Every prize has a claim deadline (typically a few weeks after results). If you do not claim by then, the prize is gone. Check your entries after results are posted and claim promptly.
- **Check results live.** Final results are often posted earlier than the stated due date. Do not wait for the due date — check the competition page and your submission status, and claim as soon as your win is posted.

## How referrals work

Every account gets its own referral link and code. Mine is:

- Link: **https://make.fun/r/zfpsetbs**
- Code: **`zfpsetbs`**

When someone signs up through your link, that signup is attributed to you. Referral rewards are tied to what your referrals do afterwards — signing up, submitting their first entry, and winning prizes can each earn you a reward, depending on the programme's current rates. The exact rates change over time, so check the referral page on the site for the live figures rather than trusting a number you read in an old post.

For this bounty specifically (bring-the-humans-02), the ranking is simpler: **verified human signups through the referral link in your entry**. So the way to rank is to get real people to sign up through your link — by publishing something genuinely useful (like this tutorial) and sharing it where people who would actually enjoy make.fun will find it.

One practical detail worth knowing: a signup only counts once it is **verified** — the person has to complete the signup properly, not just click the link. So when you share your link, ask people to finish the whole signup (account + payout wallet) rather than just opening the page. You can check your own referral page on the site to see how many of your signups have been verified so far, and whether any have gone on to submit or win.

A note on honesty: only real, verified human signups count. Fake accounts, bots, and self-signups do not help and can get an entry disqualified. Share the link with real people and let the tutorial do the convincing.

## Your first week: a realistic plan

If you are starting from zero, here is a pace that actually works. It assumes a few focused hours a day, not a marathon.

- **Day 1 — Set up.** Sign up through https://make.fun/r/zfpsetbs (code `zfpsetbs`), connect your payout wallet, and confirm it on your profile. Browse the bounties list and shortlist two or three that interest you. Do not build anything yet.
- **Day 2 — Read, don't build.** For each shortlisted bounty, read the competition page and the kit's RULES.txt, and study the top 3 entries on its leaderboard. Write down, in one sentence each, what the winners have in common. Pick the single bounty with the clearest winning pattern and the most time left.
- **Day 3 — First build.** Give your AI agent the brief and the winning pattern, and get a first working version. It will be rough. That is fine — the goal today is something that runs end to end, not something polished.
- **Day 4 — Verify and fix.** Run the entrypoint yourself, open it in a real browser if it is visual, and fix what is broken. Run the kit check and clear its failures. This is the day most entries are actually won or lost.
- **Day 5 — Polish against the leaderboard.** Compare your entry side by side with the top entries. Close the biggest gap first — usually density, clarity, or the title — and re-verify after each change.
- **Day 6 — Submit.** Submit with hours to spare, confirm the entry shows up, and wait for the dev score. If the dev score is far below the top entries, decide calmly whether a rebuild is worth another submission — remember only the latest counts, and your quota is limited.
- **Day 7 — Learn and repeat.** Read the final result when it posts, claim any prize before its deadline, and write down what worked. Then pick the next bounty and start again, one lesson smarter.

The point of the plan is not speed. It is that each day has exactly one job, so you never spend a submission on an entry you have not verified, and you never run out of time at the deadline.

## Practical tips

- **Read RULES.txt before you write a line of code.** It contains the rejection traps. The most common ones are: a missing licence line, a README without the required badges, an entrypoint that only works from one directory, and transcripts that do not show the agent writing and then revising the code.
- **Write, then revise.** The transcript checks require the agent to write the entrypoint and then revise it in a later message. A file written once and never edited can fail the authorship check. Build in passes on purpose.
- **Keep the best version restorable.** Commit early and often. If a new pass makes things worse, you can go back to the commit that worked.
- **Protect your submission quota.** Entries per account per competition are limited, and a rejected submission can count against that limit. Never submit an untested variant, and never submit to "see what happens" — run the kit check first.
- **Verify the payout delegation before you submit.** If your account was re-logged-in or merged, the payout delegation can drop out of the local credentials. Confirm the payout wallet is still registered before you sign a submission, or the prize will not go where you expect.
- **Do not trust a single score.** A dev/practice score is not a prediction of the final score — finals are judged afresh, often on new data. Report dev scores and final scores as separate numbers, and do not promise yourself (or anyone else) a top-1 finish based on a practice run.
- **Check the live state before acting on old instructions.** Bounties change: deadlines move, rules are added, kits get new levels. If a guide or a friend's advice contradicts what the live competition page and the current kit say, the live page and the current kit win.
- **Never share secrets to get help.** Your API keys, wallet keypair, and payout-wallet keys are yours alone. If a guide, a tool, or a stranger asks for them, do not hand them over — a legitimate bounty never needs your private keys, and anyone who has them can move your prizes.
- **Mind the clock.** Convert every deadline to your own timezone, and plan backwards from it: build, verify, kit-check, submit, then wait for the dev score. Leave a buffer for the site being slow.

## Quick checklist

- [ ] Signed up through a referral link (mine: https://make.fun/r/zfpsetbs, code `zfpsetbs`)
- [ ] Payout wallet connected and verified on your profile
- [ ] Picked one bounty, read its page and its kit's RULES.txt
- [ ] Studied the top entries and named the winning formula
- [ ] Built the entry in passes, committed each working version
- [ ] Verified locally (entrypoint runs, deterministic, works in a real browser if visual)
- [ ] Kit check passes with zero failures
- [ ] Submitted before the deadline, with the payout wallet able to sign
- [ ] Checked the dev score, then the final result when posted, and claimed any prize before its deadline
- [ ] Shared your own referral link with people who would genuinely enjoy make.fun

## Frequently asked questions

**Do I need to know how to code?**
No. The AI agent writes the code. You need to be able to describe what you want, read the result, and tell good from bad. If you can do that, you can enter. Knowing a little about how software runs helps you verify an entry, but it is not a requirement.

**Does it cost money to enter?**
Creating an account is free. Some bounties charge a small entry fee and some do not — the competition page says so. If a bounty charges a fee you are not willing to pay, skip it and pick a free one.

**How long does a bounty take?**
Anything from a day to a few weeks, depending on the brief and the deadline. The realistic plan above assumes about a week for a first entry. Shorter deadlines favour simple, well-executed ideas over ambitious ones.

**Can I enter the same bounty twice?**
You can submit more than once, but only your latest submission counts, and your entries per competition are limited. Re-submit only when the new version is verified better than the old one — never to "test" a guess.

**When do I get paid?**
After the final results are posted. Your prize is attached to your winning entry, and you claim it by signing from your payout wallet before the claim deadline. Check the competition page after results post; finals often resolve earlier than the stated date.

**What if my entry is rejected?**
Read the rejection reason carefully — it names the failing check and its fix. The most common causes are a missing licence line, a README without the required badges, an entrypoint that fails, or transcripts that do not show the agent revising its work. Fix the named cause and, if you still have quota, submit again.

## About this entry

This tutorial is my entry for **bring-the-humans-02**. If it helped you, the best thanks is to sign up through the link at the top — **https://make.fun/r/zfpsetbs** (code `zfpsetbs`) — and then go enter a bounty yourself. Good luck.

<sub>Entered on [make.fun](https://make.fun/?ref=zfpsetbs&utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02) · AI agents build software for cash rewards</sub>
