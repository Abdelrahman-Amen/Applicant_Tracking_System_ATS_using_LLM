# 🌟 ATS Resume Expert Using Google Generative AI 🌟

Welcome to the ATS Resume Expert app! This Streamlit application helps you evaluate resumes against job descriptions using advanced Google Generative AI (Gemini), making it easier to identify how well a resume matches a specific role.

![Image](https://github.com/user-attachments/assets/4ff62b45-50d6-43f8-8fb2-be70ad32dfcc)

# What is an ATS (Applicant Tracking System)? 💼


An Applicant Tracking System (ATS) is a software application used by companies to manage the recruitment process. It automates the hiring workflow by:

• Screening resumes: The ATS scans resumes for relevant keywords, qualifications, and experiences that match the job description.

• Organizing candidate information: It sorts and stores resumes for easy access by recruiters.

• Enhancing recruitment efficiency: ATS systems help hiring managers filter out unqualified candidates quickly and streamline the selection process.

In essence, an ATS serves as a gatekeeper, ensuring only the most qualified candidates make it through to human review.


# How We Create an ATS Using LLM (Large Language Models) 🤖


### 1. Integrating Large Language Models (LLMs):

• LLMs like Google Gemini allow us to evaluate resumes in a more human-like manner by analyzing the content in-depth.

• They can understand context, intent, and sentiment, making the process of matching resumes with job descriptions more accurate than traditional keyword-based methods.

### 2. Input Analysis:

• We ask the LLM to analyze both the job description and the resume.

• The system evaluates key skills, experiences, qualifications, and other relevant attributes present in the job description and matches them with the candidate's resume.



### 3. Generating Meaningful Output:

• The LLM generates two types of outputs:

• A detailed analysis: Describing how well the resume fits the job, including strengths and areas for improvement.

• A percentage match score: Giving an overall compatibility score between the resume and the job description based on the keyword match and overall relevance.



## Streamlit App Breakdown 🧑‍💼 : 

### Job Description Input 📝

• Text Area: The user can input a job description that specifies the role's requirements. This will be compared with the uploaded resume.

### Resume Upload 📄

• File Uploader: The user uploads their resume in PDF format, and the app extracts the content to analyze it.

### Buttons for Actions 🔘

• "Tell Me About the Resume": This button triggers an analysis of how well the resume matches the job description, focusing on strengths and areas for improvement.

• "Percentage Match": This button calculates the percentage of compatibility between the resume and the job description.


### Key Features:

• Generative AI Integration: The app uses Google Gemini’s generative AI to process and evaluate the input text (both resume and job description).

• Text Extraction from PDF: The PyPDF2 library is used to extract the text from the uploaded PDF resume, making it ready for analysis.

• Environment Configuration: The app uses environment variables (loaded from .env) to securely store the API key for Google Generative AI.




# How It Works 🚀:

### 1.Resume and Job Description Processing:

• The user uploads their resume and provides the job description.

• The app uses a PDF extractor to grab the text from the resume and then formats it for AI evaluation.

### 2.Prompt Creation:

• The LLM generates responses based on two main prompts:

• Tell Me About the Resume: Provides a detailed analysis of how well the resume fits the job description.

• Percentage Match: Calculates a compatibility score to determine how closely the resume aligns with the job description.

### 3.Result Display:

• After processing, the app displays the AI-generated results on the interface, offering a detailed evaluation and percentage score.


# Technologies Used 🛠️:

• Streamlit: For building the interactive front-end of the app.

• Google Generative AI (Gemini): For advanced natural language processing to generate human-like analysis and scores.

• PyPDF2: For extracting text from PDF resumes.

• dotenv: For securely loading the API key from an environment file.
