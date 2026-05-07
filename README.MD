# jsitor: The Day My Code Disappeared: A Warning About Trusting Online Editors With Your Work

I lost all my code today. Not because of my mistake. Not because I deleted anything. Simply because I trusted a platform that wasn't ready to be trusted.

I'm writing this not out of anger, but out of responsibility — because no one should go through this without a warning.

---

## The False Sense of Synchronization

JSitor uses GitHub OAuth for authentication. You log in with your GitHub account, and everything feels familiar, connected, safe. That single UX decision creates a powerful — and completely false — psychological impression: that your code is somehow tied to GitHub, backed up, versioned, protected.

It isn't.

The GitHub login is nothing more than an identity provider. Your snippets live exclusively in JSitor's own database. There is no sync. There is no repository. There is no safety net. The GitHub connection is a door key, not a vault.

I only understood this after everything was already gone.

---

## What Actually Happened

In late December 2025, the JSitor creator pinned an issue on GitHub with the following statement:

> *"Unfortunately, it seems like our application was a victim of cyber attack. This has lead to impacting a significant amount of snippets data (html, css, js). The attacker seems have taken control of our database via some means and deleted some records. We are investigating the issue. We are extremely sorry for this issue."*

The snippets still appear in the repository. The thumbnails — static screenshots from the last time each snippet was executed — are still there, like tombstones marking where code used to live. But open any snippet and every editor panel is empty. The HTML is gone. The CSS is gone. The JavaScript is gone.

The post is from December 2025. There has been no follow-up about recovery. No mention of backups being restored. No timeline. Silence.

That silence is the most telling part of all.

---

## The Uncomfortable Truth About "Free" Online Editors

Tools like JSitor, CodePen, JSFiddle and similar platforms are extraordinary for quick prototyping, sharing ideas, and learning in public. But most of them share a structural vulnerability that we collectively choose to ignore: they are small operations, often maintained by one person or a tiny team, with infrastructure costs that don't scale with the trust users place in them.

When things go well, they feel like professional tools. When things go wrong, you discover they were always a single point of failure.

No redundancy. No disaster recovery plan. No SLA. No obligation to your data whatsoever.

We accept these terms because the tools are convenient and free. And then we're surprised when the bill finally comes — not in dollars, but in lost work.

---

## What I Should Have Done Differently

The answer is embarrassingly simple in retrospect: treat every online editor as a scratch pad, never as a repository.

Every snippet worth keeping should have a permanent home in a real Git repository under your own control. The workflow should be: write locally, push to GitHub, optionally paste into an online editor to share or demonstrate. Never the other way around.

The online editor is a window. GitHub is the house. I had been living in the window.

---

## A Note to Tool Creators

If you build a platform where developers store their work — even informally, even in "snippets" — you are holding something irreplaceable. Code represents hours of thinking, experimentation, and problem-solving. It represents professional history.

This is not a responsibility you can take lightly. At minimum, users deserve transparent communication about how their data is stored, what backup policies exist (or don't), and what happens in a worst-case scenario. They deserve to know upfront that a GitHub login does not mean GitHub protection.

Transparency isn't a weakness. The absence of it, however, is a breach of trust.

---

## Final Words

I'm not here to condemn JSitor or its creator. Building and maintaining a public tool alone is hard, and attacks happen. But the combination of an implied safety that doesn't exist, no backup recovery, and months of silence after a data loss event is a pattern the developer community needs to talk about openly.

If this post saves even one person from losing their work, it was worth writing.

Back up your code. Own your data. Trust convenience tools for what they are — convenient, and nothing more.

---

*Published on GitHub as a public record. May 2026.*

---
> **Note:** This page contains 1 cross-origin iframe(s) that could not be accessed due to browser security policies. Some content may be missing. Links to these iframes have been preserved where possible.


---
Source: [Bug: Código dos snippets desapareceu. | Inner AI](https://app.innerai.com/?sessionId=a05ef390-3295-4dbe-9f7e-da7ea98f4898)
