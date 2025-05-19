# Henosia-AIBuddy
Integrating AI into Henosia - A semester project with company collaboration

**This project is part of an 8th semester Interaction Design semester project at Aalborg University**


# About the program:

AIBuddy is a Proof of Concept (POC) created to showcase how AI might play a role in Henosia (a collaborative low-code design tool for hybrid designers) and ease the workflow for their users.
By using a small dataset as guidelines for the GPT4 engine, the user can prompt custom code snippets to get a name, description and code for the snippet. The snippet can then be saved and ideally, inserted into Henosia to showcase.



# Get started:

The code is originally written in Google Colab and uses their secret key feature. To run the code, you must go to the left menu and click on 'secrets' --> 'add new secret' --> Name it 'OPEN_API_KEY' and insert your OpenAI API key (Remember to enable access to the notebook).

This should allow you to run the code.


To finetune the model, you can adjust the following parameters:

GPT4 (Lines 13 - 43):
- System message: Instructions for GPT4
- User message: How it should handle the user prompt
- max_tokens: Max tokens GPT4 can use
- temperature: Adjusts the creativity of GPT4 (lower number = less creativity)

TF-IDF Vectorization & Cosine similarity (Line 87):
- Relevance threshold: Only entries in the dataset with a similarity score above this number is considered relevant

**OBS! Extensive testing showed that current parameters gives the most accurate output**

# Other information:

The custom Snippet Dataset is uploaded to the HuggingFace website and can be found here: https://huggingface.co/datasets/P8IxD/Snippet_dataset_til_test

**You can change the dataset with your own by changing the path in line 7**

# Authors:
Christian Midjord Holfelt & Maja Thestesen
