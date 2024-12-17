# WordColorStroop

### Word Color Stroop
The Word Color Stroop (WCS) paradigm is designed to involve inhibition cognitive behavior, eliciting functional brain activity in the dorsolateral prefrontal cortex. There are many different type of stroop paradigms (such as emotional stroop tasks). This one presents the name of colors (in english) on screen, with the font color often not agreeing with the meaning of the word itself. The task requires the observer's cognitive inhibition processing in order to accurately interact with it. This particular WCS was modified based off work by Jahani, _et al._, and was set up for an experiment using fNIRS to capture brain activity.
`https://doi.org/10.1109/ICBME.2015.7404124`

<img width="166" alt="Image" src="https://github.com/user-attachments/assets/2bb234c9-2e7c-4c03-b49b-b4446a0da2ef" />

<img width="163" alt="Image" src="https://github.com/user-attachments/assets/f1fbf1da-8f81-497f-b66f-d5a5da53950e" />

### Paradigm Setup
**Intro**
Instructions for Easy/Congruent task. 2 practices with feedback (untimed).
Instructions for Difficult/Incongruent task. 2 practices with feedback (untimed).

**Run**
Initial Rest (20s)
18 blocks (9 Easy/Congruent, 9 Difficult/Incongruent) in randomized order

Each block:
6x3s trial
10-15s jittered rest

**Easy/Congruent Condition:**
One of the words has matching font color and meaning. The other word does not.
Designed so the two words are never the same meaning or same font color.

**Difficult/Incongruent Condition:**
The prompt word meaning and font color never match.
The three option words have different meanings from one another.
The three option words' meaning and font color never match.

### Specifications, may need modification for user needs

- This was primarily run with PsychoPy version 2022.1.1. PsychoPy downloads and information can be found here.:
`https://www.psychopy.org/download.html`
- The "Begin Experiment" tab of code_3 in "Intro_Easy" Routine, + the "Begin Routine" tab of code_2 in "SendTrigger" Routine +  "marker" column of "rows.xlsx" spreadsheet are set up to send a block onset stimulus marker on recorded data by Aurora (NIRx, Germany) via LSL.
- WCS was run on a T495s ThinkPad. For different monitors, PsychoPy screen settings may need to be altered to display correctly.
