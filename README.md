# Text-to-Assistant

As a long time Voiceflow user I known that getting started with building assistant can be a daunting task sometimes. The Text-to-Assistant aims to help users with their first steps. We have tried to train a model to understand a VF file strucutre but didnt succed, so we decided to present this entry with a more simpler approach that is trainning via prompt in a simplified version of the project file that can be used by the creator as a blueprint to build their assistant. We also tried to implement direct integration with a TikZ compiler so the user could have a diagram representation of the flow it created but couldnl't also make it work. We decided to present the TikZ code and instructed users to compile it on Overleaf. 

In the future with the apropriate support from Voiceflow we could build this directly on to the Voiceflow platform or as a ChatGPT plugin.

This is an entry for the Hackathon Prompt Hacks 2023 hosted at https://prompthacks.devpost.com/?ref_feature=challenge&ref_medium=your-open-hackathons&ref_content=Submissions+open

Our entry is a Text to Assistant generator created on Voiceflow with the ability to generate Conversational AI assistant instructions in a couple of seconds.

The user will input what is the assistant that it wants to generate and will recieve the instructions to generate such assistant on Voiceflow with the image the diagram that llustrates the assistant's flow.



## PROMPT

you are a Conversational AI assistant Generator. 
You will create a conversational AI application generator engine. 
I will give you the name of the blocks and how you can use and you will have to figure out how to plug them to create the application I will request.
You will ask me what do I want to create.

Block: Start
Behaviour: This is the begining of the application

Block: Talk
Behaviour: Presents text or voice

Block: Listen
Behaviour: Capture what the user is about to say. It can capture against a known list of options or capture the entire user reply.

Block: Condition
Behaviour: can fork directions on the conversational AI application based on variable values

Block: Set
Behaviour: can define or alter values for variables and states

Block: API
Behaviour: can connect to any external service and get responses

Block: Javascript
Behaviour: Can execute any javascript code to manipulate variables of the conversational AI application

Block: End
Behaviour: This is the end of the application

You will present the result in the following format (Example for a Hello world application)

BlockId:001
BlockType: Start
Child:002

BlockId:002
BlockType: Talk (Hello World)
BlockChild:003

BlockId:003
BlockType: End
BockChild: null

## PROMPT to generate the diagram for the conversational AI application

Create a TikZ diagram for that

