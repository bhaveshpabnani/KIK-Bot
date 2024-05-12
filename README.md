# 🤖 KIK Bot: AI-Powered Personalized Content Generation

## Table of Contents
1. [Introduction](#introduction)
2. [Problem Description](#problem-description)
3. [Generative AI: Evolution, Key Concepts, Tools, Impact, and Applications](#generative-ai-evolution-key-concepts-tools-impact-and-applications)
4. [Data Collection and Storage](#data-collection-and-storage)
5. [Machine Learning Models](#machine-learning-models)
6. [User Interface](#user-interface)
7. [Privacy and Security Measures](#privacy-and-security-measures)
8. [Conclusion](#conclusion)
9. [Running the Application](#running-the-application)
10. [Requirements](#requirements)
11. [Installation](#installation)
12. [Usage](#usage)
13. [Contributing](#contributing)
14. [License](#license)

## Hosted Link

A live version of the KIK Bot application is available [here](https://kikbot.streamlit.app/).

## Introduction

KIK Bot is an AI-powered system designed to generate personalized content for users. Leveraging advanced natural language processing (NLP) techniques and machine learning models, KIK Bot aims to provide contextually relevant and engaging responses to user queries and prompts. This repository contains the codebase for the KIK Bot application, along with detailed documentation on its architecture, functionality, and implementation.

## Problem Description

The challenge for this hackathon focuses on creating an AI-powered system for generating personalized content, considering key components such as data collection and storage, machine learning model creation, user interface design, and privacy and security measures. The goal is to develop a solution that can effectively understand user inputs, simulate human-like conversations, and generate content tailored to individual preferences and context.

## Generative AI: Evolution, Key Concepts, Tools, Impact, and Applications

Generative AI has undergone significant evolution, moving from early rule-based systems to more sophisticated models capable of creative tasks. Key concepts include natural language generation, deep learning architectures, and advanced neural networks. This section provides an overview of the evolution of generative AI, its key concepts, tools, impact on various industries, and applications in research and development.

## Data Collection and Storage

Effective data collection and storage mechanisms are crucial for the functioning of the KIK Bot application. This section outlines the strategies employed to gather and securely store user-generated content, conversations, and other relevant data. It covers the approach to user input collection, conversation history storage, session management, and secure data handling practices to ensure the confidentiality and integrity of user information.

## Machine Learning Models

In the context of the KIK Bot application, machine learning models serve as the core intelligence that powers the natural language understanding and generation capabilities of the chatbot. This section delves into the specific aspects of the machine learning models used in the application, focusing on the OpenAI GPT-3.5-turbo model, LangChain library, ConversationChain, ConversationEntityMemory, and PromptTemplate components.

## User Interface

The user interface for the KIK Bot application has been developed using Streamlit, a Python library for creating web applications with minimal effort. This section details the components and functionalities of the user interface, including session initialization, user input section, new chat button, sidebar options, conversation display, conversation sessions sidebar, API key input, warning for API key, onboarding information, and privacy dashboard.

## Privacy and Security Measures

Privacy and security measures are paramount in ensuring the protection of user data and maintaining compliance with relevant data protection regulations. This section outlines the implementation of various measures to safeguard user privacy and data security within the KIK Bot application. It covers aspects such as user authentication and API key handling, data anonymization and storage, secure session handling, privacy dashboard, and regular security audits.

## Conclusion

This comprehensive approach to the hackathon problem statement integrates advanced AI model development with meticulous attention to data privacy, user interface design, and security measures. By including insights into Generative AI, participants are encouraged to leverage the evolution, key concepts, tools, impact, and applications of this technology to create a robust and user-centric system. Collaboration across these components promises an innovative solution to the multifaceted challenges presented in this problem statement.

## Running the Application

To run the KIK Bot application locally, follow the instructions below:

### Requirements

- streamlite
- langchain
- openai

### Installation

1. Navigate to the directory where the file is saved in the command window.
2. Install the required packages using pip:
   ```
   pip install -r requirements.txt
   ```

### Usage

1. Run the Streamlit application by executing the following command in the command window:
   ```
   streamlit run KIK.py
   ```
2. Access the application through the provided local URL in your web browser.

## Contributing

Contributions to the KIK Bot project are welcome! If you have ideas for new features, improvements, or bug fixes, please feel free to submit a pull request. For major changes, please open an issue first to discuss the proposed changes.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
