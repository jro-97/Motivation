# Motivation

A daily motivational quote app for my daughters. Each day I add a new quote, commit it, and text them the link. They see a beautiful, shareable quote card they can save to their phone.

**Live site:** `https://<your-username>.github.io/Motivation/`

---

## How to Add a New Quote

1. Go to your **Motivation** repository on GitHub (works from your phone or laptop)
2. Tap on the file **`quotes.json`**
3. Tap the **pencil icon** (✏️) to edit the file
4. Add a new entry **at the very top** of the list, right after the opening `[` bracket. Follow this format:

```json
[
  {
    "date": "2026-03-07",
    "quote": "Your new quote goes here.",
    "author": "Author Name",
    "note": "A personal note for the girls. — Dad"
  },
  ... (previous entries stay below)
]
```

5. Make sure:
   - The **date** matches today's date in `YYYY-MM-DD` format
   - There's a **comma** after the closing `}` of your new entry (before the next entry)
   - The **quote** and **author** fields are filled in
   - The **note** field is optional but adds a personal touch
6. Scroll down and tap **"Commit changes"**
7. Wait about 60 seconds for GitHub Pages to rebuild
8. Open your site link, confirm the new quote shows up, and text the link to the group chat!

---

## quotes.json Format

```json
[
  {
    "date": "2026-03-06",
    "quote": "She believed she could, so she did.",
    "author": "R.S. Grey",
    "note": "Never stop believing in yourselves. — Dad"
  }
]
```

| Field    | Required? | Description                                    |
|----------|-----------|------------------------------------------------|
| `date`   | Yes       | The date in `YYYY-MM-DD` format                |
| `quote`  | Yes       | The motivational quote text                    |
| `author` | Yes       | Who said or wrote the quote                    |
| `note`   | No        | A personal note from you (shown on the card)   |

---

## Setting Up GitHub Pages

If you haven't enabled GitHub Pages yet:

1. Go to your repository on GitHub
2. Click **Settings** (the gear icon tab)
3. In the left sidebar, click **Pages**
4. Under **Source**, select **Deploy from a branch**
5. Choose the **main** branch and **/ (root)** folder
6. Click **Save**
7. Your site will be live at `https://<your-username>.github.io/Motivation/` within a minute or two

---

## Features

- **Today's quote** displayed as a beautiful, shareable card
- **Save to Phone** button to download the card as a PNG image
- **Previous Messages** archive to browse and save past quotes
- **Mobile-first** design that looks great on any phone
- **No backend** — pure static site, works entirely on GitHub Pages
