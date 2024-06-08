# SAM and Inpainting

This folder contains images related to segmentation and inpainting.

Files prefixed with inpaint are the outputs of the inpainting,
files prefixed with screenshot are the screen captures, showing also the masks and prompts.

## Dragon
Everything related to dragon uses the supplied dragon image.

3 runs have been done:
- using defaults (medieval village)
- for a castle background
- more modern style, with other toys

## Mona Lisa
Everything related to monalisa uses the supplied Mona Lisa image.

4 runs have been done:
- using the defaults (creating the dragon background)
- 3 iterations, using the output of the first as input, and changing the subject. One to replace the woman by a cat, and 2 to replace her by a man.

## Fox
fox512 is a picture from wikipedia. The fox has been replaced by a zebra.

## Knight
knight-armor-old is another pictire from the web.
The knight has been placed in front of a shopping center.
2 additional variants have been generated, using lower and higher values for the Classifier-Free Guidance Scale.


# Execution Notes
Runs have been done on my local machine. Unless caused by other issues, I had some issues getting it to work with some versions of gradio.
I finally installed 4.25.0 and that worked for me.
