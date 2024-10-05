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


## Second iteration

To reduce the ammount of *hallucinations* I feeded NotebookLM with a document with some extra facts:
[02_Facts.txt](https://raw.githubusercontent.com/set-soft/KiBot-media/main/podcasts/AI_from_docs/02_Facts.txt).

This reduced the ammount of *hallucinations* drastically. As a side effect the focus was put on CI/CD:

[Second audio](https://media.githubusercontent.com/media/set-soft/KiBot-media/main/podcasts/AI_from_docs/02_KiBot_correction_1.wav)

Still I found one major error. So I used *audacity* to remove it (you can see the file history).

Again converted it to an MP4 and uploaded to YouTube:

[![CI/CD podcast](https://img.youtube.com/vi/BgSvupdpGvo/0.jpg)](https://www.youtube.com/watch?v=BgSvupdpGvo)

Using a similar process I got the english subitles:
[02_en.srt](https://raw.githubusercontent.com/set-soft/KiBot-media/main/podcasts/AI_from_docs/02_en.srt)

For the spanish translation I used a Google Translator [wrapper](https://www.syedgakbar.com/projects/dst).
I finally editer the SRT to separate both voices:
[02_es.srt](https://raw.githubusercontent.com/set-soft/KiBot-media/main/podcasts/AI_from_docs/02_es.srt)


## Third iteration

I included more facts to finally kill the remaining *hallucination*:
[03_Facts.txt](https://raw.githubusercontent.com/set-soft/KiBot-media/main/podcasts/AI_from_docs/03_Facts.txt).

This again changed the focus. A side effect of using simple facts, instead of incorporating them to the original source.

[Third audio](https://media.githubusercontent.com/media/set-soft/KiBot-media/main/podcasts/AI_from_docs/03_KiBot_correction_2.wav)

Following a similar process:

[![General podcast](https://img.youtube.com/vi/rfq6ljDD6FI/0.jpg)](https://www.youtube.com/watch?v=rfq6ljDD6FI)

[03_en.srt](https://raw.githubusercontent.com/set-soft/KiBot-media/main/podcasts/AI_from_docs/03_en.srt)

[03_es.srt](https://raw.githubusercontent.com/set-soft/KiBot-media/main/podcasts/AI_from_docs/03_es.srt)

[03_en_runway.srt](https://raw.githubusercontent.com/set-soft/KiBot-media/main/podcasts/AI_from_docs/03_en_runway.srt)
is the voice to text result obtained using Runway, I just fixed KiBot and KiCad.

