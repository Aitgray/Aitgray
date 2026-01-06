# Hi!
## About Me
My name is Aidan, I recently obtained my Master's in Computer Science and I'm looking for a job. I'm a tech enthusiast, I love building tools that make my life and the lives of people around me easier. Maybe some simple examples before I go more into depth, idk yet.
## My Projects
I have a number of projects that I've completed, some I can't reveal due to requests by professors, but I'll still describe what I've done.
### Past
All my projects/repos up until KVALD, which I need to make public
### Present
BardBot - My pride and joy
I run a DnD campaign with some friends from High School, as a way to stay connected. After a few months of writing summaries by hand, I had the idea that there must be a better way, and so the first iteration of BardBot was born. I had been wanted to get some experience working with APIs and cloud services so I signed up for the student trial of Azure. I built a pipeline to record our sessions, send those recordings to Azure's transcription and storage services, and then fetch the transcriptions so I could plug them into ChatGPT. It wasn't without issues, but it worked spectacularly well. I ended up saving an hour or two each week, using AI for it's primary use case: to eliminate menial tasks. The first iteration served me well for a time, but eventually I ran out of credits, so I had to make a change.

The second iteration was a relatively simple fix, I made a local version of the bot that would skip over Azure's services and use locally running open-source transcription models instead. This change was a resounding success, but it came with some drawbacks. Azure's transcription models were quite good, and the models I had running locally weren't quite up to snuff. In addition to that, the library I had been using to capture audio from Discord ended up breaking, due to an update. While I managed to circumvent the issue by recording the audio via OBS, BardBot fell by the wayside and I stopped using it for a time.

Having graduated, I finally had some time to devote to the project, and I came back to exceptional news, the dependancy was fixed! Having recently taken a class on Cloud Computing, I decided to make some much needed improvements to the bot, improving transcriptions, features, and performing some much needed resiliancy improvements. The first change was in the form of a transcriber update, I swapped to OpenAI's Whisper to get more accurate transcripts. I also containerized the bot to resolve some issues with CUDA, but also to enable the next step of my plan: Local LLM integration. In another container I deployed Llama 3.1 8B, so I could send the transcripts directly to my own LLM. I implemented RAG as well, placing my notes into a vector database to ensure the summaries were as accurate as possible. More work still needs to be done of course, but that's where the bot is at currently.
### Future
Homelabbing:
- Personal Nas running TrueNAS
- Self hosted email server via Proton
- Self hosted
## Other Learning
What projects have I worked on that aren't on github?
## Employment
I am actively seeking roles related to Systems Engineering, Software Engineering, and Infrastructure.
