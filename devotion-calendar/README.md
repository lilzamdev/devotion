# Mt. Calvary Devotion Calendar

Daily devotion calendar for the Mt. Calvary MBC youth.
Static site (GitHub Pages) + Supabase database.

## Files
| File | What it is |
|---|---|
| `index.html` | The whole website |
| `config.js` | Your Supabase URL + key (edit this) |
| `supabase-setup.sql` | Database setup (run once in Supabase) |

## Setup
1. **Supabase** → New project → open **SQL Editor**.
2. In `supabase-setup.sql`, change `CHANGE-THIS-PASSWORD` to your host password, paste the whole file, click **Run**.
3. **Project Settings → API**: copy the **Project URL** and the **anon / publishable key** into `config.js`.
4. **GitHub** → new public repo `devotion` → upload `index.html` and `config.js`.
5. Repo **Settings → Pages** → Source: *Deploy from a branch* → `main` / `(root)` → Save.
6. Open `https://lilzamdev.github.io/devotion/` (ready in 1–2 minutes).

## Using it
- **Members:** tap your name → create a 4-digit PIN → write your devotion on your turn day.
- **Host:** tap **Host** at the bottom → password. Tabs: Calendar · Review · Members.
- Forgot PIN → Members tab → **Reset PIN**, they make a new one.
- Change a day's turn: tap the date → **Change turn & theme**.
- Add/remove members: Members tab → Roster → Save (turns re-shuffle from tomorrow).

## Notes
- Keep `supabase-setup.sql` out of the public repo (it's only needed once).
- Supabase free projects pause after ~1 week with no visits — just open the site or the Supabase dashboard to wake it.
- Replace the done / waiting / missed icons in `index.html` (search for `ICONS`).
