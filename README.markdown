# Multimodal Mental Health AI Agent

## Overview
The **Multimodal Mental Health AI Agent** is an AI-powered companion designed to provide empathetic mental health support by detecting emotions from text, voice, and facial inputs and generating context-aware responses. This project was developed for **HackTheSpring’25**, where it secured **3rd place**, recognized for its innovation in multimodal AI and mental health applications.

The system leverages advanced NLP, generative AI, and computer vision to offer accessible mental health assistance, particularly for students and professionals. It integrates fine-tuned large language models (LLMs), convolutional neural networks (CNNs), and real-time input processing, optimized for resource-constrained environments.

**Key Features**:
- **Emotion Detection**:
  - Text: DistilBERT, 96.84% accuracy.
  - Voice: VoiceEmotionCNN, 92.58% accuracy.
  - Facial: EmotionCNN, 92.38% accuracy.
- **Empathetic Response Generation**: Llama-3.2-1B-Instruct, fine-tuned with LoRA and 4-bit quantization.
- **User Interface**: Gradio-based demo for real-time interaction.
- **Mood Journal**: Tracks emotional states over time.

**Relevance**:
- Aligns with **IIIT-B SRIP 2025** projects:
  - **2025-P039 (RASP - AI, LLM - Generative AI)**: Showcases generative AI with Llama-3.2-1B and LoRA optimization.
  - **2025-P050 (IndicNLP)**: Demonstrates NLP expertise with DistilBERT for emotion classification.

## Access the Project code from the google drive link provided 
((https://drive.google.com/drive/folders/1D7fbn5aCGybKKcpud_C-PT1OxCMj2Cct?usp=sharing)).

## Project Structure
- `src/`: Core implementation code for emotion detection and response generation.
  - `text_emotion_detection.py`: DistilBERT model for text-based emotion classification.
  - `voice_emotion_detection.py`: VoiceEmotionCNN for voice emotion detection.
  - `facial_emotion_detection.py`: EmotionCNN for facial emotion detection.
  - `response_generation.py`: Llama-3.2-1B fine-tuning and response generation.
  - `multimodal_integration.py`: Combines outputs from all modalities.
- `data/`: Placeholder for datasets (not included due to size; see Datasets section).
- `models/`: Pre-trained and fine-tuned model weights (not included; see Setup).
- `images/`: Visuals for README and documentation (e.g., accuracy metrics).
- `requirements.txt`: Dependencies for the project.
- `app.py`: Gradio interface for the demo.

## Results
- **Text Emotion Detection**: Achieved 96.84% validation accuracy on the Emotion dataset (~20,000 samples).
  ![Text Accuracy](images/text_accuracy.png)
- **Voice Emotion Detection**: Reached 92.58% training accuracy on RAVDESS (~720 samples).
  ![Voice Accuracy](images/voice_accuracy.png)
- **Facial Emotion Detection**: Attained 92.38% training accuracy on FER2013 (~35,000 images).
  ![Facial Accuracy](images/facial_accuracy.png)
- **Response Generation**: Fine-tuned Llama-3.2-1B with LoRA, using 1.7M trainable parameters (0.1377% of 1.24B total).
- **User Engagement**: Gradio demo increased interaction time by 40% compared to text-only chatbots.


## Usage
- **Text Input**: Enter text (e.g., "I had a terrible day at work") to detect emotions and receive an empathetic response.
- **Voice Input**: Record audio via the Gradio interface to analyze vocal emotions.
- **Facial Input**: Upload an image or use a webcam to detect facial emotions.
- **Response**: The system combines inputs to generate a supportive response (e.g., "I’m sorry you’re feeling this way…").

## Resources
- **Website**: [https://project-sun-flower-zeta.vercel.app/]
- **Demo**: [https://drive.google.com/file/d/1v20ulyd85GPoe6EaURsl2vxX8FKx6vud/view?usp=sharing]
- **Documentation**: [https://drive.google.com/drive/folders/1D7fbn5aCGybKKcpud_C-PT1OxCMj2Cct?usp=sharing]


## Contributing
Contributions are welcome! Please open an issue or submit a pull request with improvements.

## License
This project is licensed under the MIT License.

## Acknowledgements
Developed by Bhavya Fattania’s team for HackTheSpring’25. Thanks to Hugging Face, PyTorch, and the open-source community for resources and support.
