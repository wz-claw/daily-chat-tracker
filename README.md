# Daily Chat Tracker

A private tracker for daily chat duration statistics.

## How to Use

1. Update `data.json` with your daily chat duration data
2. Push changes to trigger automatic deployment
3. View statistics at the GitHub Pages URL

## Data Format

Add entries to `data.json` in this format:

```json
{
  "date": "YYYY-MM-DD",
  "hours": 2.5,
  "notes": "Optional notes"
}
```

## Updating Data

Simply add new entries to the `data.json` array and push to the `gh-pages` branch. The GitHub Action will automatically update the statistics page.

## Viewing Stats

The statistics page shows:
- Total days tracked
- Total hours
- Average hours per day
- Maximum hours in a day
- Trend chart
- Detailed data table
