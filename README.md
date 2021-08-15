# Secret Sauce AI Program Overview (under heavy construction!)
- [Introduction](https://github.com/secretsauceai/secret_sauce_ai#introduction)
    - [Focus](https://github.com/secretsauceai/secret_sauce_ai#focus)
    - [Philosophy](https://github.com/secretsauceai/secret_sauce_ai#philosophy)
    - [Method](https://github.com/secretsauceai/secret_sauce_ai#method)
    - [Key vocabulary](https://github.com/secretsauceai/secret_sauce_ai#key-vocabulary)
   - [Program resources](https://github.com/secretsauceai/secret_sauce_ai#program-resources)
    - [Current project](https://github.com/secretsauceai/secret_sauce_ai#current-project)
    - [More information](https://github.com/secretsauceai/secret_sauce_ai#more-information)
# Introduction

Secret Sauce AI is an open source program (program in the sense of management, not software) for projects to identify blockers and improve the basic open source tools and pipeline components in the AI (voice) assistant pipeline (wakeword, ASR, NLU, NLG, TTS) mostly geared for deployment on edge devices and self hosted solutions. This is not a voice assistant project in and of itself, rather Secret Sauce AI helps AI (voice) assistant projects come together as individuals and solve basic problems faced by the entire community. 

## Focus

- tools
    - data collection
    - other small automation tools (automate: tutorials, how to's, recipes, etc. as CLIs, skills, and/or web tools)
- modular (can swap out components easily for customization, ie microservices)
- tweaking existing open source resources for improvements
- emphasis on 'tiny ML' and user-based data collection (data collection driven)
    - system learns from the user
    - data collection stays on the local device, it belongs to the user!
- documentation and how to's to help folks setup their own AI
    - Get a user onboarded by asking: "what's your personal AI (voice) assistant's MVP?"

## Philosophy

How many folks want their own AI, but even though we live in the future from our childhood dreams, it doesn't seem any closer. The open source community isn't there yet. With Secret Sauce AI, we help people achieve their dreams of their own personal AI by providing that secret sauce flavor.

Note the term 'personal AI'. Everyone has their own use cases, their own ideas. The AI has to be modular and customizable to realize these dreams. But it needs one more component, the most important of all...

It needs to learn from the user's interactions (without the user having to program it!). If an AI can't learn, it isn't an AI. People will have a lot more patients for an AI that actually learns. When they know they can teach it, they will want to treat it more like a child and they will be even more immersed in the 'Wizard of Oz' effect. 

## Method

The method statement is simple yet is complex because an AI (voice) assistant covers a broad domain of disciplines and the process is also iterative:

- Define your personal MVP
    - requirements
    - blockers
    - open questions (problem statements)
    - resources
- Break down the general domain of AI (voice) assistants (wake word, ASR, NLU, NLG, TTS, etc.) by category and:
    - blockers
    - how to's
    - open questions (problem statements)
    - resources
- Align the aspects of your MVP with that of the general domain categories (surprise, everyone has the same problems you do!)
- Prioritize work on the aligned components based on difficulty, always pick the lowest hanging fruit first
- Repeat

This method was first employed on the wake word problem(s), as this seems to be a quintessential problem of voice assistants. Almost all voice assistant systems require a good wake word system and none exists. Although in comparison to other categories, it could be called the lowest hanging fruit (less problems to solve, easier to scope, partial solutions exist). It was the hope of the program that this would galvanize the open source AI (voice) assistant community and in the process provide valuable deliverables that would unblock individuals' MVPs. 

Each category will spin off projects that will provide the deliverables that will greatly improve MVPs. The projects are there to help individuals achieve their MVPs.


# Program resources
## Current project: [wake word project](https://github.com/secretsauceai/secret_sauce_ai/wiki/Wake-Word-Project)
- data collection
- data generation
- creating optimal models
- improving architecture

## More information
For more information, check out the detailed [program overview](https://github.com/secretsauceai/secret_sauce_ai/wiki) on the wiki and the [kanban board](https://github.com/secretsauceai/secret_sauce_ai/projects/1)
