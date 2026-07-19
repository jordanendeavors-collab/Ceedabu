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
  ch5.mp3  2:14  The Alignment

NAVIGATION
  Sticky bar at the top: brand returns to the top, Menu drops a panel
  with all four destinations. On screens wider than 1000px a rail on
  the right marks which section you are in.

LIGHT LEVELS
  Dark / Med / Light in the top bar. The choice is remembered, and the
  session canvas repaints to match, so the breathing screen is not a
  black rectangle when the rest of the site is parchment.

DURING A SESSION
  With "The boards" selected, your nine plates drift behind the
  breathing orb - slow push in, pull out, and lateral drifts, one
  every 22 seconds with a 3 second cross. Order is shuffled each
  session so it is not the same walk twice. They sit at roughly 20%
  and are washed back toward the ground colour, so the orb always
  wins and the text on the plates never becomes something to read.
  Choose "Plain" for an empty field.

LANGUAGES
  Picker in the top bar: English, Italiano, Espanol, Francais,
  Ellinika, Ivrit, Samskrtam, Arabiyya. Choice is remembered.
  Hebrew and Arabic flip the whole layout right-to-left.

  Labels, buttons and breath cues are translated. YOUR CHAPTERS ARE
  STILL ENGLISH -- a line appears above Begin saying so in the chosen
  language, so nobody is misled.

  TO ADD A LANGUAGE'S NARRATION
    Record the four chapters in that language and drop the files in
    beside index.html:
        ch1-it.mp3  ch2-it.mp3  ch3-it.mp3  ch4-it.mp3
    Codes: it es fr el he sa ar
    The player asks for the localised file first and falls back to the
    English one if it is not there, so you can add them one at a time.
    No code change needed. Remove the engOnly line for that language
    once all four are recorded.

  ON SANSKRIT
    No browser ships a Sanskrit speech voice. The cue words are written
    in Devanagari and read by a Hindi voice where one exists. Close,
    not exact. Recording ch1-sa.mp3 etc. is the real fix.

NOTES
  - Must be served over https, not opened as a local file.
  - Filenames are case sensitive on Vercel. Keep them lowercase.
  - To re-record a chapter, replace the mp3 under the same name.
