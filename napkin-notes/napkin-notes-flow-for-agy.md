# Napkin Notes production flow — for review

Draft v0.1, 2026-10-14. Written for a second reviewer (agy). Items marked (assumed) were guessed by the author and may be wrong.

## Context

Napkin Notes is a YouTube channel about money psychology, using narrated napkin-style illustrated scenes (assumed). One owner approves at defined gates; AI agents and tools do everything else. There are two flows: a long video flow (A) and a Shorts flow (B) that cuts clips from the approved long video (assumed).

Legend: **GATE** = owner must approve. **AGENT** = agent doing judgement work. **ROUTINE** = automated, same every time, no review.

## Flow A — Long video

### Phase 1 · Research to locked script

| # | Step | Type | Who/tool | Takes in | Hands on | Notes |
|---|---|---|---|---|---|---|
| A1 | Weekly trend pull | ROUTINE | VidIQ | Seed keywords, competitor channels | Outlier videos, rising keywords, trending money topics | Scheduled. Needs nothing from you. Cadence assumed weekly. (assumed) |
| A2 | Score and shortlist ideas | AGENT | Research agent | Trend data, Napkin Notes Channel Archive, HOLD list | 5 ranked idea cards: angle, why now, VidIQ scores, overlap warning, one recommended pick | Drops anything that repeats a posted video. |
| A3 | Pick topic | GATE | Owner | 5 idea cards | Approved topic and angle | You decide: take the recommended one, pick another, or ask for a fresh five (back to A2 with your note). Aim for a one-minute decision.; loops back to A2 (fresh five) |
| A4 | Draft outline and script | AGENT | Script agent | Approved angle, your voice and format notes | Hook, outline, full script, list of factual claims with sources | The claims list is what you check at A5. The fact-check list is my addition. (assumed) |
| A5 | Approve script | GATE | Owner | Script and claims list | Locked script | You decide: hook, tone, facts. Reject sends it back to A4 with your comments. After this point every change costs voice and image credits, so this is the last cheap place to change your mind.; loops back to A4 (revise) |

### Phase 2 · Voice, transcript and images

| # | Step | Type | Who/tool | Takes in | Hands on | Notes |
|---|---|---|---|---|---|---|
| A6 | Voiceover | ROUTINE | ElevenLabs or you | Locked script | Narration audio | Confirm whether you record it or ElevenLabs speaks it. (assumed) |
| A7 | Transcribe with timestamps | ROUTINE | ElevenLabs | Narration audio | Word-level timestamped transcript | If the voice is generated from the locked script you already have the text and only need the timing. See O5. |
| A8 | Clean and split into scenes | AGENT | Storyboard agent | Transcript | Scene list: start and end time, spoken line, visual idea |  |
| A9 | Write napkin image prompts | AGENT | Storyboard agent | Scene list, locked napkin style guide | One prompt per scene, same style prefix on every prompt | The style guide is what keeps the look the same from video to video. |
| A10 | Generate images | ROUTINE | Higgsfield | Prompts | 1 to 3 variants per scene | Spends credits. Confirm which generator you use. (assumed) |
| A11 | Pre-check images | AGENT | QA agent | All variants, scene list | Contact sheet marking each scene pass or flag: style drift, misspelt text, duplicates, wrong aspect ratio | Saves you from looking at obvious failures. |
| A12 | Review images | GATE | Owner | Contact sheet | One approved image per scene | You decide: accept the passes, pick a variant, or send flagged scenes back. The loop goes to A9 to fix the prompt, or straight on to A10 for a plain reroll.; loops back to A9 (fix prompt or reroll) |

### Phase 3 · Edit, package, publish

| # | Step | Type | Who/tool | Takes in | Hands on | Notes |
|---|---|---|---|---|---|---|
| A13 | Assemble the cut | AGENT | Editor agent | Approved images, audio, transcript | Draft video: timing, captions, motion, music | Which editing tool does the assembly is not known to me. (assumed) |
| A14 | Watch final cut | GATE | Owner | Draft video | Approved cut | You decide: pacing, caption accuracy, audio levels. Reject sends timestamped notes to A13.; loops back to A13 (fixes) |
| A15 | Title, thumbnail, description | AGENT | Metadata agent | Locked script, approved cut | 3 scored titles, thumbnail options, description, chapters, tags | Scores come from VidIQ. This only needs the script, so it could start earlier (O1). |
| A16 | Pick title and thumbnail | GATE | Owner | Scored options | Approved metadata | You decide: title, thumbnail, description. Could be one sitting with A14.; loops back to A15 (redo) |
| A17 | Schedule and upload | ROUTINE | VidIQ | Approved cut, approved metadata | Scheduled YouTube video | The only step that publishes the long video. It cannot run until A14 and A16 are approved. |
| A18 | Archive and log | ROUTINE | Google Drive | Final files | Assets saved in Napkin Notes Channel Archive, tracker row updated |  |

