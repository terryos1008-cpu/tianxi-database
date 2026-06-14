# Data Integrity Audit · 2026-06-14

**Overall:** 🔴 `critical`  ·  critical gaps: **50**  ·  warn gaps: 20

**Recommendation:** `gha_next_delta_will_fix`

## Per-category

| Category | Severity | Expected | Present | Missing | Stale | Notes |
|---|---|---|---|---|---|---|
| race_artefacts | 🔴 critical | 675 | 625 | 50 | 0 | days with any missing artefact: 10 |
| fixtures_cache | 🟢 ok | 1 | 143 | 0 | 0 | total cached race days: 143 |
| horse_profiles | 🟡 warn | 1212 | 1212 | 0 | 14 | 14 profiles are stale (profile_last_scraped < last_race_date); total profiles in DB: 5952 |
| horse_form_records | 🟢 ok | 1212 | 1212 | 0 | 0 | total form_records files: 5952 |
| jockey_profiles | 🟢 ok | 35 | 35 | 0 | 0 | total jockey profiles: 64 |
| jockey_records | 🟡 warn | 64 | 59 | 5 | 0 | 5 jockey profiles have no records file |
| trainer_profiles | 🟢 ok | 32 | 32 | 0 | 0 | total trainer profiles: 67 |
| trainer_records | 🟢 ok | 67 | 67 | 0 | 0 |  |
| trial_results | 🟢 ok | 1 | 1 | 0 | 0 | trial rows: 5904 |
| entries_upcoming | 🟡 warn | 1 | 0 | 1 | 0 | 1 upcoming race days lack entries file |

### 🔴 race_artefacts — sample missing (first 20)

```
results_2026-05-13
commentary_2026-05-13
dividends_2026-05-13
sectional_times_2026-05-13
video_links_2026-05-13
results_2026-05-17
commentary_2026-05-17
dividends_2026-05-17
sectional_times_2026-05-17
video_links_2026-05-17
results_2026-05-20
commentary_2026-05-20
dividends_2026-05-20
sectional_times_2026-05-20
video_links_2026-05-20
results_2026-05-24
commentary_2026-05-24
dividends_2026-05-24
sectional_times_2026-05-24
video_links_2026-05-24
```
