# Glotchy_writeup
Writeup for the Glotcy chall from MidnightCTF


(dont have any links of image off the challsplay/website)
The chall linked to a webpage with a background of scanlines from a crt-tv.
In the middle of the page was this;
![image](https://github.com/user-attachments/assets/7ba771b2-1156-41a5-9fb6-5c956d053c1d)

You could do inspect and see flag.png and download just the image.


From the scanlines refrence i guess you needed to reorder the horizontal lines of the image to  be able to read whats on the image.

I used this python script; https://github.com/SadEmoji/Python_scripts/blob/main/Image_slicer.py
to slice the image into the lines 1 pixel high with the full width.

Then i used this python script; https://github.com/SadEmoji/Python_scripts/blob/main/Image_arrange_sort_color.py
to sort the lines based on brightness of the colors and add them back into a image
I got this image from it;
![Skärmavbild 2025-05-20 kl  12 42 59](https://github.com/user-attachments/assets/a5a0194e-dc1a-4df9-9041-848f0c50afc4)

It is blocky and still not readble but now human-sortable.

I bring it into gimp and first line it up, i realise the pink is to show diffrences from when its diagonal  

So i sort the blocks and get the flag;
<img width="1203" alt="Skärmavbild 2025-05-17 kl  17 16 27" src="https://github.com/user-attachments/assets/4381095b-10ce-4397-a4bf-7653a7f72656" />
