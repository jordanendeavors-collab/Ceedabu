THE HUMMING OF GOD - 4.7.8
Flat build for 4in7hld8hum.com

WHY THIS VERSION
  GitHub's mobile uploader cannot create folders, so the earlier
  package landed flat and every path broke. This build has NO folders.
  Every file sits at the repo root, right next to index.html.

UPLOAD
  Put all 23 files in the root of the repo. Nothing goes in a folder.
  Delete the old b1-b9.jpg first - the previous upload may have left
  thumbnails under those names.

FILES
  index.html        the whole site
  ch1-ch4.mp3       narration, chapters 1-4
  b1-b9.jpg         boards, full size (opened when tapped)
  t1-t9.jpg         boards, thumbnails (shown in the grid)

  Thumbnails are named t#, not b#, so they can never collide with the
  full-size boards during a flat upload. Keep both sets.

CHAPTERS
  ch1.mp3  2:12  The Invocation
  ch2.mp3  2:19  The Convergence
  ch3.mp3  1:57  Finding Your Pitch
  ch4.mp3  1:29  The Cadence

NOTES
  - Must be served over https, not opened as a local file.
  - Filenames are case sensitive on Vercel. Keep them lowercase.
  - To re-record a chapter, replace the mp3 under the same name.
