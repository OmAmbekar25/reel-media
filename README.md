# reel-media

Transient public hosting for rendered short-form video.

Instagram's Content Publishing API **fetches** video from a public HTTPS URL —
it cannot accept an upload — so each rendered MP4 is pushed to the `media`
branch just long enough for Meta to ingest it, then cleared.

The `media` branch is an orphan branch holding exactly one commit, rewritten on
every upload. No video ever enters history, so this repository stays empty
however many reels pass through it.
