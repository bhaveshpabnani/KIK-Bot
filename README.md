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


![image](https://github.com/bhaveshpabnani/KIK-Bot/assets/132581707/2559d18c-7537-4780-a187-05d7228698cd)

## Introduction

KIK Bot is an AI-powered system designed to generate personalized content for users. Leveraging advanced natural language processing (NLP) techniques and machine learning models, KIK Bot aims to provide contextually relevant and engaging responses to user queries and prompts. This repository contains the codebase for the KIK Bot application, along with detailed documentation on its architecture, functionality, and implementation.

## Problem Description

The challenge for this hackathon focuses on creating an AI-powered system for generating personalized content, considering key components such as data collection and storage, machine learning model creation, user interface design, and privacy and security measures. The goal is to develop a solution that can effectively understand user inputs, simulate human-like conversations, and generate content tailored to individual preferences and context.

## Generative AI: Evolution, Key Concepts, Tools, Impact, and Applications

Generative AI has undergone significant evolution, moving from early rule-based systems to more sophisticated models capable of creative tasks. Key concepts include natural language generation, deep learning architectures, and advanced neural networks. This section provides an overview of the evolution of generative AI, its key concepts, tools, impact on various industries, and applications in research and development.

## Data Collection and Storage

Effective data collection and storage mechanisms are crucial for the functioning of the KIK Bot application. This section outlines the strategies employed to gather and securely store user-generated content, conversations, and other relevant data. It covers the approach to user input collection, conversation history storage, session management, and secure data handling practices to ensure the confidentiality and integrity of user information. This section provides an overview of how user data is collected, stored, and managed within the
KIK Bot application. The implementation details highlight the seamless interaction between
users and the AI assistant, with a focus on preserving conversation history and enabling
personalized content generation.

### 1. User Input Collection:

The primary source of data for the KIK Bot is the user's input, which includes text-based
conversations, thoughts, and queries. The Streamlit application provides a user-friendly
interface for collecting this input. The `get_text` function, implemented using Streamlit's
`st.text_input` method, enables users to interact with the AI assistant seamlessly. User input is
captured through this interface, forming the basis for personalized content generation.

### 2. Conversation History Storage:

The KIK Bot maintains a comprehensive record of user interactions, preserving both user inputs
and the AI-generated responses. The `st.session_state` object is leveraged to store and
manage this conversation history. Each user input and corresponding AI-generated output are
appended to the session state, enabling a continuous and coherent dialogue throughout the
user's interaction with the AI.

### 3. Session Management and Reset:

To enhance user experience and facilitate continuous learning, the KIK Bot allows users to
initiate new chats. The `new_chat` function clears the session state, creating a clean slate for
the AI assistant to engage with users afresh. Additionally, the ability to store and retrieve
previous chat sessions provides users with a convenient way to revisit and download past
conversations.

### 4. Secure Data Handling:

Security and privacy considerations are paramount in handling user data. While the code
snippets provided focus on functionality, it is crucial to implement best practices for data
encryption, access control, and secure storage to ensure the confidentiality and integrity of user
information.

## Machine Learning Models

In the context of the KIK Bot application, machine learning models serve as the core intelligence that powers the natural language understanding and generation capabilities of the chatbot. This section delves into the specific aspects of the machine learning models used in the application, focusing on the OpenAI GPT-3.5-turbo model, LangChain library, ConversationChain, ConversationEntityMemory, and PromptTemplate components. In this section, we'll delve into the specific aspects of the machine learning models used in the application.

### OpenAI GPT-3.5-turbo Model:
The primary machine learning model utilized in the KIK Bot application is the OpenAI GPT-3.5-turbo. GPT-3.5-turbo is a state-of-the-art language model developed by OpenAI, and it excels in natural language understanding and generation tasks. It is capable of generating contextually relevant and coherent responses based on the input it receives.

Initialization:

The GPT-3.5-turbo model is initialized using the OpenAI API key provided by the user. The API
key establishes a secure connection to OpenAI's servers, allowing the application to interact
with the GPT-3.5-turbo model for text-based tasks.

Usage in ConversationChain:

The ConversationChain, a component of the LangChain library, leverages the GPT-3.5-turbo
model to generate responses during conversations. It handles the interaction flow, incorporating
the historical chat context and user inputs to create a seamless and context-aware
conversational experience.

### LangChain Library:

The LangChain library acts as a facilitator for building conversational agents by providing
abstractions and components that simplify the integration of language models. It encapsulates
various functionalities, such as conversation management, memory storage, and prompt
generation, making it easier for developers to create sophisticated chat applications.

ConversationChain:

ConversationChain is a key component of the LangChain library used to manage and
orchestrate conversations. It integrates with the GPT-3.5-turbo model, handling the generation
of responses and maintaining the conversation history.

ConversationEntityMemory:

The ConversationEntityMemory component is responsible for managing the memory of the
chatbot. It stores important entities, user preferences, and contextual information to enhance the
personalization of responses. The memory is persistent across conversations, allowing the bot
to retain information about the user's preferences and writing style.

PromptTemplate:

PromptTemplate is employed to structure the prompts sent to the GPT-3.5-turbo model. It
defines placeholders for dynamic content, such as chat history and user input, enabling the
generation of coherent and context-aware responses.

### Memory Management:

Efficient memory management is crucial for creating a chatbot that can provide personalized
and contextually relevant responses. In the KIK Bot application, the ConversationEntityMemory
and ConversationBufferMemory components play a vital role in storing and retrieving
information.

ConversationEntityMemory:

This memory module stores entities and user-specific information, allowing the bot to adapt its
responses based on the user's preferences and historical interactions.

ConversationBufferMemory:

The ConversationBufferMemory serves as a short-term memory buffer, storing recent chat
history to maintain context within the current conversation. It enhances the coherence of
responses by considering recent user inputs.

In summary, the Machine Learning Models in the KIK Bot application, powered by OpenAI
GPT-3.5-turbo and supported by the LangChain library, enable a personalized and
context-aware conversational experience. These models, coupled with effective memory
management, contribute to the bot's ability to simulate human-like interactions and generate
content tailored to the user's writing style and preferences.

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
