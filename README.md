# ChatFaq Project

## Project Objectives

The ChatFaq project aims to create a user-friendly chatbot using AutoGen. The primary goal is to achieve a basic implementation of AutoGen that allows users to ask questions and receive responses. The project focuses on the integration of conversational AI with an emphasis on text-based interactions.

## Agents Setup

### Conversable Agent

- **Function**: Serves as the communication hub, facilitating information exchange between different agent classes.
- **Responsibilities**: Ensures smooth interaction and data flow within the system.

### Assistant Agent

- **Function**: Acts as the AI brain of the system, utilizing large language models (LLMs) to perform tasks.
- **Responsibilities**: Executes tasks based on the information received but does not interact directly with the user.

### UserProxy Agent

- **Function**: The front-facing agent that interacts directly with the users.
- **Input Restriction**: Limited to text inputs only in this basic implementation.
- **Responsibilities**: Presents the final output or response to the user.

## Workflow

1. **User Interaction**: The user initiates the conversation by asking a question.
2. **Conversable Agent**: Receives the user's question and forwards it to the Group Manager.
3. **Group Manager**: Coordinates with various agents, including the Conversable Agent and Assistant Agent, to process the request.
4. **Response Generation**: The Assistant Agent processes the request and prepares a response.
5. **UserProxy Agent**: Delivers the final response back to the user.

![alt text](AutogenDigram.png)
