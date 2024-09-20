#!/usr/bin/make

01_KiBot.mp4: 01_KiBot.wav ../../logos/cute_robot/AI_depth_to_image/02_metalic_glow.jpg
	ffmpeg -loop 1 -i $(word 2, $^) -i $< -c:v libx264 -tune stillimage -c:a aac -b:a 192k -pix_fmt yuv420p -shortest $@