### Phase 4 · After it is live

| # | Step | Type | Who/tool | Takes in | Hands on | Notes |
|---|---|---|---|---|---|---|
| A19 | Pull 48h and 7-day stats | ROUTINE | VidIQ | Published video | Views, retention, click-through, comments |  |
| A20 | Triage comments, draft replies | AGENT | Community agent | Comments | Reply drafts, flagged questions and complaints |  |
| A21 | Approve replies | GATE | Owner | Reply drafts | Replies sent | You decide: send, edit, skip. Nothing is posted as you without this.; loops back to A20 (edit) |
| A22 | Weekly insights for next topics | AGENT | Analyst agent | Stats from A19 and B11 | What topics, hooks and thumbnails worked | Closes the loop: this is what makes next week's A2 shortlist better. |

## Flow B — Shorts

### Phase 1 · Find the clips

| # | Step | Type | Who/tool | Takes in | Hands on | Notes |
|---|---|---|---|---|---|---|
| B1 | Final cut and transcript ready | ROUTINE | Google Drive | Approved cut from A14, transcript from A7 | Trigger: Shorts work starts | Assumes Shorts are cut from the long video. Starting at A14 approval, rather than after publish, is O6. (assumed) |
| B2 | Find 3 to 6 clip moments | AGENT | Clip-scout agent | Transcript, cut | Candidates: start and end, hook line, why it should work | VidIQ clip tools may suggest moments. (assumed) |
| B3 | Dedupe against posted and HOLD | AGENT | Clip-scout agent | Candidates, Money Video Clips, HOLD folder | Keep list. Overlaps go to HOLD with the reason | Automates what the 'HOLD - already posted or overlaps' folder does by hand today. |
| B4 | Pick clips | GATE | Owner | Keep list with timestamps | Approved clip list | You decide: which go ahead, which wait. Best done in a batch across several videos (O7).; loops back to B3 (re-scout) |

### Phase 2 · Produce and score

| # | Step | Type | Who/tool | Takes in | Hands on | Notes |
|---|---|---|---|---|---|---|
| B5 | Cut, reframe 9:16, captions | AGENT | Editor agent | Approved clips | Vertical drafts with burned-in captions | Higgsfield reframe or Shorts Studio are the tools I would try. (assumed) |
| B6 | Hook text, title, caption, tags | AGENT | Metadata agent | Vertical drafts, transcript | Copy for each platform |  |
| B7 | Hook score | ROUTINE | Higgsfield predictor | Vertical drafts | Score and pass or fail against a threshold | A fail goes back to B5 once, automatically. A second fail is flagged to you. The threshold still needs setting. (assumed); loops back to B5 (retry once) |
| B8 | Batch review | GATE | Owner | All passed Shorts on one sheet | Approved batch | You decide: yes, fix, or drop for each Short. Fixes go to B5 with your note.; loops back to B5 (fix) |

### Phase 3 · Post and learn

| # | Step | Type | Who/tool | Takes in | Hands on | Notes |
|---|---|---|---|---|---|---|
| B9 | Schedule posts | ROUTINE | YT · TikTok · Reels | Approved batch | Scheduled on each platform | The only step that publishes Shorts. Staggered times. Confirm which platforms you post to. (assumed) |
| B10 | File and number | ROUTINE | Google Drive | Posted Shorts, thumbnails | NN_slug.mp4 in Money Video Clips, thumbnail saved, tracker updated | Matches your current naming, like 01_trap-spending-matches-income.mp4. Overlaps stay in HOLD. |
| B11 | Pull 48h stats | ROUTINE | VidIQ | Posted Shorts | Views, watch time, swipe-away rate |  |
| B12 | Rank hooks, flag winners | AGENT | Analyst agent | Stats from B11 | Which hooks and topics earn their own long video |  |

## Agents

- **Research agent** (A2): Shortlists and ranks topic ideas, checks them against what is already posted. Tools: VidIQ, Drive. Never: Pick a topic.
- **Script agent** (A4): Drafts hook, outline, script and claims list. Tools: Claude. Never: Lock a script.
- **Storyboard agent** (A8, A9): Turns the transcript into scenes and writes the napkin image prompts. Tools: Claude. Never: Generate images itself.
- **QA agent** (A11): Checks generated images against the style guide and flags failures. Tools: Vision model. Never: Approve an image.
- **Editor agent** (A13, B5): Assembles the long video and cuts vertical Shorts. Tools: Editing tool, Higgsfield. Never: Approve a cut.
- **Metadata agent** (A15, B6): Writes titles, descriptions, thumbnails, hooks and tags and scores them. Tools: VidIQ. Never: Pick final title or thumbnail.
- **Community agent** (A20): Drafts comment replies. Tools: VidIQ comments. Never: Send a reply.
- **Clip-scout agent** (B2, B3): Finds Short-worthy moments and removes overlaps. Tools: VidIQ, Drive. Never: Choose clips.
- **Analyst agent** (A22, B12): Turns stats into what to make more or less of. Tools: VidIQ. Never: Change the strategy alone.

