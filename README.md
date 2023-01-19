# Gradio for Stable Diffusion

The goal of this project was making an interactive app for Stable Diffusion using Gradio so that I can experiment with Stable Diffusion more easily, and also share it with friends. 

I initially used the 'Interface' class to build one for image-to-image and another for inpainting. But I ended up with the 'Blocks' class so that I can combine the two models into one app using the tabs. The notebook file [Gradio_Img2Img-Inpainting-SD2_Share.ipynb](https://github.com/sooolee/gradio-stable-diffusion/blob/main/Gradio_Img2Img-Inpainting-SD2_Share.ipynb) is shared here. 

![gradio](https://github.com/sooolee/gradio-stable-diffusion/blob/main/images/gradio.png?raw=true)


## Having Fun with Stable Diffusion v2 Image-to-Image

I used my own sketch of a bathroom with a prompt like "A photo of a bathroom with a bay window, free-standing bathtub with legs, a vanity unit with wood cupboard, wood floor, white walls, highly detailed, full view, symmetrical, interior magazine style" Also used a negative prompt of "unsymmetrical, artifacts, blurry, watermark, signs, text." 

Some of the samples I liked are shown below. Some of the seeds were reused.

![sketch-to-photos-bath](https://github.com/sooolee/gradio-stable-diffusion/blob/main/images/sketch-to-photos-bath.png?raw=true)

Using a professional sketch didn't make much difference in my opinion. Below are some samples of the generated bedrooms based on a professional sketch. 

Prompt used: "A photo of a bedroom, full room view, a bed in the middle, nightstands, ceiling with molding, wooden floor, wall closet on a side, centered symmetrical composition, 4K, 8K, highly detailed, interior magazine style."

![sketch-to-photos-bedroom](https://github.com/sooolee/gradio-stable-diffusion/blob/main/images/sketch-to-photos-bedroom.png?raw=true)

I got curious about how well the algorithm would generate architectural sketches based on a sketch. I got pretty interesting results.

![sketch-to-sketch](https://github.com/sooolee/gradio-stable-diffusion/blob/main/images/sketch-to-sketch.png?raw=true)

## Modifying Images using Stable Diffusion Inpainting

I really like the inpainting model. I have been modifying my personal photos using this model for fun. 

Below are some modified images using Inpainting. I re-fed some of the img-2-img outputs into Inpainting model in order to variate them. 

![img2img_inpainting](https://github.com/sooolee/gradio-stable-diffusion/blob/main/images/img-2-img_inpainting.gif?raw=true)

Another example of image modificiation is where I sequentially looped the modified versions of an image for continued changes. (I haven't built the looping function within Gradio as of this moment. It was manual feeds.)

![img_modification](https://github.com/sooolee/gradio-stable-diffusion/blob/main/images/img_modification_inpainting.gif?raw=true)

## What's Next?

Gradio is really cool. I plan to imrove the tool to add the txt-to-img model (another tab), looping between models (tabs), and looping within a model (tab). 
