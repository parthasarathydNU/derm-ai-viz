## DermAI-Viz: AI-Driven Skin Condition Visualization

DermAI-Viz is a pioneering platform that utilizes deep learning to simulate the progression and treatment outcomes of various skin conditions. By generating realistic images of skin rashes, this tool aids dermatologists in diagnosis and treatment planning, and serves as an educational resource for medical students.


> Generating skin rash examples using a diffusion model
> 
> ![GIF-2024-07-27-09-30-26](https://github.com/user-attachments/assets/55a51acb-ff1b-4b11-b4df-59379d25aaac)
>
> This model needs more work right now the images look blurry

> Generating images of butterflies using a diffusion model
> 
> ![denoising_process](https://github.com/user-attachments/assets/531ac252-f1ec-4c0b-98b4-ada2c6d9bdc0)



### Features

- **Visualize Skin Conditions**: Generates images showing the progression of skin conditions over time.
- **Treatment Outcome Simulation**: Helps predict the response of skin conditions to various treatments.
- **Supports Diverse Skin Types**: Includes data across different skin colors and types to ensure broad applicability.

### Technical Stack

- **Diffusion Models**: Utilizes state-of-the-art generative models for high-quality image synthesis.
- **Python**: Built using Python with libraries such as TensorFlow and PyTorch for model implementation.
- **Web Interface**: Easy-to-use web interface for interacting with the model outputs.

### Current State:
- ~~Figured out how to train a Diffusion Model on custom data using a simple Unet : [Notebook](https://github.com/parthasarathydNU/gen-ai-coursework/blob/main/diffusion/diffusers.ipynb)~~
- ~~Trained a simple model and uploaded it on HuggingFace : [DhruvParth/sd-class-skinrash-64](https://huggingface.co/DhruvParth/sd-class-skinrash-64)~~
- ~~Trained V2 Model : [DhruvParth/ddpm-celebahq-256-fineTuned-skin_rash_v2_12epochs](https://huggingface.co/DhruvParth/ddpm-celebahq-256-fineTuned-skin_rash_v2_12epochs)~~
- Explored Guidance using the CLIP model from OpenAI to generate rash images from text based prompt: [Notebook](https://github.com/parthasarathydNU/derm-ai-viz/blob/main/notebooks/guidance.ipynb)

### Model:
```python
from diffusers import DDPMPipeline
pipeline = DDPMPipeline.from_pretrained('DhruvParth/ddpm-celebahq-256-fineTuned-skin_rash_v2_12epochs')
image = pipeline().images[0]
image
```
![GIF-2024-07-27-09-30-26](https://github.com/user-attachments/assets/92ad5640-540d-47ff-aeb3-54153bd8f583)

### Contributing

We welcome contributions from the community, including feature enhancements, bug fixes, and documentation improvements. Please fork the repository, make your changes, and submit a pull request.

### License

Distributed under the MIT License. See `LICENSE` for more information.

### Acknowledgments

- Collaborators and data providers from dermatological institutions
- Open-source projects and libraries that inspired and supported our development
