# Life XP

Minimal React + Vercel Functions app for healthy lifestyle gamification.

## Stack

- React loaded directly in the browser through ESM modules
- Vercel serverless API for daily feedback generation
- Local browser storage for saved daily entries

## Deploy

1. Push the repository.
2. In Vercel, set Framework Preset to `Other`.
3. Keep the Root Directory at the repository root.
4. Leave the Build Command empty.
5. Deploy.

Frontend: `http://localhost:5173`

## Notes

- Workout XP assumption: `rehab` and `light` both award `20 XP`, since the brief listed four workout types but only three XP values.
- Running supports either minutes or kilometers. Kilometer thresholds are mapped as `2 / 4 / 6+ km` for `20 / 40 / 60 XP`.
- Streak and total XP are computed from saved daily history in local storage.
- This project is intentionally deployable without a frontend build step, which is useful for static Vercel deployments.
