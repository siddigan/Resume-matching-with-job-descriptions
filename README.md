
README


This repository contains code for a resume matching system using Bert LM. The system works by first extracting the text from the resume PDF file and then preprocessing the text. The preprocessed text is then used to generate embeddings. The embeddings for the resume are then compared to the embeddings for the job description using cosine similarity. The resumes with the highest cosine similarity are then returned as the top matches.



Instructions

To use the code, follow these steps:


Install the required dependencies:
pip install pandas pypdf nltk transformers torch sklearn numpy
Download the resume dataset from Kaggle:
kaggle competitions download -c resume-dataset
Extract the resume dataset:
unzip resume-dataset.zip
Run the following command to train the model:
python main.py
Once the model is trained, you can use it to match resumes to job descriptions by running the following command:
python main.py --test
This will generate a CSV file called result.csv containing the top 5 resume matches for each job description.



Usage


To use the resume matching system, simply provide it with a job description and a set of resumes. The system will then return the top 5 resume matches for the job description.


The system can be used in a variety of applications, such as:


Recruitment: Recruiters can use the system to find the best candidates for open positions.
Job search: Job seekers can use the system to find jobs that are a good match for their skills and experience.
Career counseling: Career counselors can use the system to help their clients find jobs that are a good fit for their interests and goals.
