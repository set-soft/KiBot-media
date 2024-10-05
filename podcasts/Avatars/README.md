# Avatars

Generated to experiment using AI avatars.

I failed to get something usable, but here are some stuff I used.

## 01 Fe/Male

Using Night Cafe I created a cute couple:

Text prompt:
```
Young man, very handsome. 40 yo. dark brown hair. Hyper realistic.
Highly detailed. In a podcast booth, wearing headphones intricate details,
HDR, beautifully shot, hyperrealistic, sharp focus, 64 megapixels,
perfect composition, high contrast, cinematic, atmospheric,
moody Cinematic film still, shot on v-raptor XL, film grain, vignette,
color graded, post-processed, cinematic lighting, 35mm film, live-action,
best quality, atmospheric, a masterpiece, epic, stunning,
dramatic Cinematic film still, shot on v-raptor XL, film grain, vignette,
color graded, post-processed, cinematic lighting, 35mm film, live-action,
best quality, atmospheric, a masterpiece, epic, stunning,
dramatic Cinematic film still, shot on v-raptor XL, film grain, vignette,
color graded, post-processed, cinematic lighting, 35mm film, live-action,
best quality, atmospheric, a masterpiece, epic, stunning, dramatic
```

Note: yes, I accidentally repeated the style

Revised prompt:
```
Handsome 40-year-old man with dark brown hair, sitting in a dimly lit
podcast booth, wearing high-fidelity headphones adorned with intricate
metal details, subtle leather textures, and a sleek, modern design.
The image is a hyper-realistic, cinematic film still, shot on a V-Raptor XL
camera, with 35mm film aesthetics, cinematic lighting, and post-processing
techniques. The atmosphere is moody and atmospheric, with a shallow depth
of field, sharp focus, and subtle film grain. The image boasts a 64-megapixel
resolution, high contrast, and beautifully nuanced color grading.
The overall aesthetic is reminiscent of the works of Gregory Crewdson, with
the attention to detail of a Photographer like Andreas Gursky, and the
cinematic lighting of a filmmaker like Roger Deakins.
```

Model: Flux Schnell 1.0

Initial Resolution: Medium

Aspect Ratio: 1:1

Runtime: Short

Seed: 3210573148

Overall Prompt Weight: 50%

![01 Male](https://raw.githubusercontent.com/set-soft/KiBot-media/main/podcasts/Avatars/01-male.jpg)

Text prompt:
```
Young female, very handsome. 30 yo. light brown hair. Hyper realistic. Highly detailed.
In a podcast booth, wearing headphones intricate details, HDR, beautifully shot,
hyperrealistic, sharp focus, 64 megapixels, perfect composition, high contrast, cinematic,
atmospheric, moody Cinematic film still, shot on v-raptor XL, film grain, vignette, color graded,
post-processed, cinematic lighting, 35mm film, live-action, best quality, atmospheric, a masterpiece,
epic, stunning, dramatic Cinematic film still, shot on v-raptor XL, film grain, vignette, color graded,
post-processed, cinematic lighting, 35mm film, live-action, best quality, atmospheric, a masterpiece,
epic, stunning, dramatic Cinematic film still, shot on v-raptor XL, film grain, vignette, color graded,
post-processed, cinematic lighting, 35mm film, live-action, best quality, atmospheric, a masterpiece,
epic, stunning, dramatic
```

Note: yes, I accidentally repeated the style

Revised prompt:
```
young female, 30, with chiseled features and light brown hair, sits poised in a professional podcast booth,
wearing a pair of sleek, intricate headphones that accentuate her sharp jawline and bright, inquisitive eyes,
hyper realistic, with fine strands of hair visible, every detail, from the fabric weave of her clothes to the
texture of the headphones, rendered in high definition, 64 megapixels, evoking the cinematic grandeur of a 35mm film,
live-action still, imbued with a moody, atmospheric quality, courtesy of masterful lighting, a subtle film grain,
and a hint of vignette, the image is a testament to the magic of the cinematic arts, reminiscent of the works of
the great Roger Deakins, Hoyte van Hoytema, and Emmanuel Lubezki, with a color grade that recalls the golden hour,
warm, inviting, and visually stunning.
```

Model: Flux Schnell 1.0

Initial Resolution: Medium

Aspect Ratio: 1:1

Runtime: Short

Seed: 2727077839

Overall Prompt Weight: 50%

![01 Female](https://raw.githubusercontent.com/set-soft/KiBot-media/main/podcasts/Avatars/01-female.jpg)


I tried to use them on [Hedra](https://www.hedra.com/), but the IA seems to be regenerating each image, without the
original prompt and a big missmatch in the model you get wrong faces in many frames. Look like they need to apply
face correction (using a GAN).


## 02 Fe/Male

I generated another couple using the previous prompts and the Stable Diffusion model offered by Hedra and got:

![01 Male](https://raw.githubusercontent.com/set-soft/KiBot-media/main/podcasts/Avatars/02-male.webp)

![02 Female](https://raw.githubusercontent.com/set-soft/KiBot-media/main/podcasts/Avatars/02-female.webp)

They get a better animation, with less artifacts.

The bad thing here is the strong limits they impose for a free trial. You can only use 30 seconds audio chunks and
you have 5 tries. This makes it useless to try just one of the NotebookLM generated podcasts. Not to mention you
have to do it twice (fe/male). Even the paid plan puts a 5 minutes limit. My impression is that in october 2024 what they
offer is useless. Note that I found the same for image to video, these technologies are too expensive, so they must
charge for any usable (or close to usable) usage. But the results aren't worth.
