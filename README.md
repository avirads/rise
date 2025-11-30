
Usecase: A company is launching a new product into the market. The product's features,specifications and data are fed into Rise AI.

Head of Product, employs a marketing team to create awareness of the product to the public. Marketing team consists of marketing agents who use Rise. Each marketing agent generates artefacts, reviews them and posts them to social media handles autonomously. Head of Product, monitors the efforts of the team and the performance of the posts.

Users:
Head of Product
Marketing agents


Rise AI consists of 
	A processor used by marketing agents to create marketing artefacts.
	A dashboard used by Head of Product showing efforts of the marketing agents.
	A leaderboard  used by Head of Product for tracking performance of the posts in realtime.


Rise AI - Internals

1. Architechture
	On the client, Rive is used for the UI/UX.
	On the server, AI nocode frameworks [flowise/n8n/comfyui] are used.
		For content generation, 
			Rise handles LLM integraions.
			Rise invokes Agentic AI workflows for Generative AI diffusion models.

2. AI Data Feed
	A RAG converts the product's IP into searchable vectors for easier integration into LLM's. 

3. Rive UI for Marketing Agents
	Chat interface is used by marketing agents to generates artefacts[images, videos and articles] of the product based upon prompts.

4. Rive UI Leaderboard 
	Leaderboard is used by Head of Product to track the efforts of the Marketing team.

5. Rive UI Dashboard 
	Dashboard is used by Head of Product to track the performance of the socila media posts.


In Rive Components are used for Data Binding.
Components have reduced repetition and provided a cleaner approach. The stats related to the posts and marketing work are connected to the actual data using View Models. This decouples design and code and the data contract allows the UI and backend teams to work independently. This decoupling is important because in the current stage of AI, lot of experimentation is needed by the backend teams in selection, testing and rejection of AI models that meet the functionality required by Rise AI.

DataBinding Usage can be seen in Leaderboard and Dashboard

In Leaderboard, Stats, foreground and background Colors are bound to the view model instances. 
In Dashboard, Likes, Comments and Reposts are bound to the view model instances.



