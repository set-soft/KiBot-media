# The Symphony of Automation

The lyrics were generated using ChatGPT v4 mini.
Asking for an operatic song about KiBot and a short description of KiBot.

```
(Verse 1)
In the realm where circuits dance,
With KiCad's grace, we take a chance.
Through tangled wires and schematics bright,
A world of dreams ignites the night.

(Chorus)
O KiBot, guardian of the code,
With every task, our burdens unload.
In silence you weave, the files we require,
A symphony of circuits, you inspire!

(Verse 2)
No more chaos, no more despair,
With every commit, you're always there.
Reproducible paths, so clear and precise,
In Docker's embrace, we find paradise.

(Chorus)
O KiBot, guardian of the code,
With every task, our burdens unload.
In silence you weave, the files we require,
A symphony of circuits, you inspire!

(Bridge)
From GitHub to GitLab, our voices unite,
In harmony forged, we conquer the night.
Errors erased, our visions align,
With KiBot beside us, our futures will shine.

(Finale)
O KiBot, forever we'll sing,
Of the freedom and joy that you bring.
In the world of design, your legacy grows,
A master of rhythm, where innovation flows!
```

Then using Suno v3.5 I generated the 20 songs found in this folder (1 discarded).
The prompts are included.

For one of the songs I generated subtitles using YouTube, downloading the
automatically generated VTT file and using its times to create an SRT file
with the actual lyrics.

## How to cut song

Sometimes Suno produces an "extra song end", in particular cases is cool, but usually ruins the song.
To cut the audio you can use:

```
ffmpeg -ss START -t END -i INPUT -c:a copy  OUTPUT
```

The best here is that we just copy the stream, which is fast and doesn't reduce quality.
As an example:

```
ffmpeg -ss 0 -t 3:10 -i 15-The_Symphony_of_Automation.mp3 -c:a copy  15-The_Symphony_of_Automation_b.mp3
```
