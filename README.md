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
| **Prompt 1 (Wide Angle Driving):** `(a photorealistic image of a (silver Mahindra XUV700:1.5) SUV:1.2), (a modern vehicle with flush pop-out door handles and large C-shaped LED headlights:1.4). The car is driving across the Mumbai Bandra-Worli Sea Link on a sunny day. Wide-angle action shot, cinematic, high 'Overall visual quality'.` | <img width="428" height="389" alt="SeaLink1" src="https://github.com/user-attachments/assets/ed2cac41-fa34-497a-9c2e-e42466881915" /> |
| **Prompt 2 (Side Profile at Sunset):** `(a side profile shot of a (silver Mahindra XUV700:1.5) SUV:1.2), (a modern vehicle with sleek lines and flush pop-out door handles:1.4). The car is parked on the Bandra-Worli Sea Link with a beautiful sunset in the background. Hyper-realistic, warm reflections on the car.` |<img width="393" height="431" alt="SeaLink2" src="https://github.com/user-attachments/assets/f1443e03-297e-47a8-beea-19dcec6bb075" /> |
| **Prompt 3 (Dynamic Front Cornering):** `(a dynamic shot of a (silver Mahindra XUV700:1.5) SUV:1.2), (a modern vehicle with a prominent grille with vertical chrome slats and C-shaped headlights:1.4). The car is cornering on the Bandra-Worli Sea Link at dusk, with city lights blurred in the background. High detail.` |<img width="626" height="380" alt="SeaLink3" src="https://github.com/user-attachments/assets/c0fc2fe0-42f2-45d9-8e71-13d31ea34629" /> |

### Location 2: Rajasthan Hawa Mahal

| Prompt | Generated Output |
| :--- | :--- |
| **Prompt 4 (Front View):** `(a photorealistic image of a (silver Mahindra XUV700:1.5) SUV:1.2), (a modern vehicle with a prominent grille and large C-shaped headlights:1.4). The car is parked on the street directly in front of the magnificent Hawa Mahal in Rajasthan. Bright morning light, sharp focus.` |<img width="601" height="379" alt="HawaMahal1" src="https://github.com/user-attachments/assets/68a72a24-d170-460b-8bc1-6c26aed1a59f" /> |
| **Prompt 5 (Dramatic Low Angle):** `(a dramatic low-angle shot of a (silver Mahindra XUV700:1.5) SUV:1.2), (emphasizing its large grille with vertical slats and modern C-shaped headlights:1.4). The stunning Hawa Mahal rises in the background against a clear blue sky. High 'Overall visual quality'.` |<img width="620" height="376" alt="HawaMahal2" src="https://github.com/user-attachments/assets/2b3c3342-3b25-4759-ad05-450603680d61" /> |
| **Prompt 6 (Side View):** `(a Side view of a (silver Mahindra XUV700:1.5) SUV:1.2), (showcasing its wheels and Flushdoor:1.4). The car is in a lively street scene with the Hawa Mahal visible in the background. The scene is accurate to the described text.` |<img width="611" height="382" alt="HawaMahal3" src="https://github.com/user-attachments/assets/e920cc5e-2a24-4acb-860e-e6032ba0dd7e" /> |

### Location 3: Nagpur Rainforest

| Prompt | Generated Output |
| :--- | :--- |
| **Prompt 7 (Action on Muddy Trail):** `(an action shot of a (silver Mahindra XUV700:1.5) SUV:1.2), (a modern vehicle splashing through a muddy trail:1.4). The car is in a dense, wet Nagpur rainforest with sunbeams filtering through the canopy. Ultra-realistic, motion blur on the wheels.` |<img width="617" height="379" alt="Forest1" src="https://github.com/user-attachments/assets/8062278d-37ae-45cc-9cb0-f6b9836a8b36" /> |
| **Prompt 8 (Parked by a Stream):** `(a serene shot of a (silver Mahindra XUV700:1.5) SUV:1.2), (a modern vehicle parked on mossy rocks beside a clear stream:1.4). The location is a misty Nagpur rainforest. Reflections of the lush greenery are on the car's body.` |<img width="623" height="379" alt="Forest2" src="https://github.com/user-attachments/assets/5387ef50-6227-4f3f-9c36-15b78ff4d66e" /> |
| **Prompt 9 (Side View):** `(an action shot of a (silver Mahindra XV700:1.5) SUV:1.2), (the vehicle is splashing through a muddy puddle on a dirt road, creating dynamic mud splashes:1.4). The scene is a dense, green Nagpur rainforest with sunbeams filtering through the canopy. High 'Overall visual quality'.` |<img width="670" height="341" alt="Forest3" src="https://github.com/user-attachments/assets/2e81f521-6a94-4729-be01-4f6bca393b17" /> |

---

## 🚀 How to Reproduce These Images

**Note:** The Jupyter Notebook (`.ipynb` file) used to generate these images will be uploaded to this repository soon.

Once the notebook is added, you will be able to clone this repository and run the code in Google Colab to create your own images. Stay tuned for the update!
