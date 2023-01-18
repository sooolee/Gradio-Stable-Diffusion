# Gradio for Stable Diffusion

The goal of this project was making an interactive app for Stable Diffusion using Gradio so that I can experiment with Stable Diffusion more easily, and also share it with friends. 

I initially used the Interface class to build one for image-to-image and another for inpainting. But I ended up using the Blocks class so that I can combine the two models into one app using the tabs. The notebook file `Gradio_Img2Img-Inpainting-SD2_Share.ipynb` is shared here. 

![gradio]

## Having Fun with Stable Diffusion v2 Image-to-Image

I used my own sketch of a bathroom with a prompt like "A photo of a bathroom with a bay window, free-standing bathtub with legs, a vanity unit with wood cupboard, wood floor, white walls, highly detailed, full view, symmetrical, interior magazine style" Also used a negative prompt of "unsymmetrical, artifacts, blurry, watermark, signs, text." Some of the seeds are reused.

![sketch-to-photos-bath]

Using a professional sketch of a bedroom didn't make much difference in my opinion. Prompt = "Photo of a bedroom, full room view, a bed in the middle, nightstands, ceiling with molding, wooden floor, wall closet on a side, centered symmetrical composition, 4K, 8K, highly detailed, interior magazine style."

![sketch-to-photos-bedroom]

I got curious how well it would generate a sketch based on a sketch. 

![sketch-to-sketch]

## Stable Diffusion v2 Inpainting

I re-fed some of the img-2-img outputs into Inpainting model in order to variate or improve the images. 

![inpainting]

Another example of image modificiation below is where I sequentially looped the modified versions of the image for continued changes in one image. (I haven't built the looping function within Gradio as of this moment. It was manual feed.)


![img-modification](https://drive.google.com/file/d/1r7A3OD22wCzqD8w893uH8YdYzm0cs19s/view?usp=share_link)

![img-modification](/Users/seulkeelee/Downloads/img_modification_inpainting.mp4)


<video width="320" height="240" controls>
  <source src="https://drive.google.com/file/d/1r7A3OD22wCzqD8w893uH8YdYzm0cs19s/view?usp=share_link" type="video/mp4">
</video>