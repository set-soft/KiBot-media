# Funny end titles

For a demo presentation of KiBot I created some sort of funny end titles.
The titles shows the various KiBots used for ilustration and the engineer.

I used OpenShot tool (cute but very raw). The End_Titles.osp file is the project.

The texts were created using InkScape using the Liberation TTF font.

The music, and its subtitles, are from the ../../music/01-The_Symphony_of_Automation/ folder.

To generate the video I asked OpenShot to create the images as PNGs (instead of Audio+Video).
I did it because the timing of the video is too short and the UI doesn't help much to adjust it.

With the PNGs I used *do_it.sh*:

```
ffmpeg -framerate 30 -pattern_type glob -i 'res/End_Titles-*.png' -i ../../music/01-The_Symphony_of_Automation/01-The_Symphony_of_Automation.mp3 -c:a libfdk_aac -af apad -shortest -c:v libx265 -pix_fmt yuv420p funny_end_titles.mp4
```

A preview of the video was uploaded to [YouTube](https://youtu.be/sEjZK7ROmu8)
