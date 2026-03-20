![image](https://i.imgur.com/j7V7Tn5.jpeg)

# <p align="center">Gllum</p>

Interact with locally running large language models (LLM's). Gllum provides an easy-to-use and familiar UI, with message persistence, and vector embeddings for retrieval-augmented generated (RAG) functionality.

Within each chat, it is possible to change models mid-conversation. 

You can use a multi-modal model like llama-vision to upload an image of a math problem, then switch to mathstral to provide a solution, and finally switch to codestral to give you a code for the solution, all within the same chat.

### Home:

![image](https://i.imgur.com/TzcyBft.jpeg)

### Switching models during a conversation (+markdown and math-mode support):

![image](https://i.imgur.com/p1tVQP1.jpeg)

### Describing images with multi-modal LLMs:

![image](https://i.imgur.com/zCY7Wci.jpeg)

### Model switcher + chat editing:
![image](https://i.imgur.com/yIS3eke.jpeg)



---

# How to run

You need to have a local Ollama server running to use this!
Run Ollama with ```OLLAMA_HOST=0.0.0.0 ollama serve```

Enter the URL of your Ollama server (Your IP Address + ":11434") in the const `OLLAMA_SERVER` in [/backend/data/global.go](https://github.com/dnvie/LocalLLM/blob/main/backend/data/global.go).

(Note: Currently, the embedding model is hardcoded, therefore you need to have "snowflake-arctic-embed2" installed.)

Run the backend with `go run main.go` while in the /backend directory.

Run the frontend with `ng serve` while in the /frontend/src directory.

-----------------------------------------------------------------------------------

Future upgrades:
- User system
- Ability to pull new models directly from within the UI
- Ability to set a default model
- Temporary Chats
- Add a lightweight LLM to generate chat titles
- Support for various screen sizes
- Add ability to search the web
