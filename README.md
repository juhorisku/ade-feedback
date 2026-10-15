# ade-feedback

This is where people who try ADE tell us what went wrong, or what could be better. It holds no
code: only the reports you write.

## How to tell us something

The easiest way is from ADE's own window: choose **Report a problem**. Your browser opens a new
report here with ADE's version, the window's build and your Windows version already filled in.
Nothing is sent until you press **Submit new issue** yourself.

You can also start here: choose **Issues**, then **New issue**, and **Tell us something**.

There is one form for everything. It asks first what your report is about -- something broken,
a feature request or an idea, the window, a question, or something else -- and then what you
would like to tell us. The other boxes are optional: for something broken, what you expected,
how to make it happen again, and how often it does; for the window, where in it you mean.

A picture of the screen often says more than words: drag it into the picture box, or paste it
there.

## What not to put here

This repository is public: anyone can read what is in it -- the words and the pictures, which
are published the moment you submit. The form asks you to confirm that before it sends. Please
leave out anything secret (passwords, keys, private code) and anything about
other people (their names, their email, what was on their screen). If a picture shows something
like that, crop it or leave it out.

## What happens next

We read every report. A report is not a promise of a change: when we take one up, we say so on
it, and we close it when the change is in a version of ADE you can install.

## For whoever looks after this repository

- The form is `.github/ISSUE_TEMPLATE/feedback.yml`, one for every kind of report: its first
  field, `about`, says which kind it is. Issue forms have no conditional fields, so every field
  only some kinds need is optional. `config.yml` turns off reports that do not use a form.
- ADE's window fills three fields of the form from the address it opens: `version`, `build`
  and `os`. Keep those three ids as they are, or the window's link stops filling them.
- The form is written in a plain, regular YAML style -- two spaces a level, a list item as
  `- key: value`, longer text as `value: |`, no tabs, no comments after a value -- because ADE's
  tests read it with a small reader of their own. Keep to it when you edit it.
- ADE learns where this repository is from its configuration, `feedback_repository` as
  `owner/name`. Nothing in ADE assumes whether the repository is private or public.
