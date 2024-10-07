# Lipsynced avatars

To create a more animated version of the podcast I tried using AI avatars.

They are currently limited and expensive (october 2024).

I tried various options. Some of them offer an excessively limited trial that
made impractical to use them for a prove of concept, when using a 8 minutes
video.

Not every service allows using an already generated audio file. All of them
can create voice from a script. But NotebookLM podcast sounds really cool to
discard the expressive voices.

Some services uses generative AI to modify avatars you upload. This approach
can generate undesirable artifacts (see the section about Other lessons). Others
needs a very clean face to work. In the case of [HeyGen](https://www.heygen.com/)
they have nice avatars created filimng people doing some natural gestures.
So then the AI just needs to do a lipsync for the real face. This produces
acceptable quality with little effort.

Note that I don't know which approach is better, but it looks like the
resources needed for the generation are too expensive and you get very
limited usage. Even paying you get a very limited usage, that prevents
experimenting. The HeyGen folder contains lipsynced avatars using the
separated fe/male audio files. As the limit is 3 minutes I had to cut the
audio and it introduced a few errors.

Once I got the clips I composed a video. Some important detail is that HeyGen
avatars continue moving even when no audio is there. So my first approach,
using the fe/male characters side by side wasn't really good.

I tried making dimming the avatar that wasn't talking, it was better, but not
good enough. So the third approach was the simplest: alternate between them.
Yes, silly me.

I used [kdenlive](https://kdenlive.org/) for the videos. Adding some simple
titles at the end. I found that modern versions of kdenlive have built-in
support for that, but it was simpler to create them in the old way.

At the end I added the cute robot waving its hand, generated using
[Runway](https://runwayml.com/) (Gen-3 Turbo).

For the subtitles in English I used the ones extracted by Runway from the audio
files and edited them using kdenlive.

[![Alternate avatars](https://img.youtube.com/vi/6eYtJ9xiS1U/0.jpg)](https://www.youtube.com/watch?v=6eYtJ9xiS1U)


## Other lessons

While trying with [Hedra](https://www.hedra.com/) I found a couple of problems worth to mention.

The Hedra/big_smile_error.mp4 shows what happens when you use a "not so natural" face.
The avatar is always smiling, which becomes exaggerated.

You can also see how complex backgrounds generates undesired artifacts: Hedra/artifacts.mp4
Not to mention problems with the eyes.

Note: lamentably Hedra free trial isn't useful, so I couldn't experiment enough to get
something usable. The 30 seconds limit makes it less than a toy.
