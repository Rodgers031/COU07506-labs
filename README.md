# COU07506-labs

Laboratory work for **COU 07506 Digital Signal Processing, 2026/27**.

One Jupyter notebook per lab week, following
`COU07506_DSP_Laboratory_Manual_2026-27.pdf`. Notebooks are named
`COU07506_WeekNN_<RegNo>.ipynb` and uploaded to DIT-eLMS after each session.

## Layout

```
COU07506-labs/
    COU07506_Week01_<RegNo>.ipynb    Week 1 — Lab 0
    data/my_voice.wav                voice recording used in Task 1.3
    README.md
```

## Week 1 — Lab 0: setting up the DSP laboratory

Handout §1.1, Listing 1.3. Required, not marked.

| Task | Content |
|---|---|
| 1.1 | unit impulse, step, ramp and $(0.8)^n u(n)$ as stem plots |
| 1.2 | $(a)^n u(n)$ for $a = 0.5, -0.8, 1.1$; periodicity of two sampled cosines |
| 1.3 | reading, plotting and playing back a recorded WAV |
| 1.4 | the same in GNU Octave (optional — reference only, Octave not installed here) |
| 1.5 | this repository, plus the eLMS submission |

Also contains the pre-lab question and the three analysis questions.

## Running it

**Google Colab** — open the notebook from this repo and use *Runtime → Run all*.
Task 1.3 also accepts a WAV dragged into the Files panel (`/content/my_voice.wav`).

**Locally** — Python 3 with NumPy, SciPy, Matplotlib and Jupyter:

```
python -m jupyter lab
```

The Task 1.3 cell looks for `data/my_voice.wav` and then `my_voice.wav`. If neither is found it
falls back to a synthetic 16 kHz test signal **and prints that it did**, so the notebook still runs
for anyone who clones it without the recording.

## Notes

- `data/my_voice.wav` is 48 kHz, mono, 16-bit PCM, 5.57 s (267 528 samples).
- All figures are regenerated from the committed code; no image is pasted in.
- AI use is declared in the AI-use statement at the end of the notebook, as the module requires.
