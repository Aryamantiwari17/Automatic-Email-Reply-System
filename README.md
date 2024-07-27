# Automatic Email Reply System for Film Equipment Rentals

## Overview

This project implements an automatic email reply system for a film equipment rental service. It uses natural language processing and machine learning techniques to classify incoming emails, provide relevant responses, and handle customer inquiries efficiently.

## Features

- Email classification into categories: positive reviews, negative reviews, and general inquiries
- Automated responses for positive and negative reviews
- FAQ-based responses for general inquiries using a Retrieval-Augmented Generation (RAG) pipeline
- Integration with a SQL database for equipment inventory management
- Use of the Groq language model for natural language generation

## Technology Stack

- Python 3.8+
- SQLAlchemy for database ORM
- Groq API for natural language processing
- scikit-learn for TF-IDF vectorization and cosine similarity
- SQLite for the database

## Installation

1. Clone the repository:
git clone https://github.com/Aryamantiwari17/Automatic-Email-Reply-System
cd film-equipment-rental-email-system

2. Create a virtual environment and activate it:
python -m venv venv
source venv/bin/activate
# On Windows, use venv\Scripts\activate

4. Install the required packages:
pip install -r requirements.txt

5. Set up your environment variables:
Create a `.env` file in the project root and add your Groq API key:
GROQ_API_KEY=your_api_key_here

## Usage

Run the main script to process sample emails:
python main.py

This will demonstrate the system's ability to classify emails and generate appropriate responses.

## Project Structure

- `main.py`: The main script that ties everything together
- `database_schema.md`: Documentation of the database schema
- `rag_pipeline.md`: Documentation of the RAG pipeline
- `email_handling_flowchart.md`: A flowchart of the email handling process

## Database Schema

The project uses a simple SQLite database to store equipment information. See `database_schema.md` for details.

## RAG Pipeline

The Retrieval-Augmented Generation pipeline is used to handle general inquiries. It combines TF-IDF based retrieval with the Groq language model for generation. See `rag_pipeline.md` for more information.

## Email Handling Process

The system follows a specific flow to handle incoming emails. Refer to `email_handling_flowchart.md` for a visual representation of this process.


## Contributing

Contributions to this project are welcome! Please fork the repository and submit a pull request with your changes.

## Acknowledgments

- Groq for providing the language model API
- The scikit-learn team for their machine learning tools
- The SQLAlchemy team for their ORM library

##Flowchart
![Flowchart](https://github.com/user-attachments/assets/9c6f4d06-0d7f-493f-b4a1-253d56b53622)
##Output
![image](https://github.com/user-attachments/assets/e3b1a3d1-2d7d-46bf-8d53-75a1e8feb710)
![image](https://github.com/user-attachments/assets/1587fcd9-1c33-496a-94ae-7c2e2bca6998)
![image](https://github.com/user-attachments/assets/fff12dd9-d49e-40e7-a087-d4227cf19c68)
![image](https://github.com/user-attachments/assets/9cfa5de2-311c-4004-a86d-cca9a86264c0)





