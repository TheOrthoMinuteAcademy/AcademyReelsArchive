# Podcast Reel Archive (Jekyll + GitHub Pages + YouTube)

## One-time setup
1. Create a new **empty** GitHub repo (e.g. `podcast-archive` or `yourname.github.io`).
2. Upload every file/folder in this package into the repo root, preserving the folder structure.
3. Edit `_config.yml`:
   - Set `title`, `description`
   - Set `url` to `https://YOUR_USERNAME.github.io`
4. In the repo, go to **Settings → Pages** → set Source to the `main` branch (root). Save.
5. Wait 1-2 minutes, then your site is live at the URL GitHub shows you.

## Adding a new reel (recurring workflow — no new repo needed)
1. Upload your reel to YouTube (Public or Unlisted) and copy the video ID
   (the part after `v=` in the URL).
2. Duplicate `_episodes/2026-08-09-example-episode.md`, rename the file to
   `YYYY-MM-DD-short-slug.md` (the date becomes the sort order).
3. Fill in the front matter: `title`, `guest`, `date`, `youtube_id`, `tags`.
4. Write show notes in the body if you want.
5. Commit/push. GitHub Pages rebuilds automatically — new card appears on the
   homepage grid, sorted newest-first, and gets its own shareable page at
   `/episodes/your-slug/`.

## Notes
- Delete the example episode file once you've added your first real reel.
- The homepage grid auto-filters by whatever tags you use in front matter —
  no code changes needed to add a new filter button.
- Videos are streamed from YouTube, so there's no file-size limit concern on
  GitHub's side (repo just stores lightweight HTML/CSS/metadata).
- To share the archive with a prospective guest, just send them the site URL —
  it works as a public portfolio of past episodes.
