# RAG Chatbot Project

## Overview
The RAG (Retrieval-Augmented Generation) Chatbot is an advanced conversational agent that leverages large language models and retrieval systems to provide accurate and relevant responses based on user queries.

## Features
- **Natural Language Understanding**: Capable of understanding and processing user inputs in natural language.
- **Dynamic Information Retrieval**: Utilizes external knowledge sources to provide up-to-date and accurate information.
- **Multi-turn Conversations**: Maintains context across multiple interactions.
- **Easy Integration**: Simple API endpoints for seamless integration with various applications.

## Installation Instructions
1. **Clone the repository**:
   ```bash
   git clone https://github.com/Ahmad000farhan/Java.git
   ```
2. **Navigate into the project directory**:
   ```bash
   cd Java
   ```
3. **Install dependencies**:
   ```bash
   ./gradlew install 
   ```
4. **Run the application**:
   ```bash
   ./gradlew run
   ```

## API Endpoints
- **POST /api/chat**: Initiates a conversation based on the user's input.
  - **Request Body**:
    ```json
    {
      "userInput": "Your message here"
    }
    ```
- **GET /api/history**: Retrieves the conversation history.
  - **Response**:
    ```json
    {
      "history": [
        "Previous message 1",
        "Previous message 2"
      ]
    }
    ```

## Architecture
The RAG Chatbot consists of the following components:
- **Client**: The front-end interface where users interact with the chatbot.
- **API Server**: Handles requests from clients and manages the logic of the chatbot.
- **Retrieval System**: Interfaces with external knowledge bases to retrieve relevant information.
- **Language Model**: Processes user input and generates appropriate responses based on the retrieved data.

## Usage Examples
1. **Starting a conversation**:
   ```bash
   curl -X POST http://localhost:8080/api/chat -H "Content-Type: application/json" -d '{"userInput":"Hello, chatbot!"}'
   ```
2. **Retrieving conversation history**:
   ```bash
   curl -X GET http://localhost:8080/api/history
   ```

## License
Licensed under the MIT License. See [LICENSE](LICENSE) for details.

## Acknowledgments
- Thanks to previous contributors and the open-source community for their valuable resources and tools that made this project possible.