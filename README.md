# Sh.Milandhoo MTCC Site Tracker

Source for the site tracker published as a claude.ai artifact:
https://claude.ai/artifact/RwQcVqzKjE9mB24iumdKEc

- `site-tracker/index.html` — the whole app (HTML, CSS, JS and embedded fonts/logo in one file).

## Modules

Tasks, Consumption, Petty cash (Prj-00544, Prj-00947), Attendance, Overtime,
Staff issues, Material issues, Machinery, Admin panel. English and Dhivehi.

## Runtime

The page runs only inside claude.ai and uses these artifact capabilities:

- `db` — shared database holding all records (users, tasks, entries, attendance, …)
- `downloads` — CSV exports
- `user` — viewer identity

The records live in the artifact's database, not in this repo. This repo
holds the code only.

## Publishing

Edit `site-tracker/index.html`, then republish it to the artifact URL above
(keeping the `db`, `downloads` and `user` capabilities). The page is stored
without the `<!doctype html><head>…<body>` wrapper; the artifact service adds
that at publish time.

Dhivehi text uses AK Liyan by Akuru Type, embedded under the SIL Open Font
License 1.1 (license text is in the page's stylesheet).
