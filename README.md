![Secret Sauce AI](https://github.com/secretsauceai/secret_sauce_ai/blob/main/SSAI_logo_2.3_compressed_cropped.png?raw=true)
## tl;dr a coordinated community of tech minded AI enthusiasts

# Secret Sauce AI Overview
- [Introduction](https://github.com/secretsauceai/secret_sauce_ai#introduction)
- [The three Secret Sauce AI ingredients](https://github.com/secretsauceai/secret_sauce_ai#ingredients)
    - [Community](https://github.com/secretsauceai/secret_sauce_ai#community): community comes first 
    - [Program](https://github.com/secretsauceai/secret_sauce_ai#program): management, projects, deliverables
    - [Philosophy](https://github.com/secretsauceai/secret_sauce_ai#philosophy): values, principles
- [Introduction to voice assistant data pipelines](https://github.com/secretsauceai/secret_sauce_ai#for-the-casual-reader-introduction-to-voice-assistant-data-pipelines)
# Introduction

Secret Sauce AI is a coordinated community of tech minded AI enthusiasts working together on projects to identify blockers and improve the basic open source tools and pipeline components in the AI (voice) assistant pipeline (wakeword, ASR, NLU, NLG, TTS) mostly geared for deployment on edge devices and self hosted solutions. This is not a voice assistant project in and of itself, rather Secret Sauce AI helps AI (voice) assistant projects come together as individuals and solve basic problems faced by the entire community.

Although this community is geared toward developers and data scientists in the FOSS (voice) AI assistant community, we hope our projects will trickle down to end users. If you are reading this as a casual reader, it is recommened to read the [introduction to voice assistants](https://github.com/secretsauceai/secret_sauce_ai#for-the-casual-reader-introduction-to-voice-assistant-data-pipelines) first to have a bit of background on this subject. 

<img align="left" height=45% width=45% src="https://github.com/secretsauceai/secret_sauce_ai/blob/main/SSAI_3_main_ingredients_compressed_cropped.png " />

# Ingredients
Secret Sauce AI is made out of 3 main ingredients:
* Community
* Program
* Philosophy
<br/>
<br/>
<br/>
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
* Check out our 🗺️ [Program roadmap](https://github.com/secretsauceai/secret_sauce_ai/projects/2)
* Have a look at the 🔨 [Program Kanban board](https://github.com/secretsauceai/secret_sauce_ai/projects/1)
* Join our [Slack](https://join.slack.com/t/secretsauceorg/shared_invite/zt-13u24g71z-5dUqoH8OGN4QpQffUIJANQ)

### I'm a tinkerer or user, what about me?
We don't want to leave anyone out, but our scope is currently pretty limited in engaging users and tinkers. You can always write me (Bartmoss) directly on [reddit](https://www.reddit.com/user/Bartmoss) or you can check out many of the projects built for users and tinkerers alike by our community. 

### Member Projects
A lot of our Secret Sauce AI members build FOSS voice assistant software. It is always worth checking their software out. We just love this community!
* 🔥 [OpenVoiceOS](https://openvoiceos.com/)
* 🔥 [Athena](https://github.com/Tadashi-Hikari/Athena) and 🔥 [The Sapphire Assistant Framework](https://github.com/Tadashi-Hikari/Sapphire-Assistant-Framework)
* 🔥 [Lily](https://github.com/sheosi/lily)
* 🔥 [Leon AI](https://getleon.ai/)
* 🔥 [GLaDOS Voice Assistant](https://github.com/Nerdaxic/GLaDOS-Voice-Assistant)
* 🔥 [V.I.S.O.R.](https://github.com/DADi590/V.I.S.O.R.---A-real-assistant--Android-Client)

## Program
A community must coordinate to be more than the mere sum of its parts. We believe heavily in Agile management, but with an open source twist. Applying traditional project management practices geared for business doesn't always work well in a free and open community made up of people who do what they do on a voluntary basis out of a deep seated passion for AI. Therefore, we try to reduce the risks of these kinds of projects and focus on bringing maxmimum value by rapidly prototyping over building end user solutions. By engaging the community at large and showing the value of the deliverables, those prototypes can trickle down to power future AI in software for end users.

* 🗺️ [Program roadmap](https://github.com/secretsauceai/secret_sauce_ai/projects/2)
* 🔨 [Program Kanban board](https://github.com/secretsauceai/secret_sauce_ai/projects/1)

### Projects
* [Wakeword](https://github.com/secretsauceai/secret_sauce_ai/wiki/Wakeword-Project) (phase 1 of project complete)
    * 📦 [Wakeword Data Collector](https://github.com/secretsauceai/wakeword-data-collector) (prototype done)
    * 📦 [Precise Wakeword Model Maker](https://github.com/secretsauceai/precise-wakeword-model-maker) (prototype done)
    * 📦 [Precise TensorFlow lite engine](https://github.com/OpenVoiceOS/precise-lite) (done)
    * 🚧 📦 [SpeechPy MFCC in Rust](https://github.com/secretsauceai/mfcc-rust) (in progress)
    * 🚧 📦 [Precise Rust runner](https://github.com/sheosi/precise-rs) (prototype in testing)
* 🚧 NLU-NLG (phase 1 of project in progress)
    * 📔 [NLU engine prototype example and benchmarks](https://github.com/secretsauceai/NLU-engine-prototype-benchmarks) (in progress)
    * 📔 [Snips data set converter](https://github.com/secretsauceai/NLU-snips-converter) (in progress)
* ASR-TTS
* 🚧 Bus (phase 1 of project in progress)
    * 📦 [Voice Assistant Protocol (VAP)](https://github.com/secretsauceai/voice-assistant-protocol) (in progress)


## Philosophy
### Values
* Benchmarking
* Privacy
* Data

### Principles
* Benchmarks show benefit: compare solutions and clearly communicate the differences
* AI over hard coding
* AI is only AI if it can learn directly from the users

<img align="right" height=50% width=50% src="https://github.com/secretsauceai/secret_sauce_ai/blob/main/TinyML%2B_learning_lifecycle.png"/>

To completely respect a user's privacy while collecting data, we find that it is best to keep the data on the user's system and run the machine learning totally locally.

A similar approach when applied to running model inference locally is called [TinyML](https://www.tinyml.org/). We call our approach *TinyML+*, the plus stands for training. With this TinyML+ approach, we can fulfil the principle of AI. 


In the TinyML+ learning cycle, data is collected from the user, a model is trained from the data, the model is used by the user where defects can be found, and further data collection leads to a closed cycle of learning. 

Simple put: instead of general models based on collection of user's personal data, the data stays on the user's device where it is used to train a model locally.

This local model belongs to the user, just as much as the data used to train this model.

As the system collects more data, it improves. This accomplishes our value of user privacy while creating AI that can learn and grow. 

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
![Voice assistant pipeline](https://github.com/secretsauceai/secret_sauce_ai/blob/main/Voice_Assistant_Pipeline.png)
Let's take a look at the basic components. It starts with a user who wants to 'wake' the voice assiant. Once the system is listening, the user speaks the utterance and it's transcribed. After transciption it is processed for intent to figure out the meaning. Once the meaning (intent) has been extracted from the utterance, the voice assistant does the requested task triggered by the intent. A response is generated which is spoken by the text to speech system.

Let's walk through a concrete example: a user wants to wake up the voice assistant and ask 'what's the weather like in Munich tomorrow'.

- Wakeword (hotword): usually a binary acoustic model that constantly runs in the background to spot the wakeword (ie 'hey Jarvis')
- ASR: once the wakeword has been identified, this triggers the ASR to transcribe the utterance into a normalized text (what's the weather like in Munich tomorrow)
- NLU: the uttrance `{'what's the weather like tomorrow in Munich'}`, is broken down by intent and the entities (keywords) `'intent': 'weather_forecast', 'entities': {'date-time': 'tomorrow', 'location': 'Munich'}`
- the weather skill contains instructions on how the entities are passed to the API to get the weather forecast for the date that is `'tomorrow'` for `'Munich'`
- NLG: the information provided by the weather API is formatted (slotted) usually using a response template response: `'{tomorrow} in {Munich} it will be {cloudy} with a high of {22} and a low of {13} degrees'`
- TTS: the TTS reads the NLG response out loud for the user.
