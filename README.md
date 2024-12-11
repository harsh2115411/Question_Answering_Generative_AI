# Q&A System Using T5 Transformer

## Project Overview
This project implements a Question-and-Answer (Q&A) system using the T5 (Text-to-Text Transfer Transformer) model. The system retrieves transcripts from YouTube videos, processes the text to extract relevant content, and generates answers to user queries.

## Features
- **Transcript Retrieval**: Extracts and processes transcripts from YouTube videos.
- **Context Extraction**: Uses BM25 to identify the most relevant parts of the transcript.
- **Answer Generation**: Generates concise answers to user questions using the T5 model.

## Tools and Technologies Used
- **Python**
  - Transformers (Hugging Face)
  - NLTK
  - rank_bm25
  - youtube-transcript-api
- **T5 Model**
  - Pre-trained models like `t5-base` or `t5-large`.
- **Jupyter Notebook**

## Project Workflow
1. **Transcript Fetching**:
   - The system uses the YouTube Transcript API to fetch transcripts of videos.
2. **Text Preprocessing**:
   - Splits the transcript into manageable chunks using NLTK.
3. **Context Retrieval**:
   - Applies BM25 to score and retrieve the most relevant chunks of text for the given question.
4. **Answer Generation**:
   - T5 transformer model generates answers based on the extracted context.


## Highlights
- **Scalable Solution**: Designed to handle transcripts of varying lengths and complexities.
- **High Accuracy**: Combines advanced NLP retrieval techniques with state-of-the-art transformer models.
- **Real-World Application**: Provides actionable insights from video content, enabling efficient information retrieval.


## Usage
1. Open the Jupyter Notebook:
   ```bash
   jupyter notebook QnA_using_T5_working.ipynb
   ```
2. Replace the `video_url` variable with a valid YouTube video URL.
3. Modify the `question` variable with your query.
4. Run all cells to fetch the transcript, retrieve context, and generate answers.

## Results
- The system retrieves concise answers from YouTube video transcripts.
- Provides relevant context using BM25 scoring.

## Future Improvements
- Incorporate multilingual support for non-English transcripts.
- Optimize the system for longer transcripts with advanced summarization techniques.
- Develop a user-friendly web interface for ease of access.

## Acknowledgments
- Hugging Face for the T5 model and Transformers library.
- NLTK and rank_bm25 for text processing and retrieval.
- YouTube Transcript API for enabling seamless transcript extraction.
