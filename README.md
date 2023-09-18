# AI-ML-Capital-Placement-Task
# Objective: Build a PDF extractor to pull relevant details from CVs in PDF format, and match them against the job descriptions from the Hugging Face dataset.

# Approach 1:
Step1:
Import Libraries: The code begins by importing necessary libraries including pandas, pdfplumber, transformers (for DistilBERT), and scikit-learn for cosine similarity calculations.

Step2:
Define Paths: It defines paths to the job descriptions PDF file (job_descriptions_pdf_path) and the folder containing candidate resumes in PDF format (pdf_folder).

Step3:
PDF Text Extraction Function: A function extract_text_from_pdf is defined to extract text from a PDF file using pdfplumber.

Step 4:
Initialize DistilBERT: DistilBERT tokenizer and model are initialized using Hugging Face's transformers library.

Step5:
Extract Job Descriptions Text: Text is extracted from the job descriptions PDF using the defined function and tokenized and preprocessed for embedding.

Step6:
Initialize CV Embeddings List: An empty list (cv_embeddings) is initialized to store candidate resume embeddings.

Step7:
Iterate Through Candidate Resumes: The code iterates through PDF files in the specified folder, extracts text from each candidate's resume, tokenizes and preprocesses the text, and computes embeddings.

Step8:
Cosine Similarity Calculation: Cosine similarity is calculated between each candidate's resume and the job descriptions to determine how closely each candidate's resume matches the job descriptions.

Step9:
Display Matching Scores: Finally, the code displays the matching scores for each candidate's resume, indicating the similarity between each resume and the job descriptions.
