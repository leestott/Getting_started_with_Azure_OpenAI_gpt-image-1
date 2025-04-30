# Getting started with OpenAI gpt-image-1 on Azure AI Foundry

## Overview
This project demonstrates how to use Azure OpenAI's `gpt-image-1` model to generate images from text prompts. The `gpt-image-1` model, also known as DALL-E 3, allows users to create high-quality, ultra-realistic images by providing descriptive prompts. This repository includes a Jupyter Notebook that guides you through the process of setting up and using the model.

## Prerequisites
Before you begin, ensure you have the following:

1. **Azure OpenAI Resource**: An Azure OpenAI resource with the `gpt-image-1` model deployed.
2. **Python Environment**: Python 3.7 or later installed on your system.
3. **Required Libraries**: Install the necessary Python libraries listed below.
4. **.env File**: Create a `.env` file in the project folder with the following keys:
   ```
   AZURE_API_KEY=<your-azure-api-key>
   AZURE_OPENAI_ENDPOINT=<your-azure-endpoint>
   AZURE_OPENAI_MODEL=gpt-image-1
   ```

## Getting Started
Follow these steps to generate images from text prompts:

1. **Clone the Repository**
   ```bash
   git clone <repository-url>
   cd gpt-image-1
   ```

2. **Install Required Libraries**
   Run the following command to install the necessary Python packages:
   ```bash
   pip install openai>=1.0.0 python-dotenv pillow matplotlib
   ```

3. **Set Up Environment Variables**
   Create a `.env` file in the project folder and add your Azure OpenAI credentials as shown in the prerequisites section.

4. **Run the Notebook**
   Open the `gpt-image-1.ipynb` notebook in Jupyter Notebook or JupyterLab and follow the instructions provided in the cells. The notebook includes:
   - Setting up the Azure OpenAI client.
   - Generating images from predefined and custom prompts.
   - Displaying the generated images.

## Example Prompt
Here’s an example of a prompt you can use to generate an image:

```
A futuristic city skyline at sunset, vibrant colors, ultra-realistic, 4K
```

The model will generate an image based on the description provided in the prompt. You can experiment with different prompts to create unique images.

## Notes
- The available image sizes for the `gpt-image-1` model are:
  - `1024x1024` (square)
  - `1536x1024` (landscape)
  - `1024x1536` (portrait)
- Ensure your Azure OpenAI resource is properly configured and accessible.

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.
