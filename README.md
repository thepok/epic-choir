# epic-choir

A free SATB **vowel choir** sample library (SFZ + WAV) made from **real singers**: the 20 voices of the
[VocalSet](https://doi.org/10.5281/zenodo.1442513) dataset, 3–10 different singers summed into every sample, so it
sounds like a section, not one voice copied. Licence: **CC BY 4.0** — free for any use, also commercial, with credit.

Listen: [`demos/hymn.mp3`](demos/hymn.mp3) (a chorale, p → f → p) · [`demos/phrases.mp3`](demos/phrases.mp3)

## Contents

| | |
|---|---|
| Parts | Soprano, Alto, Tenor, Bass |
| Vowels | ah, oh, oo, ee, eh — one SFZ per part and vowel (`S_ah.sfz` … `B_oo.sfz`, 20 programs) |
| Dynamics | p / mf / f, crossfaded on **CC1** (mod wheel; default 80) |
| Ranges | S C4–G#5 · A A3–F5 · T B2–G#4 · B A2–F4 (no low bass below A2) |
| Samples | 600, one per whole tone (repitched by at most 1 semitone), 44.1 kHz 16-bit stereo, ~740 MB |
| Singers per sample | 3–10 (median 9–10), each from its own recording, each on its own seat in a simulated hall |

**Download the samples** from the [Releases](../../releases) page — one zip per part (`epic-choir-v1.0-S.zip`,
`-A`, `-T`, `-B`, ~165 MB each, each with its SFZ files) — unpack them all into one folder (they share the
`samples/` tree), and load any `.sfz` in an SFZ player (e.g. sfizz, Sforzando,
TX16Wx, Decent Sampler via conversion).

Tips: the takes are close-miked recordings in a simulated room — a gentle treble cut (≈ −2 dB above 6 kHz) and a
hall reverb make it sit further back. Ride CC1 for swells. No consonants or words: wordless vowels only.

## How it was made

From `VocalSet11.zip` (md5 `0c09396242f946e7111ad7d8fc649b81`): segments of the long tones, scales and arpeggios
(straight, pp, forte, slow piano / forte; vowels a e i o u) were cut, pitch-shifted by at most 2 semitones (median
0.7 incl. each singer's own intonation), their sustains extended from their own audio (no fixed loops), level-matched,
placed in a simulated hall (one seat per singer) and summed per note. Each singer keeps their own breath onset and
release. Built with [AgentSound](https://github.com/thepok/AgentSound), an agent-first offline DAW. Details:
`SOURCE.json`, `ATTRIBUTION.txt`.

## Licence and credit

The samples are a derived work of VocalSet, licensed under
[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/); this pack is released under the same licence. Please
credit, in music or products made with it:

> Choir samples derived from VocalSet (Wilkins, Seetharaman, Wahl, Pardo 2018), CC BY 4.0,
> https://doi.org/10.5281/zenodo.1442513 — epic-choir by thepok

Original dataset: Wilkins, J., Prem Seetharaman, Alison Wahl, & Bryan Pardo. (2018). *VocalSet: A Singing Voice
Dataset* (Version 1.2) [Dataset]. Zenodo. https://doi.org/10.5281/zenodo.1442513 — paper: ISMIR 2018, Paris.

The samples were modified as described above. No endorsement by the VocalSet authors is implied.
