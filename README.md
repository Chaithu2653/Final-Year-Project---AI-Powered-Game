# AI-Powered Game

## Introduction

The AI-Powered Game project is designed to explore the potential of conversational artificial intelligence within interactive gaming environments. Traditional non-playable characters (NPCs) in games rely on predetermined dialogue trees, offering limited and often repetitive interactions. This project replaces static NPC behavior with dynamic, context-aware conversational agents powered by large language models (LLMs).

By integrating natural language processing, speech synthesis, and memory-based interaction models, this system allows game characters to engage players in real-time, personalized dialogue. These characters are capable of remembering past interactions, responding with emotional nuance, and adjusting their behavior based on ongoing player input, resulting in a more immersive and engaging gaming experience.

## Technology Stack

### Programming Language

- **Python 3.12**: Chosen for its simplicity, rich ecosystem, and compatibility with AI libraries.

### Backend Frameworks and Libraries

- **FastAPI or Flask**: Lightweight web frameworks for handling API requests between the game interface and the AI models.
- **LangChain**: A high-level framework for building applications powered by LLMs, particularly useful for managing prompt templates, memory, and tool integration.
- **OpenAI GPT-3.5 / GPT-4**: The language models used to generate human-like dialogue and reasoning for in-game characters.
- **ChromaDB / FAISS**: Vector databases used to store and retrieve contextual embeddings that support character memory and continuity in conversations.
- **PyAudio and SpeechRecognition**: Used to capture and process voice inputs from players in real-time.
- **ElevenLabs or Edge-TTS**: Text-to-speech services used to convert LLM-generated responses into audio, enabling seamless voice-based interactions with players.

### Optional Frontend and Game Engine Integration

- **React or Three.js**: Can be used for custom game UI overlays that display dialogue and interaction logs.
- **Unity or Unreal Engine**: For integrating AI logic into 3D or 2D gameplay environments, including triggering animations, actions, or events based on conversational cues.

### Supporting Tools

- **pipwin**: Simplifies installation of Windows-specific binary dependencies.
- **Virtual Environments**: Used to isolate dependencies and maintain reproducible environments across systems.

## System Overview

The core functionality of the AI-Powered Game is organized around several coordinated components:

1. **Voice Input Processing**: 
   Players speak into a microphone. Their voice is captured using `PyAudio` and transcribed using `SpeechRecognition`.

2. **Query Handling and LLM Response Generation**:
   The transcribed input is processed through LangChain and sent to an LLM. The model evaluates the current context, relevant memory embeddings, and user intent before generating a response.

3. **Contextual Memory Management**:
   ChromaDB or FAISS stores conversation history and embeddings. This allows the NPC to maintain long-term memory, improving character consistency and realism over time.

4. **Text-to-Speech Rendering**:
   The generated response is vocalized using ElevenLabs or Edge-TTS. Voice output is either streamed back to the player or played within the game client.

5. **Game Logic Integration**:
   The backend can trigger in-game events or actions based on the player's statements. For example, asking a character for help may unlock a quest or provide critical game hints.


## Limitations

While the project showcases promising results, several limitations remain:

- **Latency**: Processing time for speech recognition, LLM inference, and speech synthesis can introduce noticeable delays.
- **API Dependency and Cost**: Relying on commercial APIs like OpenAI and ElevenLabs can result in high operational costs, especially in large-scale games.
- **Offline Capability**: Most models require internet connectivity and cloud infrastructure. Offline support is limited without major sacrifices in quality.
- **Emotion and Personality Modeling**: While memory and tone can be adjusted, achieving nuanced emotional modeling and long-term character development still poses challenges.
- **Scalability**: Integrating AI-powered NPCs in large-scale multiplayer environments requires robust infrastructure and load balancing strategies.

## Conclusion

The AI-Powered Game project demonstrates how LLMs can be used to enhance game interactivity by enabling intelligent and emotionally responsive NPCs. By incorporating memory, voice interaction, and real-time response generation, the system significantly improves the depth and flexibility of in-game dialogue.

## Team

| Name               | GitHub Profile                                          |
|--------------------|---------------------------------------------------------|
| Chinmayee N Holla    | [github.com/chinholla](https://github.com/ChinmayeeHolla) |
| Chaithu A | [github.com/Chaithu2653](https://github.com/Chaithu2653)                           |
| B M Nitish Kumar | [github.com/BMNITISHKUMAR](https://github.com/BMNITISHKUMAR)                           |
| Nuthank K Gowda | [github.com/NuthanKGowda](https://github.com/NuthanKGowda)                         |
