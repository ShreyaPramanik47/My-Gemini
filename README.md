# My Gemini - Question Answering Tool Using Google Generative AI

This project integrates **Google Generative AI (Gemini API)** with an **Express.js** server to build a tool that answers user questions by generating AI-powered text responses.

## Features:
- **GoogleGenerativeAI Integration**: Utilizes the Gemini 1.5 Flash model for generating content.
- **Express.js Server**: Provides a simple API to handle requests and deliver responses.
- **Environment Variables**: Uses `dotenv` for secure API key management.
- **Body Parser**: Parses incoming JSON request bodies.

## How it Works:
1. The server exposes an API endpoint `/api/content` that accepts a user query (question) via a JSON request body.
2. The query is sent to Google Generative AI's Gemini model, which generates a relevant response.
3. The server sends the response back to the client.

## Example Request:

To ask a question, send a GET request to `/api/content` with the following JSON format:

```json
{
  "question": "Who is Bill Gates?"
}
