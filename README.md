# justfixed-data

Data files consumed by the [JustFixed](https://github.com/razukadm/justfixed)
app at runtime.

Two kinds of content:

- `curves/` — Brazilian yield curves (DI futures from B3, ETTJ from ANBIMA).
  Refreshed periodically by the admin. Format: see `docs/CURVE_FORMAT.md`
  (TBD).
- `seed/` — Initial issuer/conglomerate reference data for new installs.
  Loaded once on first app launch (when the user's database is empty).

This repository is public and unauthenticated. The JustFixed app fetches
files via raw GitHub URLs. Updates here propagate to all users on next
app launch.

For format details and admin tooling, see the JustFixed source repo's
`docs/` directory.
