# NewsNotes

A macOS desktop widget that shows the day's top stories from NPR and Hacker News as sticky notes.

## Project goal
Each day, the first time I log in, I see the day's news on my desktop. Each article is a sticky note with a title, a short description and a link for each story, without opening a browser.

## MVP scope
- Fetch stories from the NPR and Hacker News RSS feeds
- Clean up each story's title, short description and link
- Cache stories once per day in `stories.json`
- Show the stories as sticky notes on the desktop with an Ubersicht widget
- Open the full article when a note is clicked
- Fall back to cached stories when offline

## Future plans
- Higher quality descriptions by sending the article to an LLM 
- Removing dupes so stories aren’t repeated, using a cache
- Dismiss, pin, remind me later options on notes


## Tech stack
- **Languages:** Python 3, JSX
- **Libraries / tools:** `feedparser`, Übersicht (macOS)
- **Data storage:** `stories.json` (date + cached stories)
`

