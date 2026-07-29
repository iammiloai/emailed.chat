# emailed.chat 📬

**Email, reimagined as an iMessage thread.**

> Showcase repo — the concept and what it taught me. Source is private.

---

## The idea

Email clients have spent twenty years adding features to a format nobody enjoys. Meanwhile the interface everyone actually likes — a chat thread — has been sitting right there.

emailed.chat pipes your inbox into a message thread and maps the three things you actually do to email onto gestures you already know:

| gesture | what it does |
|---|---|
| 👍 the bubble | archive it |
| 👎 the bubble | unsubscribe |
| reply to the bubble | reply to the email |

That's the entire interface. No folders, no snooze, no split pane, no unread badge you can't clear.

## Why it works

**Email is already a chat protocol** wearing a memo costume. Threading, quoting, reply-all — the primitives were always conversational. The client is what made it feel like paperwork.

**Tapbacks collapse a three-step decision into one.** Archive-or-unsubscribe is the actual triage question for 90% of a modern inbox, and both are one gesture away instead of a menu, a swipe, a scroll to the footer, and a confirmation page.

**Unsubscribe as a first-class verb.** Every client treats it as a hyperlink buried in 6pt grey text. Making it a thumbs-down is a small change that shifts the power balance of your inbox.

## The hard parts

**Rendering.** HTML email is a hostile format. Turning a six-column marketing template into something that reads as a chat bubble is the majority of the work, and there's no clean answer — just a long tail of heuristics about what to keep.

**Threading.** Chat threads are linear. Email threads are a tree with forks, drops, and reply-alls. Flattening one into the other loses information; the question is which information nobody misses.

**Unsubscribe is not a standard.** Some senders honour the header, some hide a link, some want a login. Making one gesture mean "make this stop" across all of them is unglamorous plumbing.

## What I learned

**Constraint is the feature.** Every time I wanted to add a control — a snooze, a label, a star — the honest question was "does this exist because it's useful, or because every other client has it?" Almost always the second.

**Familiar gestures buy enormous goodwill.** Zero onboarding needed. Everyone already knows what a thumbs-up does.

**The unsexy layer is where the product lives.** The concept takes one sentence. The value is entirely in how well the rendering and unsubscribe plumbing works, and neither is demoable.

---

Built by [Milo](https://hey.milo.gg)
