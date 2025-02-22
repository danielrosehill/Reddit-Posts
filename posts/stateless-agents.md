# Agent building framework with stateful sytem prompt handling

22-Feb-25

Looking for: agent building framework for large personal network with intelligent system prompt handling (stateful)

I've been working on building out a personal network of AI assistants over the past couple of years with the view that it will, over the long term, prove to be a strong digital asset of sorts.

I quite enjoy writing system prompts and have created ones for many niche purposes (today's one: send photos, suggest home DIY repairs!). Thus my network has mushroomed to more than 700 of them.

I'm working currently on choosing the right framework to provision the network and add the requisite front-end elements. 

What I've observed: so many of the agent tools seem to be designed with the enterprise function in mind in which just a couple of configurations need to be optimised and deployed as custom service chatbots (etc). My use case is rather different and the required needs are more in the realm of a single frontend for quick agent switching and ideally also orchestration. 

My overall AI philosophy is to avoid dependence on any one provider's ecosystem or API. So although I like how OpenAI Assistants API provides a very sensible approach to build out AI assistants and provides all the moving parts required like vector storage for context, it also comes at an enormous price: vendor lock.

The other difficulty I've noticed in building out these agent tools is the question of handling system prompts in a way that doesn't bog down the context window. I've noticed that lengthier system prompts tend to be quite effective in guiding very determinative behaviour traits for an agent and are thus effective. But in stateless architectures, these longer prompts quickly eat away at context and result in high token usage and ultimately significantly higher API charges.

So two design considerations are guiding my choice of framework (if I use one): something built for this kind of thing (ideally). And just as importantly: a framework  