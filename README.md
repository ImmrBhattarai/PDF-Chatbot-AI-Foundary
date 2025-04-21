# PDF-Chatbot-AI-Foundary | DIO Project
A chat bot to talk to your multiple PDFs (vectorized via text embedding models) at once; provides grounded answers to your queries to the GPT-4o powered bot

Read my detailed article to see how you can do this as well: [Medium Article](https://immrbhattarai.medium.com/make-your-own-ai-powered-pdf-chatbot-1bf661fc5ecb)

## Challenge Completed in Azure Foundry Hub

### What I did:
1. Created an Azure Foundry Project (Via Azure portal)

2. Created a Hub for the project

![image](https://github.com/user-attachments/assets/c0cfd16e-84b8-4bfb-ad50-420200da90bd)
![image](https://github.com/user-attachments/assets/ea6b80f6-1aca-4de1-905d-574944f201d0)

3. Model + Endpoints | Manage Deployments of your Models and services

![image](https://github.com/user-attachments/assets/df7335fa-0bae-40ab-9c98-e3be9efb0a98)

   3.1. Created a chat completion model **(GPT-4o)**
   
   ![image](https://github.com/user-attachments/assets/5e389892-6539-4ac6-bb4a-4c581f35f214)
   ![image](https://github.com/user-attachments/assets/c9c1e3d5-9eb0-4c21-aa85-f275313e42ce)
   ![image](https://github.com/user-attachments/assets/49ab1a09-98ed-4a18-ad43-623db9e6b8d4)


   3.2. Created a text embedding model **(text-embedding-3-large)**
   
   ![image](https://github.com/user-attachments/assets/1b49d73f-8833-4b14-8a43-fcec181446fa)
   ![image](https://github.com/user-attachments/assets/1a4972ba-fee0-4898-944d-e030fa77f67c)

After completing both 3.1 and 3,2, you will see something like this:

![image](https://github.com/user-attachments/assets/d9024574-366d-4846-939f-34e4bfbd1fb6)

4. Set the tone of the chatbot to define my use cases. Set the system instruction.
   
**"You indentiy yourself as a visa counselor for the USA Visa related queries, either for pre-processing or post-processing stages. You only help with visa for the USA and particularly for Student Visa, nothing more. In case someone asks you anything beyond, silently deny that. You go above and beyond only to offer help in your subject as a Visa Counselor."**
   
![image](https://github.com/user-attachments/assets/82c75947-9d87-4213-80bf-907895edcd27)
![image](https://github.com/user-attachments/assets/f8f73744-7988-4ba5-8703-540c9fa7c997)

   
5. Add Data Sources and configure them

![image](https://github.com/user-attachments/assets/b49e6cbd-3976-4a3e-b769-546671ac6b3f)
![image](https://github.com/user-attachments/assets/089f0d92-5c2b-42b4-bf32-b829fdba6592)
![image](https://github.com/user-attachments/assets/2274d4ea-23d4-4ae4-b53c-11c46f882cb5)
![image](https://github.com/user-attachments/assets/eb81f3ee-af4a-4a4c-8bf5-9d756078031e)

Instead of scientic paper research, I opted for visa guide. I collected public PDFs from the internet for this purpose.

   5.1 Select Appropriate VM size
   
   ![image](https://github.com/user-attachments/assets/0541dc56-c7b8-4bf3-94b9-c3837fda032c)

   5.2 Ingestion steps
   
   ![image](https://github.com/user-attachments/assets/7c96aa26-1736-4b3b-9bff-d5901d6f60f9)
   ![image](https://github.com/user-attachments/assets/77040863-9422-436e-ad48-54f625c7b902)
   
6. Test the chat playground and observe model responses

![image](https://github.com/user-attachments/assets/5da20c8e-c313-4389-a500-ad6b74c230bf)
![image](https://github.com/user-attachments/assets/5c6973dc-d472-42fb-9f65-226f9276d9c4)
![image](https://github.com/user-attachments/assets/76ccb8af-39d7-4c23-a722-682cc149e02b)
![image](https://github.com/user-attachments/assets/47998568-250d-4c64-bf1f-4087131d5c4f)

7. Deploy your model

![image](https://github.com/user-attachments/assets/97967644-dd0b-4cbb-80e8-fe26a6373743)


8. Utilized Endpoint in localhost

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

## What was my experience with this project?
Trying out the hands-on Azure Foundry for the very first time felt really confusing, but navigating every other settings, section, options, menus, etc made me feel comfortable in no time. The DIO challenge added new confidence in me to try out the new agentic chatbot (still in preview).
