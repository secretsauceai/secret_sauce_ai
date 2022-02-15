![Secret Sauce AI](https://github.com/secretsauceai/secret_sauce_ai/blob/main/SSAI_logo_2.3_compressed_cropped.png?raw=true)
## tl;dr a coordinated community of tech minded AI enthusiasts

# Secret Sauce AI Overview (under heavy construction!)
- [Introduction](https://github.com/secretsauceai/secret_sauce_ai#introduction)
    - [Focus](https://github.com/secretsauceai/secret_sauce_ai#focus)
    - [Philosophy](https://github.com/secretsauceai/secret_sauce_ai#philosophy)
    - [Method](https://github.com/secretsauceai/secret_sauce_ai#method)
- [Program resources](https://github.com/secretsauceai/secret_sauce_ai#program-resources)
    - [Current projects](https://github.com/secretsauceai/secret_sauce_ai#current-project)
 - [Introduction to voice assistant data pipelines](https://github.com/secretsauceai/secret_sauce_ai/blob/main/README.md#for-the-casual-reader-introduction-to-voice-assistant-data-pipelines)
    - [More information](https://github.com/secretsauceai/secret_sauce_ai#more-information)
# Introduction

Secret Sauce AI is a coordinated community of tech minded AI enthusiasts working together on projects to identify blockers and improve the basic open source tools and pipeline components in the AI (voice) assistant pipeline (wakeword, ASR, NLU, NLG, TTS) mostly geared for deployment on edge devices and self hosted solutions. This is not a voice assistant project in and of itself, rather Secret Sauce AI helps AI (voice) assistant projects come together as individuals and solve basic problems faced by the entire community.

Although this community is geared toward developers and data scientists in the FOSS (voice) AI assistant community, we hope our projects will trickle down to end users. If you are reading this as a casual reader, it is recommened to read the [introduction to voice assistants](https://github.com/secretsauceai/secret_sauce_ai/blob/main/README.md#for-the-casual-reader-introduction-to-voice-assistant-data-pipelines) first to have a bit of background on this subject. 

<img align="left" height=35% width=35% src="https://github.com/secretsauceai/secret_sauce_ai/blob/main/SSAI_3_main_ingredients_compressed_cropped.png " />

# Ingredients
Secret Sauce AI is made out of 3 main ingredients:
* Community
* Program
* Philosophy

<br/>
<br/>
<br/>
<br/>

## Community
We are nothing without the community behind us, and this is why community always comes first. There are (currently) 4 defined roles:
* Developer
* Data scientist
* Tinkerer
* User

Our current focus is on developers and data scientists. These are the folks that are building the technology that will trickle down to tinkerkers and users.

### Are you a developer or data scientist interested in joining our community?
After reading through our program overview and other relevent links:
* check out our [program roadmap](https://github.com/secretsauceai/secret_sauce_ai/projects/2)
* have a look at the [program Kanban board](https://github.com/secretsauceai/secret_sauce_ai/projects/1)
* join our [slack](https://join.slack.com/t/secretsauceorg/shared_invite/zt-12aqaii01-l~nu2078PyeGZDk0L6vl7Q)

### I'm a tinkerer or user, what about me?
We don't want to leave anyone out, but our scope is currently pretty limited in engaging users and tinkers. You can always write me (Bartmoss) directly on [reddit](https://www.reddit.com/user/Bartmoss) or you can check out many of the projects built for users and tinkerers alike by our community. 

### Member Projects
A lot of our Secret Sauce AI members build FOSS voice assistant software. It is always worth checking their software out. We just love this community!
* [OpenVoiceOS](https://openvoiceos.com/)
* [Athena](https://github.com/Tadashi-Hikari/Athena) and [The Sapphire Assistant Framework](https://github.com/Tadashi-Hikari/Sapphire-Assistant-Framework)
* [Lily](https://github.com/sheosi/lily)
* [Leon AI](https://getleon.ai/)
* [GLaDOS Voice Assistant](https://github.com/Nerdaxic/GLaDOS-Voice-Assistant)

## Program
A community must coordinate to be more than the mere sum of its parts. We believe heavily in Agile management, but with an open source twist. Applying traditional project management practices geared for business doesn't always work well in a free and open community made up of people who do what they do on voluntary basis out of a deep seated passion for AI. Therefore, we try to reduce the risks of these kinds of projects and focus on bringing maxmimum value by rapidly prototyping over building end user solutions. By engaging the community at large and showing the value of the deliverables, those prototypes can trickle down to power future AI in software for end users.

### Projects
* [Wakeword](https://github.com/secretsauceai/secret_sauce_ai/wiki/Wake-Word-Project)
* NLU-NLG
* ASR-TTS
* Bus

TODO: Add project descriptions

## Philosophy

How many folks want their own AI, but even though we live in the future from our childhood dreams, it doesn't seem any closer. The open source community isn't there yet. With Secret Sauce AI, we help the community achieve those dreams of their own personal AI by providing that secret sauce flavor by bringing the community together, to focus on AI solutions.

Note the term 'personal AI'. Everyone has their own use cases, their own ideas. The AI has to be modular and customizable to realize these dreams. But it needs one more component, the most important of all...

It needs to learn from the user's interactions (without the user having to program it!). If an AI can't learn, it isn't an AI. People will have a lot more patients for an AI that actually learns. When they know they can teach it, they will want to treat it more like a child and they will be even more immersed in the 'Wizard of Oz' effect. 

Finally, we really respect user's privacy. Normally, voice assistants are glorified data scrapers and the models and methods used within the voice assistant are supposed to be a 'once size fits all' approach. However, if there is one thing we have learned from doing this professionally and personally for years is: there is no such thing as a general model that works for everyone. To achieve privacy and 'real AI' that can learn from the user, we avocate 'TinyML'. 

Simple put: instead of general models based on collection of user's personal data, the data stays on the user's device where it is used to train a model locally. This local model belongs to the user, just as much as the data used to train this model. As the system collects more data, it improves. This accomplishes our goals of user privacy while creating AI that can learn and grow. 

## Method
General what is our approach to solving these problems? The method statement is simple yet is complex because an AI (voice) assistant covers a broad domain of disciplines and the process is also iterative:

- Define your personal MVP
    - requirements
    - blockers
    - open questions (problem statements)
    - benchmarking possible methods
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
- benchmarking solutions
- automating the model generation data pipeline

## Current project: [NLU project]()
- protype NLU solutions for teaching and benchmarking purposes
- improve open source data set for voice assistants
- general benchmark of methods for performance vs resource usage (f1 scores of intent and entity extraction vs CPU% for training and inference)
- deep dive into current production solutions for NLU
- create modular NLU engine design (hot swap out classifiers)

# For the casual reader: introduction to voice assistant data pipelines
For the casual reader, these subjects can be hard to understand (how voice assistants actually work can be quite complicated), but since it seems there is a lot of interest about our projects from casual users, let's introduce this subject. let's start with some basic vocabulary.

## Key vocabulary
- ***utterance:*** command, question, or query from a user (ie 'turn on the kitchen lights')
- ***response:*** the written response to an utterance by the assistant/chatbot (ie 'I turned on the living room lights')
- ***word slotting:*** often times a response is based on a template and words are slotted in to give a correct response, this can also include grammar (this is pretty easy in English, it's in other languages that templating becomes more complex and is often overlooked in the construction of such systems) (ie 'the living room lights are now on' template: the [entity] [singular|plural] now on)
- ***tagged words:*** utterances can contain inputs for actions and/or responses, these are referred to as entities, tagging these entities is also known as NER (named entity recognition) (ie 'turn on the kitchen lights', entity: kitchen lights) or entity extraction
- ***intent:*** when an utterance is classified for its action and or response (some systems use the tagged words to find intent, others use the whole utterance) (ie 'turn on the kitchen lights' -> skill: home assistant, action: turn on/off, entity: kitchen lights)
- ***NLU:*** natural language understanding, this usually describes finding the intent and word tagging more generally (ie NLU engine, an engine that performs the intent classification and word tagging)
- ***NLG:*** natural language generation, this describes the creation of responses to utterances. It can include actual generation (using some kind of language model that requires the utterance as prompt), or the more common approach of using templates and word slotting.
- ***ASR:*** automated speech recognition, also known as STT, speech to text.
- ***wakeword:*** a specific word or phrase (for best results it should be at least 3 syllables) trained into a binary class acoustic model (wakeword or not-wakeword) used to activate the ASR (ie 'hey jarvis')
- ***TTS:*** text to speech
- ***NLP:*** natural language processing, this covers all of these tasks and many more

## Voice assistant pipeline
Let's take a look at the basic components. It starts with a user who wants to 'wake' the voice assiant. Once the system is listening, the user speaks the utterance and its transcribed. After transciption it is processed for intent to figure out the meaning. Once the meaning (intent) has been extracted from the utterance, the voice assistant does the requested task triggered by the intent. A response is generated which is spoken by the text to speech system.

Let's walk through a concrete example: a user wants to wake up the voice assistant and ask 'what's the weather like in Munich tomorrow'.

- Wake word (hot word): usually a binary acoustic model that constantly runs in the background to spot the wake word (ie 'hey Jarvis')
- ASR: once the wake word has been identified, this triggers the ASR to transcribe the utterance into a normalized text (what's the weather like in Munich tomorrow)
- NLU: the uttrance {'what's the weather like tomorrow in Munich'}, is broken down by intent and the entities (key words) 'intent': 'weather_forecast', 'entities': {'date-time': 'tomorrow', 'location': 'Munich'}
- the weather skill contains instructions on how the entities are passed to the API to get the weather forecast for the date that is 'tomorrow' for 'Munich'
- NLG: the information provided by the weather API is formatted (slotted) usually using a response template response: '{tomorrow} in {Munich} it will be {cloudy} with a high of {22} and a low of {13} degrees'
- TTS: the TTS reads the NLG response out loud for the user.

## More information
For more information, check out the detailed [program overview](https://github.com/secretsauceai/secret_sauce_ai/wiki) on the wiki.

You can also go straight to [Secret Sauce AI Program Board](https://github.com/secretsauceai/secret_sauce_ai/projects/1) to check out the status of issues in the projects as well as open questions the community is working on. 
