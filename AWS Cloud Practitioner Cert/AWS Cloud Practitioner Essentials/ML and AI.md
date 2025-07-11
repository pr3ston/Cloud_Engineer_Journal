AI - Broad field focused on the development of intelligent computer systems capable of performing humanlike tasks

ML - Type of AI for training machines to perform complex tasks without explicit instructions. 
- Training finds the patterns hidden in vast amounts of data to produce ML model
- ML model then applied to new data to make predictions/decisions based on what it learned

## AWS AI/ML Solutions
#### AI Services
- pre-built models that are already trained to perform specific functions
###### Language services
- Interpret speech
- Amazon Comprehend
	- Uses natural language process to extract key insights from documents.
	- Key phrases, language, sentiment, other common elements
- Polly
	- Converts text to lifelike speech.
	- Supports multiple languages, different genders, variety of accents
	- Virtual assistances, e-learning apps, accessibility enhancements
- Transcribe
	- Speech to text
	- Multiple languages
	- Speaker identification, custom vocab, real-time subscription
	- Call transcription, automated subtitling, metadata generation for media content
- Translate
	- Text translation
	- For global communication
	- Real-time and batch text translation
###### Computer vision and search services
- Answering questions and gathering insights from various types of content sources
	- Documents, images, videos, etc.
- Kendra
	- Uses natural language process to search for answers within large amount of enterprise content.
	- Understands context of a query -> precise/relevant answers
	- Chatbots, app search integration, intelligent search
- Rekognition
	- Video analysis service
	- Identify objects, people, text, scenes, activities within images and videos stored in S3
	- Content moderation, identity verification, media analysis, home automation
- Textract
	- Detects and extracts typed and written text found in documents, forms, and tables in documents
	- Financial, healthcare, government form text extraction for quick processing
###### Conversational AI and personalization services
- Users interact with apps through text/voice conversations.
- Lex
	- Add voice and text conversational interfaces to apps
	- Uses natural language understanding and automatic speech recognition
	- For virtual assistants, natural language for FAQs, automated app bots
- Personalize
	- Use historical data to build intelligent apps
	- Personalized streaming, product and trending recommendations
#### ML Services
- A more customized approach with Amazon SageMaker AI where you build, train, and deploy your own ML models with fully managed infrastructure
###### SageMaker AI
- Fully managed
- Build, train, deploy your own ML models
- SageMaker IDE provides simplified access control
	- Track experiments, visualize data, debug/monitor workflows
- Offers pretrained models
#### ML frameworks and infrastructure
- A completely custom approach to building models and using purpose-built chips that integrate with popular ML frameworks
- Allow complete control over ML training process
###### Core Components
- ML frameworks
	- library or tool that provides experienced ML practitioners with pre-built, optimized components for building ML models
	- Supports PyTorch, Apache M-X Net, TensorFlow
- AWS ML Infrastructure
	- ML infra like ML EC2, EMR, ECS can support your custom solutions

## Deep Learning
- Subset of machine learning
- Models are trained using layers of artificial neurons that mimic human brain
- Each layer summarizes and feds info to next layer until final model produced
## Generative AI
- Type of deep learning powered by extremely large ML models known as foundation models (FMs)
- FMs are pretrained on vast collections of data
- FMs can be adapted to perform multiple tasks
	- create videos, images, music, etc
- LLMs are type of FM trained to use human language

#### Amazon SageMaker JumpStart
- Select form pre-trained FMs and ML solutions
- Fully customizable models for your use case and data
- Quickly deploy
- Library of pre-built ML solutions
	- computer vision, NLP, tabular data

#### Amazon Bedrock
- Fully managed
- Customize FMs from AWS and leading AI companies
- Access FMs through single API

#### Amazon Q
- Generative AI assistant tailored for you

###### Amazon Q Business
- Can answer pressing questions, solve problems, take action using data and expertise fround in company information repos
- For information requests, automated workflows, insight extraction

###### Amazon Q Developer
- Provides code recommendations
	- C#, Java, JS, Python, TypeScript
- Integrates with multiple IDEs

## Data Analytics
- When analysts transform raw historic data to uncover valuable insights/trends

#### ETL Process
- Extract data from various sources
- Transform data into consistent usable format
- Load data into destination system

#### AWS Data Pipeline Services
- Ingest
	- AWS Kinesis
		- Ingest data in real-time
		- Deliver to multiple apps
	- AWS Data Firehose
		- Ingest data in near real-time
		- Batch, compress, encrypt data before loading
	- AWS Glue (Data Catalog Feature)
		- Fully managed metadata repo
		- Discover, catalog, manage data
		- Automate data discovery
		- Data governance, compliance support
- Transform
	- Fully managed ETL service
	- Create ETL jobs visually 
	- Simple code-free data processing
- Storage
	- S3 (Data Lake, flexible), 
	- Redshift (Data Warehouse, more structured)
- Load/Process
	- EMR
		- Perform large-scale complex data processing with popular frameworks
		- More control/flexibility
- Visualization
	- Quicksight
		- Interactive business intelligence dashboards and reports
		- Highly scalable
		- For technical and non-technical users
		- Can be used with Amazon Q
	- OpenSearch Service
		- Real-time search, monitoring, analysis of business/operational data
		- For app monitoring, log analysis, website search
- Query
	- AWS Athena
		- Fully managed, serverless
		- For standard, infrequent SQL queries
		- Analyze data across different envs
	- AWS Redshift
		- Fully managed data warehouse
		- For complex queries
		- Find-grained query control
		- Advanced features
- 