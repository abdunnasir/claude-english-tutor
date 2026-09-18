# claude-english-tutor

A Claude Code skill that reviews an English sentence for grammar and
word-choice errors, explains what's wrong and why, and gives a corrected
version — built for ongoing English practice.

## Install

npx skills add abdunnasir/claude-english-tutor -a claude-code -g -y

## Usage

Invoke `/english-coach` in Claude Code, then give it a sentence to check.

## What it does

Point it at a sentence and it flags grammar, word-choice, and register
issues — explaining *why* each one is wrong, not just what to change —
then gives you a corrected sentence.

**Example**

Input: `We see a doctor today as Tim was not feeling well.`

- **"We see"** — wrong tense. The sentence describes a past event, so the
  verb must be past tense.
  - Fix: **"We saw"**

**Corrected sentence:** We saw a doctor today as Tim was not feeling well.

### Kinds of fixes it catches
- **Verb tense errors** — "We see a doctor today" → "We saw a doctor today"
- **Word choice / register** — "not feeling good" → "not feeling well"
- **Preposition and article mistakes** — "good in English" → "good at English"
- **Awkward phrasing** — "I am having a doubt" → "I have a doubt"
