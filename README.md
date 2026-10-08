# Pitch Space Lab — Prototype 10

Fixes a regression introduced by the audio warm-up code in Prototype 09. Audio now resumes only when playback is requested and waits briefly before the first scheduled note; no silent oscillator is created on pointer-down.

Harpejji positional-redundancy visualization from Prototype 09 is retained.


Prototype 11 fix: removed a hidden Tonnetz target playback that was being queued during page load. On browsers that suspend Web Audio until the first user gesture, that queued triad could start together with the first note of Exercise 1, producing the reported one-time discordant chord. The Tonnetz target is now initialized silently and plays only when explicitly requested.
