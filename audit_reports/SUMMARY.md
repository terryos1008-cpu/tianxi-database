# Data Integrity Audit · 2026-05-20

**Overall:** 🔴 `critical`  ·  critical gaps: **15**  ·  warn gaps: 22

**Recommendation:** `gha_next_delta_will_fix`

## Per-category

| Category | Severity | Expected | Present | Missing | Stale | Notes |
|---|---|---|---|---|---|---|
| race_artefacts | 🔴 critical | 640 | 625 | 15 | 0 | days with any missing artefact: 3 |
| fixtures_cache | 🟢 ok | 1 | 143 | 0 | 0 | total cached race days: 143 |
| horse_profiles | 🟡 warn | 1264 | 1264 | 0 | 14 | 14 profiles are stale (profile_last_scraped < last_race_date); total profiles in DB: 5952 |
| horse_form_records | 🟢 ok | 1264 | 1264 | 0 | 0 | total form_records files: 5952 |
| jockey_profiles | 🟢 ok | 47 | 47 | 0 | 0 | total jockey profiles: 64 |
| jockey_records | 🟡 warn | 64 | 59 | 5 | 0 | 5 jockey profiles have no records file |
| trainer_profiles | 🟢 ok | 44 | 44 | 0 | 0 | total trainer profiles: 67 |
| trainer_records | 🟢 ok | 67 | 67 | 0 | 0 |  |
| trial_results | 🟢 ok | 1 | 1 | 0 | 0 | trial rows: 5904 |
| entries_upcoming | 🟡 warn | 3 | 0 | 3 | 0 | 3 upcoming race days lack entries file |

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
```
