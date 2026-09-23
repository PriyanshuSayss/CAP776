# CAP776 — Daily Routine Log

## What this repository contains

This repository contains a day-by-day breakdown of my daily routine data,
originally recorded in `12603655.xlsx`. The data has been split out of the
spreadsheet into one JSON file per date, stored under `daily-routine/`, so
that each day's routine can be viewed, tracked, and version-controlled
independently.

The original spreadsheet (`12603655.xlsx`) is kept unchanged in the
repository root as the source of record. Its values and formulas have not
been modified in any way.

## Date range covered

**17 August 2026 – 21 September 2026** (36 days).

## Repository structure

```
daily-routine/
├── 2026-08-17.json
├── 2026-08-18.json
├── ...
└── 2026-09-21.json
```

Each file contains only that single date's data — no other day's data is
present in the file.

## Field meanings

| Field                    | Meaning                                                              |
|---------------------------|-----------------------------------------------------------------------|
| `date`                    | The calendar date of the entry (YYYY-MM-DD).                        |
| `sleep_min`                | Minutes spent sleeping.                                              |
| `fitness_min`              | Minutes spent on fitness/exercise.                                   |
| `study_min`                | Minutes spent studying.                                               |
| `coding_min`               | Minutes spent coding.                                                 |
| `class_min`                | Minutes spent in class.                                               |
| `classes_attended`         | Number of classes attended that day.                                 |
| `other_activities_min`     | Minutes spent on other activities not covered above.                 |
| `total_tracked_min`        | Sum of all tracked minutes for the day.                              |
| `free_unaccounted_min`     | Minutes in the day not accounted for by any tracked category.        |
| `days_feeling`             | A short descriptor of how the day felt overall (e.g. "Good", "Tired"). |
| `satisfaction_level`       | Self-reported satisfaction level for the day.                        |
| `energy_level`             | Self-reported energy level for the day.                              |
| `notes`                    | Free-text notes about the day.                                       |
| `special_event` (optional) | Present only on days with a notable event (see below).               |

## Special events preserved from the source data

- **31 Aug 2026** — English CA 1
- **1 Sep 2026** — Networking CA
- **9 Sep 2026** — Database Management System CA
- **15 Sep 2026** — Python CA

Note: 10 Sep 2026 is not tagged with a `special_event` field. The source
spreadsheet's notes for that date describe it only as a day after the CA
("CA was over, so the day felt a little more relaxed") and do not mention
a farewell event, so nothing was added that isn't present in the original
data.

## Important notes on dates and timestamps

- **The dates inside the data are the actual dates of the activities**
  (17 Aug 2026 – 21 Sep 2026), exactly as recorded in `12603655.xlsx`.
- **All historical entries are retrospective/reconstructed estimates**
  based on my usual routine, as stated in the original spreadsheet;
  durations are approximate, not measured in real time.
- **Git commit timestamps represent when this repository was updated**,
  not when the activities themselves occurred. Commit history was created
  after the fact while organizing this data, and timestamps have not been
  backdated or altered to match the activity dates.
