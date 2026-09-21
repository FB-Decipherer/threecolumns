# Three Columns

A website format for one topic at a time, built on three depths: **plain answers**,
**previewed sources**, and **full technical detail** — so one topic serves two readers
at once, the newcomer who knows nothing about it and the reader who already knows the
subject well, without either of them wading through the other.

Its second idea is about footnotes. Instead of being buried at the foot of a page,
tucked behind a link, or scattered wherever they fall, every reference is gathered into
one column of its own — centered in the layout and always in the same place.

They are three columns wherever they will fit as three columns. On a wide screen they sit
side by side. On a phone they stack and you read one at a time. In print they become one
document. And where one column holds more than any column can — an entire municipal code,
say — it is given its own page, as at worland-dog-law.online. Stacked, paged or side by
side, it is the same three.

Live: **https://threecolumns.online**

## Why

Most sites serve one reader and make the others work for it. A customer scrolling
past technical specifications stops reading; a specialist scrolling past an
explanation of basic terms also stops reading.

The middle column is the part nobody else does. Every external source gets a card
that says what it is, who made it, what you would find there, and what it is doing
on this page — **with the link last**, deliberately. When the link came first,
readers clicked it and never read the preview, which defeated the whole column.

## What it costs, and what it can't do

The domain, and nothing else. Hosting is GitHub Pages; the certificate is issued
automatically. Nobody has promised free hosting forever, and the protection against
that is structural rather than contractual: this is a handful of plain files that
could be moved to any other static host in an afternoon, unchanged.

It is hard to compromise because there is nothing to attack — no database, no login,
no forms, no server code, no plugins, no cookies. Nothing in it has a version number,
so nothing in it can become an old version.

## The files

| file | what it is |
|---|---|
| `index.html` | the public page — columns A, B, C |
| `setup.html` | page D — the setup sheet. Unlinked, noindex. Not an admin panel: a form that produces text you paste into a file. |
| `domain.html` | page E — standing up a domain, step by step. Unlinked, noindex. |
| `links.json` | link-health status: the date of the last check and any dead links. Written by whoever ran the check — by hand on this site, since no scheduler is wired up yet. If absent, the page says nothing about link health — no file, no claim. |
| `phone-view.js` | Phone view: shows the page in a phone-sized frame. For every reader here, because the page's own button carries `data-public`; on a site made from the format, hidden unless the address carries `?dev`. |
| `top-button.js` | the round up-arrow button that returns to the top, once the reader has scrolled about a screen down |
| `back-link.js` | the Back button on a source card, returning to the numeral that opened it |
| `masthead-sitemap.svg` | the picture at the head of the page: the map of the site family, with which way each link points |
| `social.png` `apple-touch-icon.png` | the share card and the home-screen icon |
| `favicon.svg` `robots.txt` `sitemap.xml` `404.html` | the usual furniture |

The browser checks behind column C's *Quality assurance* are kept in
`Three Columns Tools/qa/` (60 checks as of 21 September 2026).

The three scripts are the same files on every site that carries them. Change one in
`Three Columns Tools/template/` first, then copy it out, so no copy drifts from the others.

## Publishing

Edit `index.html`, open GitHub Desktop, type one line saying what changed, click
**Commit**, then **Push**. Live in about a minute. Two words to learn; branches and
pull requests can be ignored indefinitely.

`domain.html` walks through the domain setup once, with every value filled in.

## Using it yourself

MIT licensed — copy it, change it, sell work built with it, no permission needed.
If you do something interesting with it, saying so is welcome and not required.

Walter Wilkinson · Worland · Washakie County · Wyoming
