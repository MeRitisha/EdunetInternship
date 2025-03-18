# AI-Powered Resume Screening and Ranking System

An AI-powered system to automate resume screening and ranking using Natural Language Processing (NLP) and Machine Learning (ML). This system helps recruiters efficiently filter and rank resumes based on job descriptions and company requirements.

---

## Table of Contents
1. Features
2. Technologies Used
3. Installation
4. Usage
5. How It Works
6. Future Enhancements
7. Contributing
8. License

---

## Features
Resume Parsing: Extracts key details from resumes (PDF/DOCX).
Job Description Matching: Matches resumes with job descriptions using BERT embeddings.
Ranking: Ranks candidates based on relevance to the job description.
Real-Time Feedback: Provides actionable feedback for resume improvement.
Multilingual Support: Handles resumes and job descriptions in multiple languages.
Bias Mitigation: Ensures fair and unbiased candidate evaluations.

---

## Technologies Used
Python: Primary programming language.
spaCy: For text preprocessing and NLP tasks.
BERT: For advanced contextual understanding of resumes and job descriptions.
scikit-learn: For cosine similarity calculations.
PyPDF2 and python-docx: For extracting text from PDF and DOCX files.
Streamlit: For building a user-friendly web interface.

---

## Installation

### Prerequisites
Python 3.8 or higher
pip (Python package manager)

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/resume-screening-system.git
   cd resume-screening-system
   ```

2. Install the required libraries:
   ```bash
   pip install -r requirements.txt
   ```

3. Download the spaCy English language model:
   ```bash
   python -m spacy download en_core_web_sm
   ```

---

## Usage

### Running the System
1. Start the Streamlit app:
   ```bash
   streamlit run app.py
   ```

2. Open the provided URL in your browser (e.g., `http://localhost:8501`).

3. Upload your resume (PDF or DOCX) and input the job description.

4. The system will:
   Parse your resume.
   Compare it with the job description.
   Provide a similarity score and feedback.

---

## How It Works

### Workflow
1. Resume Upload: Users upload their resumes in PDF or DOCX format.
2. Text Extraction: The system extracts text from the resume.
3. Preprocessing: The text is cleaned and tokenized using spaCy.
4. BERT Embeddings: BERT generates embeddings for the resume and job description.
5. Cosine Similarity: The system calculates the similarity between the resume and job description.
6. Ranking & Feedback: Resumes are ranked, and feedback is provided for improvement.

### Example
```python
# Sample Resume
resume_text = """
Experienced software engineer with 5 years of experience in Python and machine learning.
Proficient in TensorFlow, PyTorch, and AWS. Strong problem-solving skills and a passion for AI.
"""

# Sample Job Description
job_description = """
We are looking for a Software Engineer with experience in Python and machine learning.
The ideal candidate should have hands-on experience with TensorFlow, PyTorch, and cloud platforms like AWS.
Strong problem-solving skills and a passion for AI are a plus.
"""

# Compare resume with job description
similarity, feedback = compare_resume_with_job_description(resume_text, job_description)
print(f"Similarity Score: {similarity:.4f}")
for item in feedback:
    print(item)
```

---

## Future Enhancements
Multilingual Support: Add support for multiple languages using multilingual models.
Bias Mitigation: Implement fairness-aware algorithms to reduce bias.
Integration with ATS: Integrate with Applicant Tracking Systems (ATS) for seamless hiring processes.
Real-Time Feedback: Provide real-time feedback for resume improvement.
Industry-Specific Customization: Tailor the system for specific industries (e.g., healthcare, finance, marketing).

---

## Contributing
Contributions are welcome! If you'd like to contribute, please follow these steps:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeatureName`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature/YourFeatureName`).
5. Open a pull request.

---

## License
This project is licensed under the MIT License. See the LICENSE file for details.

---

## Contact
For any questions or feedback, please contact:
Your Name  
Email: ritisha251@gmail.com  
GitHub: [your-username](https://github.com/MeRitisha)  
LinkedIn: [Your LinkedIn Profile](https://www.linkedin.com/in/ritisha-duggempudi-351042257/)


