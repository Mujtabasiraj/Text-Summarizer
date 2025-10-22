TEXT-SUMMARIZATION-TOOL

COMPANY: CODTECH IT SOLUTIONS

NAME: Syed Mujtaba Siraj Uddin

NCS ID: E19E86-0116588288923

DOMAIN: Artificial Intelligence

DURATION: 4 WEEKS

MENTOR: Vaishali

DESCRIPTION

This task focuses on building an intelligent tool that can automatically summarize lengthy PDF documents into concise, meaningful summaries. The goal is to help readers grasp the essence of large reports, research papers, or articles quickly—without having to read every line. In essence, it bridges the gap between overwhelming information and accessible understanding.

The project leverages the Transformers library from Hugging Face, specifically using the DistilBART model (sshleifer/distilbart-cnn-12-6). This model is a pre-trained neural network designed for text summarization tasks. It uses advanced natural language processing (NLP) techniques to understand large portions of text and generate clear, human-like summaries. By doing so, the system ensures that the summarized content retains the original context and intent.

The workflow begins when a user uploads a PDF document into the application. To process the document, the system utilizes LangChain’s PyPDFLoader, which extracts textual data from each page of the uploaded file. The extracted text is then cleaned and divided into smaller chunks to ensure smooth processing, as models often have input length limitations. This chunking also allows the summarizer to handle documents of varying sizes more efficiently.

For each chunk of text, an adaptive summarization process takes place. Instead of using fixed-length summaries, the system dynamically adjusts the summary length based on the content’s word count. This means shorter sections receive briefer summaries, while longer ones get more detailed outputs. The summarizer applies a compression ratio (for example, summarizing to 50% of the original chunk length) to control how much information is condensed at each step. This adaptability makes the tool versatile, capable of working with everything from brief memos to dense research papers.

After summarizing individual sections, the tool merges all summaries into one combined text. A second round of summarization is then performed on this combined text—compressing it further while maintaining coherence and meaning. The result is a final, polished summary that captures the essence of the entire document in a readable, well-structured form.

To make this system user-friendly, the project integrates Gradio, a Python library that allows developers to create interactive web interfaces easily. The interface consists of simple components: a file upload box for the PDF, a button labeled “Summarize,” and two output sections—one displaying the extracted original text and the other showing the generated summary. Once the user clicks the button, the summarization pipeline runs automatically and displays the results directly on the web page. Gradio’s interface also supports GPU acceleration, ensuring faster processing for large files.

Overall, this task demonstrates how deep learning and NLP can work together to transform the way we interact with information. By automating the process of summarizing lengthy documents, this tool saves time, reduces cognitive load, and enhances productivity—making it a valuable assistan[Uploading Task-1.ipynb…]()
t for students, researchers, and professionals alike.

OUTPUT
<img width="1280" height="724" alt="501523772-ec87d631-9919-4aac-ad5d-ba6bd9fd78f9" src="https://github.com/user-attachments/assets/68ec3541-3631-4750-bf9e-0fd3dfe1c9f4" />

