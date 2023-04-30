# tta
## Text-to-Assistant

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

