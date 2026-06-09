# IPA Board Meeting Website

A simple, free, linked multi-page website for Board meeting materials.

## Files included

| File | Purpose |
|------|---------|
| `index.html` | Homepage with navigation cards |
| `agenda.html` | Meeting agenda & schedule |
| `reports.html` | Reports & document downloads |
| `presentations.html` | Slide deck downloads |
| `bios.html` | Board member profiles |
| `style.css` | Shared styles (colors, fonts, layout) |

---

## How to publish for free on GitHub Pages

1. Go to https://github.com and sign in (or create a free account).
2. Click **New repository**. Name it something like `ipa-board-meeting`. Set it to **Public**.
3. Click **uploading an existing file**, then drag all 6 files into the upload area.
4. Click **Commit changes**.
5. Go to **Settings → Pages** in your repository.
6. Under "Source", select **Deploy from a branch**, choose `main`, and click **Save**.
7. After ~1 minute, your site will be live at: `https://YOUR-USERNAME.github.io/ipa-board-meeting/`

Share that URL with Board members. That's it!

---

## How to update the site

### Change the meeting date / time / location
Open `index.html` in any text editor (Notepad, TextEdit, VS Code).
Find the text `Month DD, YYYY` and `HH:MM – HH:MM ET` and replace them.

### Update the agenda
Open `agenda.html`. Each row in the table looks like:
```html
<tr>
  <td class="time">9:00 AM</td>
  <td class="duration">10 min</td>
  <td>
    <div class="topic">Your Topic Title</div>
    <div class="presenter">Description here</div>
  </td>
  <td>Presenter Name</td>
</tr>
```
Copy, paste, and edit rows as needed.

### Link a document or presentation
Open `reports.html` or `presentations.html`.
Find `href="#"` in the relevant item and replace `#` with your file's URL:
```html
<a href="https://drive.google.com/your-file-link" class="doc-link">
```

### Add a Board member
Open `bios.html`. Copy the block between the `COPY AND PASTE THIS BLOCK` comments, paste it inside the `<div class="bio-grid">`, and update the initials, name, role, and bio.

### Change the brand colors
Open `style.css`. The colors are at the top under `/* TOKENS */`.
The main IPA green is `#49ac57`. Do not change these unless directed.

---

## Need help?

Contact support@poverty-action.org
