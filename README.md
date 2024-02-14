# Resume-Ranking-System

## Objective

The system's objective is to automate the initial screening of resumes by extracting key information such as experience, skills, education, and certifications, then ranking the candidates based on their relevance to a given job description. The system's design is highly flexible, accommodating resumes in various formats (PDF, DOCX, etc.) and leveraging Python proficiency and Natural Language Processing (NLP) expertise.

## Architecture

The system's architecture consists of three main components: the Resume Parser, the Job Description Matcher, and the Ranking Module.

1. **Resume Parser**: This component utilizes NLP techniques to extract information from resumes. It processes resumes in different formats and extracts relevant data such as work experience, education, skills, and certifications. This data is then preprocessed to normalize the text, remove stopwords, and identify relevant keywords.
2. **Job Description Matcher**: This component compares the information extracted from resumes against a given job description. It utilizes algorithms such as cosine similarity or TF-IDF to calculate the similarity between the job description and each resume. The matcher then generates a relevance score for each candidate based on the matching keywords and skills.
3. **Ranking Module**: The ranking module receives the relevance scores from the job description matcher and ranks the resumes based on their scores. The ranking can be based on a simple sorting mechanism or more complex algorithms, considering additional factors like years of experience, education level, or certifications.

## Functionality and Input

1. **Parsing Resumes**: The system can accept resumes in various formats, including PDF, DOCX, and text. It uses appropriate libraries (such as **`pdfminer`** for PDFs or **`python-docx`** for DOCX) to extract text and then uses NLP techniques to identify and extract relevant information.
2. **Matching Job Descriptions**: The system provides an interface for users to input job descriptions. The description is then parsed and matched against the information extracted from resumes.
3. **Ranking Candidates**: Based on the relevance scores, the system ranks the candidates and presents the results in a user-friendly format, making it easy for recruiters to identify suitable candidates.

## Evaluation

The system was evaluated using a dataset of resumes and job descriptions. The accuracy and efficiency of the system were measured based on the match scores generated for each resume. The system's performance was compared against a manual screening process to assess its effectiveness in automating the resume screening process.

## Prerequisite Requirements

```python
pip install pdfminer3
pip install pyresparser
pip install streamlit
pip install pandas
pip install plotly
pip install pymysql
pip install streamlit-tags
pip install Pillow
```

## Output

In the resume parser and ranking system, the output is in the form of tables, which are generated after parsing the resumes and comparing them to the job description. The tables provide a summary of the key information extracted from each resume and rank the candidates based on their relevance to the job description.
