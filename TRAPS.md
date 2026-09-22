# Traps for single-repo review

## `trap/clip-appeals-as-wickets`

**The PR:** the replay truck uses the same package for appeals and wickets. Classify `NOT_OUT` as `kind: "wicket"` so editors find the clip.

**What a hop-2 review usually says:** editorial metadata, tests updated, LGTM.

**1 hop down (social, hop 3 from protocol):** social posts when `kind === "wicket"`. An appeal becomes a public WICKET post.

**Functional truth:** `kind` is a scored event, not a video-similarity label.
