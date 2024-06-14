# Use Case
The user can upload a image, and the LLM needs to understand the image. The user can also generate images of a particular scene or add new features from the image by interacting with the LLM chatbot.
## About workflow
This workflow can be divided into two parts: 
1. **Image to Text:** An image is given as input, and text is generated using a custom node.
2.  **LLM Chatbot to Generate Image:** The text is passed to the chatbot, and additional text can also be provided to the bot. The chatbot will return text from which we generate an image.
# Overview
![Workflow]((https://github.com/sribalakumaran/images/blob/main/wholeworkflow.JPG))

git hub link:https://github.com/zhongpei/Comfyui_image2prompt/tree/main

## How to use the workflow
Download the custom nodes using the above git link
Download image to prompt models into the plugin's  `ComfyUI/models/image2text`  directories, respectively. Use the following links for downloading:

-   [Download moondream1 Model](https://huggingface.co/vikhyatk/moondream1)
-   [Download moondream2 Model](https://huggingface.co/vikhyatk/moondream2)
-   [Download internlm-xcomposer2-vl-7b Model](https://huggingface.co/internlm/internlm-xcomposer2-vl-7b)
-   [Download uform-gen2-qwen-500m Model](https://huggingface.co/unum-cloud/uform-gen2-qwen-500m)
-   [Download Qwen-1_8B-Stable-Diffusion-Prompt](https://huggingface.co/hahahafofo/Qwen-1_8B-Stable-Diffusion-Prompt)
-   [Download deepseek-vl-1.3b-chat](https://huggingface.co/deepseek-ai/deepseek-vl-1.3b-chat)
-   [Download deepseek-ai/deepseek-vl-7b-chat](https://huggingface.co/deepseek-ai/deepseek-vl-7b-chat)
Load the input image and add necessary text prompt to change or add features for the image
## Here are some example 
![Input image](https://github.com/sribalakumaran/images/blob/main/download.jpg)
### Image to prompt output

    A red car is depicted in motion on a road, with grass on the ground behind it. A wall is visible on the right side of the image, while the background features trees and a sky overhead.
### Phi3mini Chatbot output

    The scene you've described paints a vivid picture of a dynamic moment captured in a still image or a short video clip. Here's a detailed interpretation of the elements you've mentioned:1. **Red Car in Motion**: The red car is the focal point of the image, likely moving at a moderate to fast pace, depending on the blur of the background and the car's speed. The color red adds a sense of energy and urgency to the scene.2. **Road and Grass**: The road, likely a two-lane or a wider one, provides a clear path for the car's movement. The grass on the ground behind the car suggests that the scene is set in a rural or suburban area, possibly a residential street or a country road. The grass adds a touch of natural beauty and contrasts with the man-made vehicle.3. **Wall on the Right**: The presence of a wall on the right side of the image introduces a sense of scale and context. It could be a barrier, a building, or a natural formation like a cliff or a hillside. The wall's visibility from the car's perspective adds depth to the scene and may influence the car's trajectory or speed.4. **Trees and Sky**: The trees in the background, possibly lining the road or dotting the landscape, provide a sense of place and time. They could be deciduous, with leaves that might change color in the fall, or evergreen, depending on the season. The sky overhead, with its rainy weather, adds a layer of atmosphere and emotion to the scene. The rain could be light, creating a misty effect, or heavy, potentially affecting the car's visibility and the overall mood of the image.5. **Rainy Weather**: The rain adds a dynamic element to the scene, influencing the car's appearance (wet paint, windshield, and windows) and the overall ambiance. The sound of raindrops hitting the car's surface, the wet road, and the rustling of leaves in the wind could be imagined, enhancing the sensory experience of the image.

In summary, this scene captures a moment of motion and contrast between the man-made
### Our text input

    raining weather
![Output image](https://github.com/sribalakumaran/images/blob/main/ComfyUI_temp_jpuop_00013_.png)
