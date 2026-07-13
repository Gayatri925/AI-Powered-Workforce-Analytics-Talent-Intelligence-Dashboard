# AI-Powered-Workforce-Analytics-Talent-Intelligence-Dashboard
**<ins>Project Statement:</ins>**
<p>This project focuses on developing an AI-Powered Workforce Analytics & Talent Intelligence Dashboard that enables organizations to gain actionable insights into workforce performance, employee engagement, talent development, diversity, attrition, recruitment effectiveness, and organizational health. The solution leverages Large Language Models (LLMs), Retrieval-Augmented Generation (RAG), predictive analytics, and agentic AI workflows to transform disparate HR and workforce data into strategic business intelligence. By automating real-time analytics and conversational querying, the platform empowers HR leaders and executives to make data-driven decisions regarding workforce planning, retention strategies, and skill development, ultimately allowing organizations to proactively address talent challenges and optimize organizational performance.</p>

**<ins>Outcomes:</ins>**
<ul>
<li>Comprehensive visibility into workforce performance, demographics, and organizational trends.</li>
<li>Predictive analytics to identify attrition risks and recommend proactive retention strategies.</li>
<li>Actionable insights into employee skills, learning progress, and career development.</li>
<li>Monitoring of diversity, equity, and inclusion metrics across the organization.</li>
<li>Intelligent, AI-powered recommendations for workforce planning and engagement.</li>
<li>Natural language interaction for rapid, data-driven workforce intelligence.</li>
</ul>

**<ins>Solution:</ins>**
<p>
<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/557b9544-c716-41cf-bf10-b7c47026e141" />
</p>

**<h2><ins>Step By Step Workflow:</ins></h2>**
<h3>Step 1: Data Ingestion</h3>
<ul>
	<li>Collect workforce data from Snowflake, Oracle HCM, and external APIs.</li>
	<li>Export Snowflake data to Google Cloud Storage using COPY INTO.</li>
	<li>Extract Oracle HCM data using Google Cloud Dataflow (JDBC Batch Template).</li>
<li>Trigger Cloud Functions using Cloud Scheduler to fetch API data.</li>
<li>Store all raw data in Google Cloud Storage for further processing.</li>
</ul>
<p>Technology Used: Snowflake, Oracle HCM, Google Cloud Storage, Cloud Dataflow, Cloud Scheduler, Cloud Functions</p>
<h3>Step 2: Workflow Orchestration</h3>
<ul>
	<li>Schedule and automate the complete ETL workflow.</li>
<li>Manage data extraction, loading, transformation, and AI model refresh.</li>
<li>Ensure each stage executes in the correct sequence through a daily workflow.</li>
</ul>
<p>Technology Used: Cloud Composer (Apache Airflow)</p>
<h3>Step 3: Data Storage & Transformation (Backend)</h3>
<ul>
	<li>Store the raw workforce data in Google Cloud Storage.</li>
<li>Load processed data into BigQuery as the centralized data warehouse.</li>
<li>Perform SQL-based transformations using Dataform.</li>
<li>Clean, validate, model, and prepare workforce data for analytics.</li>
</ul>
<p>Technology Used: Google Cloud Storage, BigQuery, Dataform</p>
<h3>Step 4: AI & Analytics Processing (Backend)</h3>
<ul>
	<li>Analyze transformed workforce data using Vertex AI and BigQuery ML.</li>
<li>Generate attrition predictions, skill gap analysis, workforce health scores, recruitment analytics, diversity metrics, and learning recommendations.</li>
<li>Create vector embeddings for semantic search.</li>
<li>Use Gemini with a Retrieval-Augmented Generation (RAG) pipeline to provide intelligent responses and recommendations.</li>
</ul>
<p>Technology Used: Vertex AI, BigQuery ML, Vertex AI Embeddings, Vector Search, Gemini (LLM), RAG</p>
<h3>Step 5: Frontend Integration</h3>
<ul>
	<li>Display workforce insights through the Web Interface (Dashboard).</li>
<li>Present Workforce KPIs such as attrition, recruitment, diversity, and learning analytics.</li>
<li>Integrate an AI Chat Interface for natural language interaction.</li>
<li>Retrieve real-time analytics and AI responses from the backend services.</li>
</ul>
<p>Technology Used: Web Interface (React/Next.js or equivalent), BigQuery APIs, Vertex AI APIs, Gemini APIs, AI Chat Interface</p>
<h3>Step 6: Security & Governance</h3>
<ul>
	<li>Authenticate and authorize users securely.</li>
<li>Protect sensitive workforce credentials and data.</li>
<li>Maintain metadata, monitor system activities, and enforce data protection policies</li>
</ul>
<p>Technology Used: Google Cloud IAM, Secret Manager, Data Catalog, Cloud Audit Logs, Encryption, VPC Service Controls</p>
<h3>Step 7: End User Interaction</h3>
<ul>
	<li>HR Managers, Executives, and Business Stakeholders access the dashboard.</li>
<li>Monitor Workforce KPIs and organizational performance.</li>
<li>Interact with the AI chatbot using natural language queries.</li>
<li>Make informed, data-driven workforce planning and talent management decisions.</li>
</ul>
<p>Technology Used: Web Browser, Web Interface, AI Chat Interface, BigQuery, Vertex AI, Gemini LLM</p>
<h4>Tech Stack</h4>
<ul>
	<li>Cloud Platform: Google Cloud Platform (GCP)</li>
<li>Programming Language: Python</li>
<li>Data Sources: Snowflake, Oracle HCM, External APIs</li>
<li>Data Ingestion: Cloud Storage, Cloud Dataflow, Cloud Functions, Cloud Scheduler</li>
<li>Workflow Orchestration: Cloud Composer (Apache Airflow)</li>
<li>Data Warehouse: BigQuery</li>
<li>Data Transformation: Dataform</li>
<li>AI/ML: Vertex AI, BigQuery ML, Gemini (LLM), Vertex AI Embeddings, Vector Search, Retrieval-Augmented Generation (RAG)</li>
<li>Frontend: React.js / Next.js (or Custom Web Interface)</li>
<li>Visualization: Web Dashboard</li>
<li>Security & Governance: IAM, Secret Manager, Data Catalog, Cloud Audit Logs, VPC Service Controls, Encryption</li>
</ul>
