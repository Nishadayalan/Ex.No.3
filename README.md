# Ex.No.3  To design an AI-powered chatbot that assists customers in resolving issues related to product troubleshooting, order tracking, and general inquiries. The chatbot should handle various customer queries efficiently while maintaining a conversational and user-friendly tone. 
Using Straightforward Prompts - Tabular Format Prompting - Missing Word Prompting - Preceding Question Prompting techniques.

### DATE: 03-08-2026                                                                            
### REGISTER NUMBER : 212223230143 
# Aim: 
To write the prompts for these following prompt types and evaluate that using any one method 1. Straightforward Prompts, 2. Tabular Format Prompting 3.Preceding Question Prompting and 4. Missing Word Prompting

# Explanation - Any one use case from Unit 5 and generate the report for that with the unit 2 Prompt type
Procedure:
1.	Straightforward Prompts:
    - •	"Define photosynthesis in one sentence."
    - 	"List three advantages of electric vehicles."

 3.	Tabular Format Prompting:
     •	"Compare and contrast AC and DC current in a table."
     •	"Provide a table listing five programming languages, their paradigms, and one use case each."
3. Preceding Question Prompting:
    •	"Why is climate change a global concern? Explain how greenhouse gases contribute to global warming."
    •	"How do vaccines work? Describe the process of immunization in simple terms."
4. Missing Word Prompting:
   •	"The capital of France is ____."
  •	"In photosynthesis, plants absorb sunlight to produce ____."

## Use Case: Renewable Energy & Electric Mobility
(Selected Domain: Sustainable Technology)

# Prompt 
## 1. Straightforward Prompting
Concept
Direct instruction that explicitly defines the role, task, constraints, and tone without complex formatting or step-by-step pre-thinking.

Designed Prompt
Role: You are a helpful customer support AI for an e-commerce platform.

Task: Assist users with product troubleshooting, order tracking, and general policy inquiries.

Tone: Conversational, professional, and empathetic.

Instructions:

Keep responses clear and under 3 sentences unless complex troubleshooting is needed.

If an order number is missing for tracking, ask for it politely.

If a product issue requires a return, provide the link to our returns portal.

User Input: "My order hasn't arrived yet, and it was supposed to get here yesterday. Can you help?"
_____________________________________________________________________________________________________

## 2. Tabular Format Prompting
Concept
Utilizing structured markdown tables within the system prompt to establish standard operating procedures (SOPs), intent-mapping rules, and strict output guidelines.

You are a customer support AI assistant. Handle user inquiries according to the table below. Match the user's intent to the corresponding action and tone:

| Intent Category | Example Trigger Words | Required Information | Target Response Tone |
| :--- | :--- | :--- | :--- |
| Order Tracking | where is my package, delayed, shipping status, track order | Order ID, Tracking Number | Reassuring, efficient |
| Troubleshooting | broken, not working, error code, setup issue | Device model, specific symptom | Patient, step-by-step |
| General Inquiries | refund policy, store hours, shipping costs | Specific query topic | Direct, informative |

Output Format Constraint: Present the response to the user along with a structured summary table of the action taken for internal logging:
1. Customer Response
2. Summary Table (Intent, Resolution Status, Next Steps)

User Input: "My screen is flickering on my TechPad Pro after the update."

____________________________________________________________________
## 3. Missing Word Prompting (Completion / Fill-in-the-Blank)
Concept
Framing system instructions as a completion task with placeholders ([_____]). This forces the LLM to structure its internal reasoning and extract key entities before producing the final response.

Complete the missing fields [_____] based on the customer prompt below, then output the final response.

System Template:  
- Identified Intent: [_____]  
- Customer Emotion: [_____]  
- Missing Details Needed: [_____]  
- Core Troubleshooting Strategy: [_____]  

Final Response: Write a friendly, 2-sentence reply addressing the customer using the filled-in details above.

Customer Query: "I received my smart lamp today, but the Wi-Fi pairing light won't stop blinking red and it won't connect to my app."
___________________________________________________________________________________________________________
## 4. Preceding Question Prompting
Concept
Instructing the AI to evaluate specific diagnostic questions before responding. This technique minimizes bad assumptions, prevents premature solutions, and guides step-by-step troubleshooting.
You are a product troubleshooting chatbot. Before providing a final resolution to any technical issue, you must evaluate three preceding questions:

1. What specific hardware/software version is the user referring to?
2. Do I have enough information to solve this, or do I need to ask a clarifying question first?
3. What is the safest initial step that won't risk data loss?

Rule: If critical information is missing, ask the user only 1-2 clarifying questions first. Do not dump full troubleshooting steps until key details are confirmed.

