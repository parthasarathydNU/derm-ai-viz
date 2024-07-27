## DermAI-Viz: AI-Driven Skin Condition Visualization

DermAI-Viz is a pioneering platform that utilizes deep learning to simulate the progression and treatment outcomes of various skin conditions. By generating realistic images of skin rashes, this tool aids dermatologists in diagnosis and treatment planning, and serves as an educational resource for medical students.

### Features

- **Visualize Skin Conditions**: Generates images showing the progression of skin conditions over time.
- **Treatment Outcome Simulation**: Helps predict the response of skin conditions to various treatments.
- **Supports Diverse Skin Types**: Includes data across different skin colors and types to ensure broad applicability.

### Technical Stack

- **Diffusion Models**: Utilizes state-of-the-art generative models for high-quality image synthesis.
- **Python**: Built using Python with libraries such as TensorFlow and PyTorch for model implementation.
- **Web Interface**: Easy-to-use web interface for interacting with the model outputs.

### Usage

Navigate to the hosted web interface, select a skin condition and its parameters, and use the model to generate visual progressions and treatment responses.

### Current State:
- Figured out how to train a Diffusion Model on custom data using a simple Unet : [Notebook](https://github.com/parthasarathydNU/gen-ai-coursework/blob/main/diffusion/diffusers.ipynb)

### Contributing

We welcome contributions from the community, including feature enhancements, bug fixes, and documentation improvements. Please fork the repository, make your changes, and submit a pull request.

### License

Distributed under the MIT License. See `LICENSE` for more information.

### Acknowledgments

- Collaborators and data providers from dermatological institutions
- Open-source projects and libraries that inspired and supported our development
