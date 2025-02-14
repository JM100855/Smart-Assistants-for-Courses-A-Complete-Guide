# Smart-Assistants-for-Courses-A-Complete-Guide

This project fine-tunes the mistral model with data related to the ESE 577 graduate course. Our method involves tailoring an advanced PDF data extractor called MinerU, which utilises layout detection followed by an OCR, and all of this is wrapped in a deep learning algorithm, allowing us to output hierarchical data, classify images and
accurately extract latex equations, which are essential for our use case. After extraction, the parameters are assigned to their corresponding section, and the Gemini Flask 1.5 API is used to create question-and-answer pairs using multiple prompting techniques. The question-answer pairs are then used to train the mistral model using LoRA for fine tuning. The results, based on extensive experimental observations, show better answers than the general mistral model on deep learning questions with more contextual, in-depth understanding and relevance to the topic. In addition, the fine-tuned model excels at addressing course-specific queries, offering deeper insights and more comprehensive answers. This pipeline highlights the potential for enhancing the model’s overall performance for any course data irrespective of the domain, providing users an end to end pipeline to create chat-bots on any PDFs.
