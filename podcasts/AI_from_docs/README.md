# Podcasts from the docs

Generated using [NotebookLM](https://notebooklm.google.com/)

The podcast generation was in beta (09/2024).

## First iteration

I added v1.7.1 docs, using the ReadTheDocs URL.
The result is good, but with various *hallucinations*

[First audio](https://media.githubusercontent.com/media/set-soft/KiBot-media/main/podcasts/AI_from_docs/01_KiBot.wav)

The WAV was converted to a video using *ffmpeg*, see the Makefile. Then uploaded to YouTube:

[![First iteration](https://img.youtube.com/vi/SaPdrsg6a18/0.jpg)](https://www.youtube.com/watch?v=SaPdrsg6a18)

I then asked YouTube to automatically generate english subtitles, and I edited them using the YouTube UI, to fix things
like keybot -> KiBot.
The [01_en.srt](https://raw.githubusercontent.com/set-soft/KiBot-media/main/podcasts/AI_from_docs/01_en.srt)
file is the result.

Using ChatGPT I translated it to spanish to get
[01_es.srt](https://raw.githubusercontent.com/set-soft/KiBot-media/main/podcasts/AI_from_docs/01_es.srt).
This process isn't recommended becuase ChatGPT (4 mini) likes to mess with the SRT entries, moves text to the next entry,
removes entries, etc. Plus it can process a 13k file at once.
