
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





