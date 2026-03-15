# The Lead Meeting Miner

**Your meetings are full of gold. You just forget to write it down.**

Last week I had a 30-minute call with Victor, my co-founder. He said five things I could have turned into LinkedIn posts.

I remembered zero of them by dinner.

That's why I built this.

Paste any meeting transcript into Claude Code. Get back one clean file with everything worth keeping:

**Content Stories** — The stuff you'd screenshot if it was in a group chat. One-liners, reactions, results. Ready to post.

**Action Items** — Who said they'd do what. Grouped by person. No more digging through a 45-minute recording.

**Client Notes** — Decisions made, questions left open, numbers mentioned. Organized by topic so you can find it later.

Works with Zoom, Google Meet, Teams, Fireflies, Otter, or any transcript you can copy-paste.

## How We Use It

We're building Sucana, an AI analytics platform for lead gen agencies. Every week we run the Meeting Miner on our team calls.

Here's what it pulled from a real call between me and Victor (he runs a PPC agency):

> **The moment:** Victor says: "Instead of selling people, the good ones just create content, attract, and sell in the back end in the comments. The offer is not public."
>
> *Why it's content: The shift from pricing pages to back-channel selling. Every marketer has seen it. Few have named it this clearly.*

One 30-minute call gave us 5 content angles, 7 action items, and 4 topics with clear decisions.

Full example: [example-output.md](example-output.md)

## Setup (Simple)

Works in Claude.ai, Claude Co-Work, or any AI chat. No terminal. No install.

**1.** Copy the contents of [SKILL.md](the-lead-meeting-miner.skill/SKILL.md)

**2.** Open Claude. Paste the SKILL.md first, then paste your meeting transcript below it.

**3.** Type: "run meeting miner"

**4.** Claude reads the instructions, mines your transcript, and gives you the three sections.

Copy the output into a new doc. Done.

## Setup (Advanced)

For Claude Code CLI users. The skill auto-detects and saves the output to a file for you.

**1.** Clone this repo:

```
git clone https://github.com/yours2grab/the-lead-meeting-miner.git
```

**2.** Open Claude Code inside the folder:

```
cd the-lead-meeting-miner
claude
```

**3.** Paste your transcript and say:

```
run meeting miner
```

**4.** Your notes land in one file: `meeting-notes-YYYY-MM-DD.md`

## Getting Your Transcript

The Meeting Miner works with any text transcript. Here's how to get one:

**Zoom** — Enable "Audio Transcript" in settings. After your meeting, download the .vtt file from your Zoom recordings. Copy-paste the text.

**Google Meet** — Turn on captions during the call. After the meeting, the transcript shows up in your Google Drive inside the meeting folder. Open it, copy the text.

**Microsoft Teams** — Click the three dots during a meeting → "Start transcription." After the call, find the transcript in the meeting chat. Copy it.

**Otter.ai** — Otter records and transcribes in real-time. Export the transcript from your Otter dashboard as text.

**Any other tool** — If your tool gives you a text file with who said what, it works. The Meeting Miner just needs readable text with speaker names.

**No transcription tool?** Record your meeting (phone, Zoom, any recorder), then upload the audio to a free transcription service like Otter.ai or Fireflies.ai. They'll give you the text.

## Bonus: Fireflies Auto-Pull

If you use Fireflies.ai, you can skip the copy-paste entirely.

Fireflies has a direct MCP integration with Claude. That means the Meeting Miner can pull your latest transcript automatically. No copy-paste. No exporting files.

**How to connect:**

1. In Claude Code, connect your Fireflies account through the MCP settings
2. Once connected, just say: "pull my latest Fireflies transcript and run meeting miner"
3. Done. It grabs the transcript and mines it in one step.

This is how we run it every week. Fireflies records the call, we open Claude Code, one command, meeting mined.

Right now Fireflies is the only transcript tool with this direct integration. All other tools work fine with copy-paste.

## Built by The Lead

The Lead is a weekly newsletter for marketers who use AI. Every Friday, one real workflow from inside our build.

[Join The Lead →](https://sucana.ai)
