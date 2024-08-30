# RAG Document Q&A with Groq and Llama3

This project demonstrates a Retrieval-Augmented Generation (RAG) system using Groq's Llama3 model for question answering based on research papers. The application allows users to input queries related to research papers and provides context-based answers using embedded documents.

### Project structure 

project-directory/
│
├── app.py
├── requirements.txt
├── .env
├── README.md
├── LICENSE
├── .gitignore
└── Screenshot_2024-08-28_224139.png

## Features
- **Document Embedding**: Embeds and stores document vectors for fast retrieval.
- **Query Answering**: Uses Llama3 to generate answers from the provided research paper context.
- **Document Similarity Search**: Displays similar document chunks related to the query.

## Setup

### Prerequisites
- Python 3.8 or higher
- Groq API Key
- OpenAI API Key

### Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/your-username/project-directory.git
    cd project-directory
    ```

2. Install the required packages:

    ```bash
    pip install -r requirements.txt
    ```

3. Create a `.env` file with your API keys:

    ```bash
    GROQ_API_KEY=your_groq_api_key
    OPENAI_API_KEY=your_openai_api_key
    ```

4. Place your research papers in a directory named `research_paper` in the root of the project.

5. Run the application:

    ```bash
    streamlit run app.py
    ```

6. Access the application at `http://localhost:8501`.

## Usage

- Enter your query related to the research paper in the input box.
- Click on **Document Embedding** to create the vector database if not already done.
- The application will return the response along with the response time.
- Use the **Document similarity search** expander to view related document sections.

## Screenshot

![Screenshot](Screenshot_2024-08-28_224139.png)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

