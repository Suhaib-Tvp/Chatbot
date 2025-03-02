# FAQ Chatbot

## Overview
The FAQ Chatbot is a Natural Language Processing (NLP)-based chatbot designed to handle frequently asked questions efficiently. It leverages sentence embeddings to understand user queries and provide the most relevant responses. The chatbot supports conversational interactions, entity recognition, and optional logging of conversations.

## Features
- Accepts natural language queries.
- Matches user queries to predefined FAQ responses using sentence embeddings.
- Understands variations in user questions.
- Supports multi-turn interactions.
- Uses Named Entity Recognition (NER) for extracting key information.
- Logs conversations for analysis (optional feature).

## Technologies Used
- **Python**
- **spaCy** for Named Entity Recognition (NER)
- **Sentence Transformers (all-MiniLM-L6-v2)** for embedding-based similarity matching
- **Cosine Similarity** for query matching
- **JSON** for storing chatbot logs

## Installation & Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/faq-chatbot.git
   cd faq-chatbot
   ```
2. Install dependencies:
   ```bash
   pip install spacy sentence-transformers torch
   ```
3. Download the spaCy model:
   ```bash
   python -m spacy download en_core_web_sm
   ```
4. Run the chatbot:
   ```bash
   python chatbot.py
   ```

## Usage
- Start the chatbot and enter your query.
- The chatbot will find the best-matching response using NLP techniques.
- If the confidence score is low, it will prompt you to rephrase the question.
- Type `exit` to stop the chatbot.

## Future Improvements
- Multi-language support.
- Dynamic FAQ updates from a database.
- Enhanced contextual understanding using deep learning models like BERT.

## License
This project is licensed under the MIT License.

