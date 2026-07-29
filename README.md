# emailed.chat

Your email as a chat. This is my main product.

[emailed.chat](https://emailed.chat)

Write-up, not source code.

## What it is

Email in a thread that looks and works like iMessage. The three things you actually do with email are mapped to gestures you already know:

| gesture | what happens |
|---|---|
| thumbs up | archive it |
| thumbs down | unsubscribe |
| reply | reply to the email |

That's the whole interface. No folders, no snooze, no split pane, no unread count you can never clear.

## Why I built it this way

Email clients have spent twenty years adding features to a format nobody enjoys. The interface people actually like, a chat thread, was sitting right there the whole time.

Two things I felt strongly about:

**Unsubscribe should be one tap.** Every email client treats it as a link buried in tiny grey text at the bottom. Making it a thumbs down changes who's in charge of your inbox.

**Fewer controls, not more.** Every time I wanted to add a snooze or a label or a star, the honest question was whether it's useful or whether every other client just has one. Usually the second.

## The hard parts

**Making emails look like messages.** HTML email is a mess. Turning a six column marketing template into something that reads as a chat bubble is most of the work, and there's no clean solution, just a lot of rules about what to keep and what to throw away.

**Threads.** A chat is a straight line. An email thread is a tree with forks and reply-alls. You lose something flattening one into the other, and the job is picking what nobody will miss.

**Unsubscribe isn't a standard.** Some senders respect the header, some hide a link, some make you log in. Getting one gesture to mean "stop" across all of them is unglamorous work, and it's where most of the value is.

## What I learned

The idea takes one sentence. Everything that makes it good is in the boring layer underneath, and none of that demos well.

---

Built by [Milo](https://milo.gg)