User Input: "My app keeps crashing every time I try to check out my cart."
____________________________________________________________________________________________________________________
# Output
1. I am so sorry to hear that your package hasn't arrived yet! I would be more than happy to check the tracking status for you—could you please share your order number? Once I have that, I will look into its location right away.
 ____________________________________________________________
2. # Customer Support AI Assistant

A prompt engineering framework and operational blueprint for an e-commerce customer support AI model. Designed to handle order tracking, technical troubleshooting, and general inquiries while providing tone-matched customer responses and structured internal logging summaries.

---

##  Features

* **Intent Recognition:** Automatically categorizes inquiries into defined support workflows.
* **Dynamic Tone Alignment:** Adapts voice (Reassuring, Patient, Direct) based on user context and severity.
* **Structured Output Logging:** Outputs both customer-facing responses and standardized internal logs for CRM / ticketing integration.

---

##  Intent Matrix & Handling Rules

| Intent Category | Example Trigger Words | Required Information | Target Response Tone | Primary Workflow |
| :--- | :--- | :--- | :--- | :--- |
| **Order Tracking** | *where is my package, delayed, shipping status, track order* | Order ID, Tracking Number | Reassuring, efficient | Politely request missing order details; look up package location. |
| **Troubleshooting** | *broken, not working, error code, setup issue* | Device model, specific symptom | Patient, step-by-step | Walk through troubleshooting steps or direct to returns portal if hardware fails. |
| **General Inquiries** | *refund policy, store hours, shipping costs* | Specific query topic | Direct, informative | Answer clearly and concisely (under 3 sentences unless complex). |

---
____________________________________________________________________________________________________________
3. #  Customer Support AI Assistant

A prompt engineering framework and operational blueprint for an e-commerce customer support AI model. Designed to handle order tracking, technical troubleshooting, and general inquiries while providing tone-matched customer responses, variable extraction, and structured logging.

---

##  Features

* **Intent Recognition & Emotion Analysis:** Identifies user intent and underlying sentiment to tailor the response.
* **Variable Extraction Template:** Dynamically fills missing metadata fields (`[_____]`) prior to generating final output.
* **Dynamic Tone Alignment:** Adapts voice (Reassuring, Patient, Direct) based on user context and severity.
* **Structured Output Logging:** Outputs customer-facing responses along with standardized internal logs for CRM / ticketing integration.

---

## Intent Matrix & Handling Rules

| Intent Category | Example Trigger Words | Required Information | Target Response Tone | Primary Workflow |
| :--- | :--- | :--- | :--- | :--- |
| **Order Tracking** | *where is my package, delayed, shipping status, track order* | Order ID, Tracking Number | Reassuring, efficient | Politely request missing order details; look up package location. |
| **Troubleshooting** | *broken, not working, error code, setup issue* | Device model, specific symptom | Patient, step-by-step | Walk through troubleshooting steps or direct to returns portal if hardware fails. |
| **General Inquiries** | *refund policy, store hours, shipping costs* | Specific query topic | Direct, informative | Answer clearly and concisely (under 3 sentences unless complex). |

---
____________________________________________________________________________________________________
4. #  Customer Support AI Assistant

A prompt engineering framework and operational blueprint for an e-commerce customer support AI model. Designed to handle order tracking, technical troubleshooting, and general inquiries while using step-by-step pre-evaluation logic to avoid overwhelming users.

---

## Features

* **Pre-Evaluation Logic:** Evaluates target platform, missing parameters, and safety risks prior to responding.
* **Streamlined Troubleshooting:** Requests missing critical details first rather than dumping multi-step solutions upfront.
* **Variable Extraction & Tagging:** Identifies intent, emotion, and missing parameters to enable downstream CRM logging.
* **Dynamic Tone Alignment:** Adapts voice (Reassuring, Patient, Direct) based on severity and context.

---

## Intent Matrix & Handling Rules

| Intent Category | Example Trigger Words | Required Information | Target Response Tone | Primary Workflow |
| :--- | :--- | :--- | :--- | :--- |
| **Order Tracking** | *where is my package, delayed, shipping status, track order* | Order ID, Tracking Number | Reassuring, efficient | Politely request missing order details; look up package location. |
| **Troubleshooting** | *broken, crash, error code, setup issue* | App version, OS / Device model, specific symptom | Patient, step-by-step | Ask 1–2 clarifying questions first; present non-destructive fixes before complex steps. |
| **General Inquiries** | *refund policy, store hours, shipping costs* | Specific query topic | Direct, informative | Answer clearly and concisely (under 3 sentences unless complex). |


______________________________________________________________________________________________________________-

# Conclusion 
 The various types of Prompts are executed successfully with generated the report.
 

