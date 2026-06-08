# Daily Chat Tracker

A tracker for daily chat duration statistics with online/offline distinction.

## How to Use

1. Update `data.json` with your daily chat duration data
2. Push changes to trigger automatic deployment
3. View statistics at the GitHub Pages URL

## Data Format

Add entries to `data.json` in this format:

```json
{
  "date": "YYYY-MM-DD",
  "online": 4,
  "offline": 1
}
```

- `online` - hours of online chat
- `offline` - hours of offline (in-person) chat

## Updating Data

Simply add new entries to the `data.json` array and push to the `gh-pages` branch. The GitHub Action will automatically update the statistics page.

## Viewing Stats

The statistics page shows:
- Total days tracked
- Total hours
- Online hours (blue)
- Offline hours (orange)
- Average hours per day
- Stacked bar chart showing online/offline breakdown
- Detailed data table
