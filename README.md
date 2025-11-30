Problem Statement :
    We all deal with long, detailed documents—assignments, research papers, technical articles, reports, and more.Reading everything fully is time-consuming and often overwhelming. People struggle with:
    Spending too much time understanding lengthy text
    Getting lost in details instead of key points
    Difficulty processing multiple documents quickly
    General information overload
A Document Summarizer solves this by automatically pulling out the core ideas from any text.
This makes reading faster and helps students, teachers, professionals, and researchers focus on what actually matters.
Services & Tools Used :
    1.Amazon Bedrock
    2.Streamlit
    3.Python
Architecture Overview :
    The design is intentionally simple:
    User pastes text into the Streamlit textbox
    Streamlit sends the text to the backend function
    The text is passed to the Amazon Bedrock model
    Bedrock generates a summarized version
    The summarized output is displayed on the page instantly
With no file handling involved, the workflow is fast, clean, and reliable.
Technical Implementation :
    1.Initializing a Bedrock client using Initializing a Bedrock client using boto3
    2.Creating a Streamlit textbox for user input
    3.Passing the text prompt to the model
    4.Receiving and displaying the summary
    5.Adding simple checks to avoid empty input errors boto3.
Future Improvements :
    Deploy the backend using AWS Lambda
    Add API Gateway for external access
    Store summaries in S3
    Add DynamoDB for user history
    Allow model selection inside the UI
    Introduce multi-language summarization
    Allow the user to upload files
    Deploy the backend using AWS Lambda
Code & Resources :
    Code is available in the following github repo :
    https://github.com/Srimathi109/Content-Summarization-Amazon-Bedrock
Conclusion :
     <img width="1681" height="873" alt="Screenshot 2025-11-30 130711" src="https://github.com/user-attachments/assets/91809bbf-ca68-49bc-b058-2ce58ad3eb0e" />
Building a Document Summarizer for Workshop 1 of the AI for Bharat Challenge gave me hands-on experience with Amazon Bedrock and Streamlit.This workshop has motivated me to explore more advanced features and expand this into a more polished, powerful tool in the upcoming challenge weeks.
