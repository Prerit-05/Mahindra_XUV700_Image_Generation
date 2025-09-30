# 🚗 Mahindra XUV700 - An AI Imagery Showcase

![Showcase Banner](./output_images/HawaMahal1.jpg)
_A photorealistic AI-generated image of the Mahindra XUV700 at the Hawa Mahal, Jaipur._

---

## 🌟 Overview

This project showcases the power of generative AI to create high-quality, photorealistic images of a specific product—the **silver Mahindra XUV700**—in a variety of iconic Indian locations. By leveraging Stable Diffusion XL, ControlNet, and the IP-Adapter, we can control the car's appearance, pose, and setting with remarkable precision.

## ✨ Features

* **Consistent Product Identity:** The IP-Adapter ensures the Mahindra XUV700 maintains its distinct silver color, branding, and key features across all images.
* **Compositional Control:** ControlNet (using Canny edges) dictates the exact pose, angle, and placement of the vehicle in each scene.
* **Photorealistic Environments:** Generates stunningly detailed and context-aware backgrounds, from the Mumbai Sea Link to the rainforests of Nagpur.
* **Customizable Prompts:** Easily adaptable prompts to place the vehicle in any imagined scenario.

## 🛠️ Technology Stack

* **Base Model:** [SG161222/RealVisXL_V4.0](https://huggingface.co/SG161222/RealVisXL_V4.0) for photorealistic image generation.
* **Control Model:** [diffusers/controlnet-canny-sdxl-1.0](https://huggingface.co/diffusers/controlnet-canny-sdxl-1.0) for precise composition control.
* **Image Adapter:** [h94/IP-Adapter](https://huggingface.co/h94/IP-Adapter) for transferring the vehicle's visual characteristics from a reference image.
* **VAE:** [madebyollin/sdxl-vae-fp16-fix](https://huggingface.co/madebyollin/sdxl-vae-fp16-fix) for improved image detail and color.
* **Framework:** [Diffusers 🤗](https://github.com/huggingface/diffusers) on Python with PyTorch.

---

## 🎨 Prompts & Generated Output Showcase

Below are the specific prompts used to generate the images.

### General Negative Prompt
This negative prompt was used for **all** generations to improve quality and avoid common AI artifacts.

> `low quality, worst quality, blurry, noisy, jpeg artifacts, cartoon, anime, drawing, painting, illustration, 3d render, CGI, video game graphics, deformed, disfigured, distorted, mutated, wrong logo, text, watermark, signature, ugly, boring`

### Location 1: Mumbai Bandra-Worli Sea Link

| Prompt | Generated Output |
| :--- | :--- |
| **Prompt 1 (Wide Angle Driving):** `(a photorealistic image of a (silver Mahindra XUV700:1.5) SUV:1.2), (a modern vehicle with flush pop-out door handles and large C-shaped LED headlights:1.4). The car is driving across the Mumbai Bandra-Worli Sea Link on a sunny day. Wide-angle action shot, cinematic, high 'Overall visual quality'.` | ![Bandra-Worli Sea Link Driving](./output_images/SeaLink1.jpg) |
| **Prompt 2 (Side Profile at Sunset):** `(a side profile shot of a (silver Mahindra XUV700:1.5) SUV:1.2), (a modern vehicle with sleek lines and flush pop-out door handles:1.4). The car is parked on the Bandra-Worli Sea Link with a beautiful sunset in the background. Hyper-realistic, warm reflections on the car.` | ![Bandra-Worli Sea Link Sunset](./output_images/SeaLink2.jpg) |
| **Prompt 3 (Dynamic Front Cornering):** `(a dynamic shot of a (silver Mahindra XUV700:1.5) SUV:1.2), (a modern vehicle with a prominent grille with vertical chrome slats and C-shaped headlights:1.4). The car is cornering on the Bandra-Worli Sea Link at dusk, with city lights blurred in the background. High detail.` | ![Bandra-Worli Sea Link Cornering](./output_images/SeaLink3.jpg) |


### Location 2: Rajasthan Hawa Mahal

| Prompt | Generated Output |
| :--- | :--- |
| **Prompt 4 (Front View):** `(a photorealistic image of a (silver Mahindra XUV700:1.5) SUV:1.2), (a modern vehicle with a prominent grille and large C-shaped headlights:1.4). The car is parked on the street directly in front of the magnificent Hawa Mahal in Rajasthan. Bright morning light, sharp focus.` | ![Hawa Mahal Front View](./output_images/HawaMahal1.jpg) |
| **Prompt 5 (Dramatic Low Angle):** `(a dramatic low-angle shot of a (silver Mahindra XUV700:1.5) SUV:1.2), (emphasizing its large grille with vertical slats and modern C-shaped headlights:1.4). The stunning Hawa Mahal rises in the background against a clear blue sky. High 'Overall visual quality'.` | ![Hawa Mahal Low Angle](./output_images/HawaMahal2.jpg) |
| **Prompt 6 (Side View):** `(a Side view of a (silver Mahindra XUV700:1.5) SUV:1.2), (showcasing its wheels and Flushdoor:1.4). The car is in a lively street scene with the Hawa Mahal visible in the background. The scene is accurate to the described text.` | ![Hawa Mahal Side View](./output_images/HawaMahal3.jpg) |


### Location 3: Nagpur Rainforest

| Prompt | Generated Output |
| :--- | :--- |
| **Prompt 7 (Action on Muddy Trail):** `(an action shot of a (silver Mahindra XUV700:1.5) SUV:1.2), (a modern vehicle splashing through a muddy trail:1.4). The car is in a dense, wet Nagpur rainforest with sunbeams filtering through the canopy. Ultra-realistic, motion blur on the wheels.` | ![Nagpur Rainforest Muddy Trail](./output_images/Forest1.jpg) |
| **Prompt 8 (Parked by a Stream):** `(a serene shot of a (silver Mahindra XUV700:1.5) SUV:1.2), (a modern vehicle parked on mossy rocks beside a clear stream:1.4). The location is a misty Nagpur rainforest. Reflections of the lush greenery are on the car's body.` | ![Nagpur Rainforest by Stream](./output_images/Forest2.jpg) |
| **Prompt 9 (Side View):** `(an action shot of a (silver Mahindra XV700:1.5) SUV:1.2), (the vehicle is splashing through a muddy puddle on a dirt road, creating dynamic mud splashes:1.4). The scene is a dense, green Nagpur rainforest with sunbeams filtering through the canopy. High 'Overall visual quality'.` | ![Nagpur Rainforest Splashing](./output_images/Forest3.jpg) |

---

## 🚀 How to Reproduce These Images

**Note:** The Jupyter Notebook (`.ipynb` file) used to generate these images will be uploaded to this repository soon.

Once the notebook is added, you will be able to clone this repository and run the code in Google Colab to create your own images. Stay tuned for the update!
