# AutoDraft: AI-Powered Email Reply Automation

## 🧠 Purpose
Automate the generation of email drafts in response to inbound messages, leveraging:
- OpenAI's GPT-4.2 API for natural language understanding and generation
- Google Sheets as a dynamic template database
- Make.com as the workflow automation platform

## ⚙️ System Architecture
<img width="1182" alt="image" src="https://github.com/user-attachments/assets/c15153bb-a5f0-4db4-a54a-9bdd45ab0087" />

### 🔄 Steps:

1. **Trigger (Email Module)**
   - Watches for new inbound emails via Gmail/Outlook integration.

2. **LLM Analysis (OpenAI GPT-4.2)**
   - Reads and parses email content.
   - Extracts context, intent, and entities.

3. **Template Lookup (Google Sheets)**
   - Searches for the best-matching response template based on email type or keywords.
   - Returns structured template + variables.

4. **Draft Generation (OpenAI GPT-4.2)**
   - Injects extracted context into the prompt template.
   - Returns a personalized email response.

5. **Email Drafting (Email Module)**
   - Populates the draft in Gmail or Outlook.
   - Draft can be reviewed/edited by a human before sending.
  
## 🧰 Tech Stack
- **Make.com** – Orchestrator for the entire flow
- **OpenAI GPT-4.2 API** – Natural Language Understanding & Generation
- **Google Sheets** – Lightweight template management
- **Gmail/Outlook** – Email client integration

## 📈 Impact
- ⚡ Reduced average email response drafting time by 90%
- 📬 Increased lead engagement by responding faster and more consistently
- 🔄 Enabled sales pods to focus on conversion, not manual replies

## 🧩 Future Improvements
- Add CRM syncing (e.g., CDK, VinSolutions)
- A/B testing engine for response variants
- Add fallback logic for missing template scenarios

## ▶️ Video Demonstration 
- Link: 
