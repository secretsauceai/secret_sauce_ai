# secret_sauce_ai

# Secret Sauce AI Program Overview


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

## Key vocabulary

- ***utterance:*** command, question, or query from a user (ie 'turn on the kitchen lights')
- ***response:*** the written response to an utterance by the assistant/chatbot (ie 'I turned on the living room lights')
- ***word slotting:*** often times a response is based on a template and words are slotted in to give a correct response, this can also include grammar (this is pretty easy in English, it's in other languages that templating becomes more complex and is often overlooked in the construction of such systems) (ie 'the living room lights are now on' template: the [entity] [singular|plural] now on)
- ***tagged words:*** utterances can contain inputs for actions and/or responses, these are referred to as entities, tagging these entities is also known as NER (named entity recognition) (ie 'turn on the kitchen lights', entity: kitchen lights)
- ***intent:*** when an utterance is classified for its action and or response (some systems use the tagged words to find intent, others use the whole utterance) (ie 'turn on the kitchen lights' -> skill: home assistant, action: turn on/off, entity: kitchen lights)
- ***NLU:*** natural language understanding, this usually describes finding the intent and word tagging more generally (ie NLU engine, an engine that performs the intent classification and word tagging)
- ***NLG:*** natural language generation, this describes the creation of responses to utterances. It can include actual generation (using some kind of language model that requires the utterance as prompt), or the more common approach of using templates and word slotting.
- ***ASR:*** automated speech recognition, also known as STT, speech to text.
- ***wakeword:*** a specific word or phrase (for best results it should be at least 3 syllables) trained into a binary class acoustic model (wakeword or not-wakeword) used to activate the ASR (ie 'hey jarvis')
- ***TTS:*** text to speech
- ***NLP:*** natural language processing, this covers all of these tasks and many more

# Wake Word Problem Statements

- Pipeline
    - Many deprecated and/or closed-source solutions (ie Snowboy or Porcupine) and outdated or otherwise limited solutions (ie Pocketsphinx)
    - Only open source solution (Precise) is old (tf 1.13), heavy (26kb, uses ~25-30% CPU on raspi4 at all times).
- Data collection/training
    - Hard to train good models without deep knowledge and lots of data

## Proposed Solutions

- Create easy way to:
    - ~~collect data~~  (prototype done)
    - train optimal models (in progress: ALMOST DONE!)
- ~~Migrate Precise to tflite~~ (done)
- Experiment with optimal compression of tflite model
- Turn Precise TF2 runner (engine) into binary or otherwise easy to use deployment
    - Many folks want to run it on Android too!

For all the details of the solutions for the Wake Word project, see the wakeword project [documentation](https://www.notion.so/Wake-Word-Project-9f51d7db8e4b4510a9b097186536e6d6).

# NLU-NLG Problem Statements

The area isn't as tightly scoped as the wake word project, its still very much a work in progress! 🙂

- Pipeline
    - Mycroft uses outdated and limited engines, however it has many skills (of varying quality)
    - Rhasspy has many untested options, however most of them lack any skills (snips has skills: quality?)
    - Rasa is/was a mess (different versions, broken documentation, lack of higher level examples, forms have to be 'coded' instead of designed as a voice service)
        - Maybe the new version is better?
        - Lack of skills
        - No non-programmatic solution for forms
    - NLG systems are mostly very primitive (i.e. lack of grammatical agreement) and bundled with the NLU engine
    - Each NLU engine has its own format for skills (utterances, responses, entities, intents, actions), so one skill can't be used in another engine
- Data collection/training
    - Lack of GUIs to build skills (besides RasaX and Botfront)
    - No system to easily collect new utterances, entities and intents from user
    - Lack of automated defect management tools (classifying user defined defects and the correct utterance/intent/action/response)
    - No built in self help (ie wiki, knowledge base, self help desk)
    - No automated testing system to determine performance (lag, accuracy, defects) of NLU engines for selecting the best solution

## Proposed Solutions

- Review NLU-NLG engines
    - **Testing system:** Firstly, it would be great to have a general testing system, using a test/training set of utterances and responses to be able to run many different NLU engines and test their performance (CPU usage, correct intent classification, NER, responses, categorizing other defects). Maybe your language or use cases require a different NLU engine from mine, but how do you know what works best if you can't benchmark the engines?
        - Build data set of utterances and responses
        - Make script that tests each NLU-NLG engine from test data set and records performance and accuracy
        - JSON format or YAML? (Rasa uses YAML also docker and IoT/HASS folks love it, that might be interesting)
    - [Intent recognition](https://rhasspy.readthedocs.io/en/latest/intent-recognition/)
        - NOTE: although RASA is rated 'very slow', it should run on a raspi4. However at the time I tested it, they couldn't really get it running on an arm64 (aarch64) machine (I was able to finally get it running, but it was a total pain, however it technically 'works')
        - NOTE: the skills from Mycroft (and Snips) should work with whatever solution is found, because having some skills is better than starting from scratch. So this means either skills from different systems either need to be 'imported', some compatibility is required in the intent handling, or you use a system that passes correctly to each engine (where the engine handles everything as usual) when the intent is classified as going to that domain
            - this applies to the testing system and having universal skills or at least being able to import/export skills
- [Intent handling (passing to skills)](https://rhasspy.readthedocs.io/en/latest/intent-handling/), this should probably use MQTT (Hermes or something else?)
- **Simple Skill Building:** there is really no way to build skills easily. Even with RasaX there are no non-programmatic forms functions. This needs to be looked into to find an easier solution to skill building. There is where a lot of projects die.
    - Can skills have a generic 'form' so that they can be easily run in other NLU engines (compatibility), this would help bridge the gap of skill ecosystems (ie skills for Mycroft; Adapt and Padatious could be converted for use in other engines)
        - this ties into the testing system and the intent handling
- **Automatic Defect Management skill:** As both a fallback skill (not just saying 'I didn't understand that'), and a skill people can ask for (ie 'diagnostic mode')
    - Eliminate if it is an ASR issue with one question (repeat the utterance back to user and ask if correct)
    - Fix intents that are unclassified variations of known intents (adds variation from user into training)
    - Can log users desire for new functionality (the utterance has no supported intent, perhaps this intent is important and should be logged)
    - Utterance collision problem solving
        - if an utterance goes to the wrong intent, user can 'explain' that to system (ie user says utterance 'diagnostic mode'), then utterance maps to correct intent
    - Can fix minor issues with entities, responses (NLG issues), etc.
    - Similar to the 'learning skill' from Mycroft (learning skill only supports utterance and response, no follow ups, intents, actions, etc.)

The NLU-NLG project documentation, much like the NLU-NLG project itself, is still a work in progress. Stay tuned. It will be formalized once the prototype wake word project is completed.
