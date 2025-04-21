# PDF-Chatbot-AI-Foundary | DIO Project
A chat bot to talk to your multiple PDFs (vectorized via text embedding models) at once; provides grounded answers to your queries to the GPT-4o powered bot

Read my detailed article to see how you can do this as well: [Medium Article](https://immrbhattarai.medium.com/make-your-own-ai-powered-pdf-chatbot-1bf661fc5ecb)

## Challenge Completed in Azure Foundry Hub

### What I did:
1. Created an Azure Foundry Project (Via Azure portal)
2. Created a Hub for the project
   ![Screenshot From 2025-04-18 22-38-04](https://github.com/user-attachments/assets/1ae4452f-6a7b-46cc-bf0a-2af5879afd8a)
   ![Screenshot From 2025-04-18 22-46-08](https://github.com/user-attachments/assets/5e2d57e0-fa2f-4e3f-9e78-a42ef98ef898)
   But I utilized a custom compute instance to reduce cloud cost/bill (thus have to install some libraries later)
   
4. Model + Endpoints | Manage Deployments of your Models and services
   
   3.1. Created a chat completion model **(GPT-4o)**
   
   ![Screenshot From 2025-04-18 22-32-58](https://github.com/user-attachments/assets/aba2a108-18fa-44e3-af84-e90a0bd1e721)
   
   3.2. Created a text embedding model **(text-embedding-3-large)**
   
   ![Screenshot From 2025-04-18 22-33-15](https://github.com/user-attachments/assets/5ed92d2b-bca1-40d3-b196-5adcb8b4daf3)
   
5. Set the tone of the chatbot to define my use cases. Set the system instruction.
   
   **"You indentiy yourself as a visa counselor for the USA Visa related queries, either for pre-processing or post-processing stages. You only help with visa for the USA and particularly for Student Visa, nothing more. In case someone asks you anything beyond, silently deny that. You go above and beyond only to offer help in your subject as a Visa Counselor."**
   
   ![Screenshot From 2025-04-18 23-04-31](https://github.com/user-attachments/assets/e292fe8d-c232-4912-9c52-805b9155b6ed)
   
7. Add Data Sources and configure them
   ![Screenshot From 2025-04-18 23-20-25](https://github.com/user-attachments/assets/0af81ec7-f073-478c-84a5-77236efcbcd7)
   ![Screenshot From 2025-04-18 23-21-35](https://github.com/user-attachments/assets/217c2433-04c9-4000-a2a1-8fca20babe1d)
   ![Screenshot From 2025-04-18 23-22-31](https://github.com/user-attachments/assets/5d5cb035-4b40-4b4e-8dd0-503d69038522)

   7.1 Select Appropriate VM size
   
   7.2 Ingestion steps
   
9. Test the chat playground and observe model responses
   ![Screenshot From 2025-04-18 23-23-19](https://github.com/user-attachments/assets/a915ac0b-3d50-48ba-b0ae-b9d2ff0e1ec6)
   ![Screenshot From 2025-04-18 23-23-47](https://github.com/user-attachments/assets/bbf1c976-f9f4-4042-88d9-fd848fffb35a)
    
10. Deploy your model
![Screenshot From 2025-04-18 23-24-11](https://github.com/user-attachments/assets/34a72699-3b01-4604-be3b-1e07e3dc7568)
![Screenshot From 2025-04-18 23-24-36](https://github.com/user-attachments/assets/3ecdab3d-249f-43bd-875b-deb0c4540e49)

11. Utilized Endpoint in localhost
![Screenshot From 2025-04-18 23-24-52](https://github.com/user-attachments/assets/928d9fb6-2945-4cc4-ad9e-877d620cb395)

---
# What I did in this project (Summary)
- Upload PDF files containing information relevant to your study or project.
- Implement a vector search system to index and retrieve information from PDFs.
- Use artificial intelligence to generate responses based on the content of uploaded documents.
- Develop an interactive chat where it is possible to ask questions and get contextual answers based on the files.

# What I learned in this project (Summary)
- What is Azure Foundry Hub
- Model Catalog and various models to explore
- Creating chat models and embedding models
- Loading Data Sources and content filter
- Creating Azure AI Search and Foundry resources
- Model Parameters and ways to deploy model
- Using system instructions to narrow down the scope of chatbot
- Insights on other available Azure OpenAI services
- Indexing, semantic search and model groundness
- Deploying chatbot endpoints
- Using endpoints in local host for a live chat environnment andexperience.
