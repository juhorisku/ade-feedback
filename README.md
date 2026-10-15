# ade-feedback

This is where people who try ADE tell us what went wrong, or what could be better. It holds no
code: only the reports you write.

## How to tell us something

The easiest way is from ADE's own window: choose **Report a problem**. Your browser opens a new
report here with ADE's version, the window's build and your Windows version already filled in.
Nothing is sent until you press **Submit new issue** yourself.

You can also start here: choose **Issues**, then **New issue**, and pick one of the two forms.

- **Something went wrong** -- ADE did something it should not have, or did not do something it
  should have. Say what happened, what you expected, how to make it happen again, and how often
  it does.
- **Something about the window** -- a part of the window is unclear, awkward, or could look or
  work better. Say where, and what would have helped.

A picture of the screen often says more than words: drag it into the picture box, or paste it
there.

## What not to put here

This repository is public: anyone can read what is in it -- the words and the pictures, which
are published the moment you submit. Each form asks you to confirm that before it sends. Please
leave out anything secret (passwords, keys, private code) and anything about
other people (their names, their email, what was on their screen). If a picture shows something
like that, crop it or leave it out.

## What happens next

We read every report. A report is not a promise of a change: when we take one up, we say so on
it, and we close it when the change is in a version of ADE you can install.

## For whoever looks after this repository

- The forms are in `.github/ISSUE_TEMPLATE/`: `bug.yml` and `ui-feedback.yml`. `config.yml`
  turns off reports that do not use a form.
- ADE's window fills three fields of either form from the address it opens: `version`, `build`
  and `os`. Keep those three ids as they are, or the window's link stops filling them.
- The forms are written in a plain, regular YAML style -- two spaces a level, a list item as
  `- key: value`, longer text as `value: |`, no tabs, no comments after a value -- because ADE's
  tests read them with a small reader of their own. Keep to it when you edit them.
- ADE learns where this repository is from its configuration, `feedback_repository` as
  `owner/name`. Nothing in ADE assumes whether the repository is private or public.
