# Athlete Training

Training, nutrition, and progress tracking for two athletes: **Denis** and **Alicja**.

## Structure

```
athlete-training/
├── README.md                       ← this file
├── shared/                         ← general guidelines & reference (apply to both people)
│   ├── assistant_instructions.md   ← how the AI assistant should work for either athlete
│   ├── training_principles.md      ← general methodology: readiness, deload, session types, recovery
│   ├── calisthenics_ladders.md     ← skill-progression ladder definitions (reference)
│   └── keto_nutrition_reference.md ← per-100 g food table, TKD fueling, electrolytes, supplements
│
├── people/
│   ├── denis/                      ← Denis's personal data
│   │   ├── profile.md
│   │   ├── training_plan.md        ← his weekly structure & priorities
│   │   ├── gym_training_plan.md
│   │   ├── calisthenics_status.md  ← current skill levels + focus (reads ladders from shared/)
│   │   ├── nutrition.md
│   │   └── workout_log.md          ← auto-synced from Strava
│   │
│   └── alicja/                     ← Alicja's personal data
│       ├── profile.md
│       ├── training_plan.md        ← flexible weekly template
│       ├── gym_training_plan.md    ← novice hypertrophy progressions
│       ├── mobility_splits.md      ← flexibility / splits routine
│       ├── running_plan.md         ← beginner VO2max / threshold build
│       ├── nutrition.md
│       └── workout_log.md          ← manual (no wearable)
│
├── tools/                          ← web dashboards / editors
│   ├── denis_dashboard.html        ← full dashboard (Strava + Garmin readiness + skills)
│   ├── denis_nutrition_editor.html
│   └── alicja_dashboard.html       ← simplified (manual log, no wearable)
│
└── .github/                        ← Strava → Denis workout-log auto-sync (Denis only)
```

## How to use this with the assistant

When asking the assistant for help, say **whose** plan you mean ("Denis's threshold session", "Alicja's gym day"). The assistant reads:

1. `shared/` for the general rules and reference, then
2. that person's folder under `people/<name>/` for their profile, plan, and logs.

Both athletes follow ketogenic nutrition. Person-specific priorities, capacities, and current levels always live in the person's own folder.
