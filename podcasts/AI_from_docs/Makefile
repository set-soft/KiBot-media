#!/usr/bin/make

all: 01_KiBot.mp4 02_KiBot_correction_1.mp4 03_KiBot_correction_2.mp4

01_KiBot.mp4: 01_KiBot.wav ../../logos/cute_robot/AI_depth_to_image/02_metalic_glow.jpg
	ffmpeg -loop 1 -i $(word 2, $^) -i $< -c:v libx264 -tune stillimage -c:a aac -b:a 192k -pix_fmt yuv420p -shortest $@

02_KiBot_correction_1.mp4: 02_KiBot_correction_1.wav ../../logos/cute_robot/AI_depth_to_image/02_metalic_glow.jpg
	ffmpeg -loop 1 -i $(word 2, $^) -i $< -c:v libx264 -tune stillimage -c:a aac -b:a 192k -pix_fmt yuv420p -shortest $@

03_KiBot_correction_2.mp4: 03_KiBot_correction_2.wav ../../logos/cute_robot/AI_depth_to_image/01_plastic_white.jpg
	ffmpeg -loop 1 -i $(word 2, $^) -i $< -c:v libx264 -tune stillimage -c:a aac -b:a 192k -pix_fmt yuv420p -shortest $@
