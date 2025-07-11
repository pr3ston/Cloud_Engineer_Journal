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