## Optimisation ideas already proposed (do not just repeat these)

- **O2 Make image review exception-based** (A11, A12; impact High, effort Medium): Image review is probably the longest wait on you. Have the QA agent build a contact sheet, default every passing scene to approved, and ask you only about flagged scenes.
- **O3 Lock the napkin look** (A9, A12; impact High, effort Medium): Keep one style guide, one set of reference images and one fixed prompt prefix. Consistent output means fewer rejected scenes at A12.
- **O7 Review Shorts in a weekly batch** (B4, B7, B8; impact High, effort Small): One sitting for 10 to 12 Shorts instead of a review per video. Auto-drop anything under the hook-score threshold before it reaches you.
- **O9 One status tracker** (A18, B10, all gates; impact High, effort Medium): Give every video and every Short a row with a status. Agents read and write it, a gate is just 'set to approved', and you get a nudge when something has waited on you for a day. Today state seems to live in folders.
- **O1 Merge the two final reviews** (A14, A15, A16; impact Medium, effort Small): Metadata only needs the locked script, so A15 can run while the cut is being assembled. Then A14 and A16 become one sitting: watch the cut, pick the title and thumbnail.
- **O4 Turn the topic gate into a 60-second decision** (A2, A3; impact Medium, effort Small): Hand over one card with a recommended pick and the overlap check already done. 'Approve recommended' becomes the default action.
- **O5 Skip or shrink transcription if the voice is generated** (A6, A7; impact Medium, effort Small): If ElevenLabs speaks the locked script, you already have the text. Check whether it can return word timings, and only run full transcription for audio you record.
- **O6 Start Shorts before the long video publishes** (B1, A17; impact Medium, effort Small): Begin clip scouting when the cut is approved, in parallel with metadata and upload, so Shorts can go out on day one or two.
- **O10 Add a fact-check pass at the script gate** (A4, A5; impact Medium, effort Small): Money content lives on credibility. Have the Script agent list each claim with a source so you can approve the facts, not just the tone. Some popular stories, such as lottery winners going broke, are widely repeated but poorly supported.
- **O11 Close the learning loop** (A22, B12; impact Medium, effort Small): A monthly digest of winning hooks, topics and thumbnails goes into the Research, Script and Metadata agents' instructions, so each video starts smarter.
- **O12 Cap regeneration loops** (A10, A12; impact Medium, effort Small): Allow, say, three rerolls per scene. After that the scene goes to you with a note rather than quietly burning credits.
- **O8 Auto-handle routine comments** (A20, A21; impact Low, effort Medium): Let the Community agent reply on its own to thanks and simple questions from an allow-list, and bring only the awkward ones to you.

## Assumptions

- The videos are narrated with napkin-style illustrated scenes, not on camera. I inferred this from 'transcription' and 'image generation review'.
- The voice is either generated by ElevenLabs from the script or recorded by you. The flow differs; see O5.
- Images come from Higgsfield. It could be ElevenLabs, Napkin AI or something else.
- I don't know which tool assembles the final video.
- Shorts are cut from the long video. I inferred this from the numbered clips in 'Napkin Notes - Money Video Clips'. If you also make standalone Shorts, that is a third flow.
- Shorts go to YouTube, TikTok and Instagram Reels. Confirm which you really use.
- The nine agents are my proposed split of the work. Map them onto the agents you really run.
- Cadence (videos and Shorts per week) and how long each gate takes you are unknown, so the impact ratings on the optimisation list are judgement, not measurement.

## Prompt for the reviewer

You are reviewing a content-production workflow for a solo creator who is the only human approver. Read the flow above, then:

1. Find the three largest bottlenecks on the creator's time and say which steps cause them.
2. Name any step that is redundant, could be merged, or could run in parallel with another. Give step IDs.
3. Judge each GATE: is it in the right place, is it needed, and could it be exception-based or batched instead?
4. List failure modes: what goes wrong silently (wrong facts, style drift, duplicate Shorts, credits burned in loops, wrong thing posted) and which step should catch it.
5. Say which agent boundaries look wrong (an agent doing too much, or two agents that should be one).
6. Review the ideas O1 to O12 above: which would you drop, which would you rank higher, and what is missing?
7. Say what you would need measured (time per gate, rejection rate per scene, cost per video) to rank improvements properly.

Answer as: a ranked table of changes (change, steps affected, expected saving, risk), then a short list of questions for the creator.
