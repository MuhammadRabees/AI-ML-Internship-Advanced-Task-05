# Auto-Tagging Support Tickets Using LLM

## Objective of the Task
The goal of this project is to automate the categorization of customer support tickets using Generative AI. By leveraging a Large Language Model (LLM), the system aims to reduce manual routing efforts and improve response times. This project is part of the AI/ML Engineering Advanced Internship at DevelopersHub Corporation.

## Methodology / Approach
This project utilizes prompt engineering and the Gemini 2.5 Flash model via the `google-generativeai` SDK:
* **Prompt Engineering:** Designed a structured prompt instructing the LLM to act as an expert customer support AI.
* **Few-Shot Learning:** Implemented few-shot learning by providing the model with carefully curated examples of support tickets and their ideal multi-tag outputs. This significantly improved the model's accuracy and format consistency compared to a zero-shot approach.
* **Security:** API keys were securely managed and hidden using environment secrets to prevent unauthorized access.

## Key Results or Observations
* **Multi-Class Prediction:** The system successfully processes raw, unstructured ticket text and accurately outputs the top 3 most probable tags per ticket.
* **Contextual Understanding:** The LLM demonstrated advanced reasoning by correctly inferring underlying intents (e.g., tagging a request for "dark mode" as a "Feature Request" and "UI/UX" issue without those exact words being present in the input).
* **Efficiency:** The system processes these requests with high accuracy and low latency, proving its viability for integration into a live customer support pipeline.
