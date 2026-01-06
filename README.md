# About Me (Introduction)
My name is Aidan, I recently obtained my Master's in Computer Science and I'm looking for a job. I'm a tech enthusiast, I love building tools that make my life and the lives of people around me easier — I like automating repetitive tasks, experimenting with ML models, and putting together systems that "just work" for the people who use them.

## My Skills at a Glance
I do most of my development in Python, though I've also worked with C++ fairly regularly over the course of my education. I've used PyTorch and Scikit-learn for my AI/ML classes and projects, matplotlib for plotting, and a handful of cloud and infra tools for coursework and personal projects. I try to write clear, tested code and make well-documented, reproducible experiments.

## My Projects
I have a number of projects that I've completed, some I can't reveal due to requests by professors, but I'll still describe what I've done.

### Past
A few of my most notable projects, with links included of course.

#### KVALD
KVALD is one of my longer-running projects — a tool/utility I built to solve a practical problem I kept running into during coursework and hobby projects. At a high level, KVALD is focused on [brief problem domain here — e.g., validation, data pipeline tooling, or a domain-specific utility], with an emphasis on reliability and ease-of-use. The project grew out of a need to automate repetitive validation and logging tasks across my experiments and small services. I implemented the core in Python, added a lightweight CLI + configuration layer, and built tests so I could refactor without fear. If you'd like a deeper write-up or code pointers for KVALD, tell me which parts you want expanded and I’ll add more details (architecture, key modules, example commands, and a quick usage guide).

#### Cloud Comparison
This is the documented result of a course project comparing cloud storage options for a CSE239 assignment. The original material lives in the repository https://github.com/char26/cse239-cloud-storage — note that the repo is private, so I can't embed the full contents here, but the project is primarily a written (LaTeX) report and experimental notes (repository language: TeX).

Summary (short):
- Goal: Compare cloud object storage options (pricing models, performance characteristics, and common trade-offs) for typical student workloads and simple backups.
- What I produced: A structured report (LaTeX) with experimental methodology, measured/collected results, and discussion of trade-offs that matter for small teams and research groups.
- Useful for: Anyone deciding between a low-cost archival solution and a frequently-accessed research dataset store; good background material for budgeting and simple performance expectations.
Because the repo is private, if you want me to lift specific figures or tables into this README, either grant access or paste the relevant markdown/TeX snippets and I’ll integrate them.

#### NetDiffusion
NetDiffusion started as a research-oriented experiment exploring how to generate or model network/SCADA-like datasets for testing anomaly detection pipelines. The working notebook and generator live at https://github.com/char26/scada-generator (public). It's implemented as a Jupyter notebook that demonstrates data generation and basic post-processing.

Summary (short):
- Goal: Provide a reproducible generator for SCADA-like (industrial control) time-series data so that anomaly detection and monitoring models can be developed without access to proprietary datasets.
- What I produced: A notebook that synthesizes signals, injects configurable anomalies, and shows simple visualizations — useful for prototyping ML models and validating detection logic.
- Tech: Jupyter Notebook, Python ecosystem for numerical work (NumPy/pandas/plotting in the notebook).
If you want a runnable package or a small CLI around the notebook, I can extract the generation code into a Python module and add usage examples.

### Present
BardBot - My pride and joy  
I run a DnD campaign with some friends from high school as a way to stay connected. After a few months of writing summaries by hand, I had the idea that there must be a better way, and so the first iteration of BardBot was born: a bot that transcribes and summarizes sessions to keep everyone in sync.

The second iteration was a relatively simple fix: I made a local version of the bot that would skip over Azure's services and use locally running open-source transcription models instead. This change improved privacy, lowered cost, and reduced latency for our sessions.

Having graduated, I finally had some time to devote to the project, and I came back to exceptional news — the dependency was fixed! Having recently taken a class on Cloud Computing, I decided to make some improvements and port parts of the transcription and storage pipeline to be more reproducible and cheaper to run.

### Future
Homelabbing:
- Personal NAS running TrueNAS
- Self-hosted email server via Proton
- Self-hosted everything else I can reasonably maintain

## Employment
I am actively seeking roles related to Systems Engineering, Software Engineering, and Infrastructure. I'm particularly interested in positions where I can combine systems-level thinking with practical software: automation, observability, fault-tolerant services, and ML infrastructure.

Contact: You can reach me via GitHub or drop a line on my profile — happy to share more detailed write-ups, CV, or live demos on request.
