---
title: 🎉 New Web Site Grand Opening!
date: 2025-05-27T13:40:00.000Z
summary: Natixar introduces new ESG and traceability tools
authors:
  - admin
  - jm
tags:
  - Natixar
  - Hugo Blox
image:
  caption: "Bye! Bye! Wix! Image credit: Natixar / S. Cranga"
---
# 🚧 Building Our Site: From Confusion to Creation (and a Few Laughs Along the Way)

Welcome to the backstage tour of how we built a multilingual, dynamic, and modern website—without losing our minds! This is the real-life story of how a state-of-the-art web presence is now within reach, thanks to Hugo, Hugo Blox, Tailwind CSS, Decap CMS, and a little help from AI.

## 🌍 Step 1: Go Global or Go Home

We wanted our site to speak every language our audience might use. Hugo and Hugo Blox made it possible to manage French, English, Portuguese, Chinese, and Spanish — sometimes with just a YAML file, a data folder, and the magic of i18n shortcodes:

With the right shortcodes and the right folder structure, no message gets lost in translation — unless you forget to add the translation file, in which case Hugo lets you know. Loudly.

`{{< i18n "contact_us" >}}`

## ⚡ Step 2: Content That Writes Itself (Almost)

We stopped drowning in markdown files by moving shared info to data files (`/data/contact.fr.yaml` etc.), and teaching our templates to look up the right content depending on language — no more tedious duplication! A sprinkle of smart partials, and voilà:

When in doubt, we debugged with `{{ printf "Lang: %s" .Lang }}` and let AI double-check our logic. Goodbye repetitive copy-paste, hello maintainable content!

```
{{ $lang := .Lang | default "en" }}
{{ with (index site.Data.contact $lang) }}
  {{ .locale.address_format }}
{{ end }}
```





## 🎨 Step 3: Make It Pretty—Responsively

Who knew layouts could be fun? We replaced row and col-12 col-lg-8 from Bootstrap with Tailwind CSS and—when needed—a dash of custom vanilla CSS for those “no-utility-class-for-this” moments. Our pages now reshape themselves gracefully, whether viewed on a smartphone or a cinema screen.

If Tailwind didn’t have the class we wanted, we just added a <style> block using one of the provided hooks — no build step required!

```
@media (max-width: 575px) {
  .responsive-grid { flex-direction: column; }
}
```





## 🤖 Step 4: Let AI Do the Heavy Lifting

Whenever we were stuck (“how do I make this button look good?”), AI stepped in with ready-to-use Tailwind classes, translation help, and tips for internationalization. What used to take an afternoon now takes a coffee break.

## 🔒 Step 5: Easy Editing & Secure Auth

Decap CMS (formerly Netlify CMS) lets us edit content through a user-friendly admin, while Netlify Identity + Git Gateway keeps the process secure (once we got those pesky GitHub OAuth and permissions issues sorted out).

Pro tip: Always double-check your callback URLs, assign the admin role to editors, and don’t forget to invite yourself!

## 🚀 Step 6: Continuous Improvement—With a Smile

We faced obstacles (like empty _index.md files for each language, or Tailwind utility class limitations), but we solved them with clever workarounds, Hugo's data system, and the power of AI-backed teamwork. The result: a fast, beautiful, multilingual site that’s a joy to update.

Ready to build yours?

Just ask AI—or read our chat log for more tips and hacks. 😉
