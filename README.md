# AI-ML-Capital-Placement-Task
# Objective: Build a PDF extractor to pull relevant details from CVs in PDF format, and match them against the job descriptions from the Hugging Face dataset.

# Approach 1: As mentioned in task description
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

Result:
![cpimage](https://github.com/Abhijeetgaurav/AI-ML-Capital-Placement-Task/assets/83373398/38fd128c-3345-422a-a452-83d59c21b44f)


# Approach 2:  Using Scripts and structuring
Step1:
Data Preparation: The code loads job descriptions from a CSV file and sets up a PDF document to store the job descriptions.

Step2:
PDF Creation: It generates a PDF document using the FPDF library and populates it with job titles and descriptions from the CSV.

Step3:
Resume and Job Descriptions Paths: It defines paths for a candidate's resume (CV) and the job descriptions PDF.

Step4:
Text Extraction from CV: Using pdfplumber and PyPDF2, the code extracts text from both the CV and job descriptions PDF files, cleaning and formatting the text.

Step5:
Text Similarity Calculation: It calculates the cosine similarity between the extracted CV text and job descriptions text to measure the match.

Step6:
Cosine Similarity Output: The code prints the similarity score, indicating how closely the CV matches the job descriptions.

Step7:
Data Output: It provides a brief summary of the code's functionality, which involves PDF generation, text extraction, and similarity computation for CVs against job descriptions.

Result:

![cpimage2](https://github.com/Abhijeetgaurav/AI-ML-Capital-Placement-Task/assets/83373398/e3b4118f-94a7-4847-b590-419f4e6a2c24)


