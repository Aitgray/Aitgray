# About Me (Introduction)
My name is Aidan, I recently obtained my Master's in Computer Science and I'm looking for a job. I'm a tech enthusiast, I love building tools that make my life and the lives of people around me easier[...] 

## My Skills at a Glance
I do most of my development in Python, though I've also worked with C++ fairly regularly over the course of my education. I've used PyTorch and Scikit-learn for my AI/ML classes and projects, matplotl[...] 

## My Projects
I have a number of projects that I've completed; some I can't reveal due to requests by professors, so I've included my most notable publically available projects.

### Past
A few of my most notable projects, with links included, of course.

#### KVALD
KVALD was written to close a gap I noticed in the literature and tooling around glare handling: while glare classification algorithms and theoretical glare-blocking pipelines existed, there wasn't a f[...] 

At a technical level KVALD combines classical image pre-processing with modern convolutional neural networks (CNNs) for segmentation and classification. The pipeline looks roughly like this:
- Input: camera image(s) from a windshield-mounted sensor.
- Pre-processing: exposure correction, denoising, and simple geometric normalization.
- Glare detection & segmentation: a CNN-based model trained to produce a per-pixel mask for bright, specular glare regions (we experimented with U-Net-style architectures and lightweight encoders for [...]
- Post-processing: morphological filtering and temporal smoothing to reduce flicker.
- Output: a binary/soft mask suitable for a dimming/actuator interface or for rendering an overlay.

Implementation notes and technologies:
- Models: CNN-based segmentation (U-Net variants, lightweight encoders); classification heads for distinguishing glare from legitimate highlights.
- Frameworks: PyTorch for model development and training; NumPy/pandas for data handling; OpenCV for pre/post-processing and visualization.
- Training: a mix of synthetic data and curated real-world captures; augmentation (exposure shifts, motion blur, noise) to improve robustness; loss functions included binary cross-entropy with Dice/Io[...]
- Deployment considerations: model quantization and ONNX export for embedded inference; latency and robustness were primary constraints with a focus on keeping inference fast enough for near real-time[...]
- Evaluation: IoU, precision/recall on held-out captures, and qualitative driving tests to verify visibility improvements.

Why it mattered: integrating a reliable, low-latency glare-masking pipeline into a smart windshield can materially improve driver comfort and safety by reducing momentary blindness from specular refle[...] 

#### Cloud Comparison
This is the documented result of a course project comparing cloud storage options for a CSE239 assignment. The original material lives in the repository https://github.com/char26/cse239-cloud-storage [...]

Summary (short):
- Goal: Compare cloud object storage options (pricing models, performance characteristics, and common trade-offs) for typical student workloads and simple backups.
- What I produced: A structured report (LaTeX) with experimental methodology, measured/collected results, and discussion of trade-offs that matter for small teams and research groups.
- Useful for: Anyone deciding between a low-cost archival solution and a frequently-accessed research dataset store; good background material for budgeting and simple performance expectations.

#### Scada Generator
Our Scada Generator started as a research-oriented experiment exploring how to generate or model network/SCADA-like datasets for testing anomaly detection pipelines. The working notebook and generator[...]

Summary:
- Goal: Provide a reproducible generator for SCADA-like (industrial control) time-series data so that anomaly detection and monitoring models can be developed without access to proprietary datasets.
- What I produced: A validation and analysis pipeline to measure the success of our project and generate key figures to aid in our analysis. The validation pipeline performed both static and ML-based [...]
- Tech: Jupyter Notebook, Python ecosystem for numerical work (NumPy/pandas/plotting in the notebook).

#### Scarab (Scarab simulator / 220_lab3)
A cycle-accurate, research-oriented multicore simulator I worked on as part of a systems/architecture lab (repository: https://github.com/Aitgray/220_lab3).

What I contributed:
- Implemented and integrated a perceptron-based branch predictor into the Scarab codebase (C/C++), including data structures, prediction/update logic, and hooks into Scarab's prediction and recovery interfaces.
- Compared the perceptron predictor's accuracy and behavior against several contemporary and legacy predictors (e.g., TAGE-SC-L, gshare and other configured predictors in Scarab), producing quantitative results and analysis.
- Worked within a large, mature simulator codebase: navigated existing predictor interfaces (bp_table, bp_conf, op/op_info), added configuration knobs, and ensured correct interactions with on-path/off-path state and recovery.
- Evaluation: ran Scarab experiments (PARAMS and benchmarks) to measure misprediction rate, confidence estimation when applicable, and trade-offs between accuracy and storage/latency.

Why it mattered:
- Demonstrates ability to make targeted, non-trivial contributions inside a complex C/C++ research codebase while producing measurable evaluation results; shows practical systems-level engineering and experimental skills.

### Present
BardBot - My pride and joy  
I run a DnD campaign with some friends from high school as a way to stay connected. After a few months of writing summaries by hand, I had the idea that there must be a better way, and so the first it[...] 

The second iteration was a relatively simple fix: I made a local version of the bot that would skip over Azure's services and use locally running open-source transcription models instead. This change [...]

Having graduated, I finally had some time to devote to the project, and I came back to exceptional news — the dependency was fixed! Having recently taken a class on Cloud Computing, I decided to mak[...]

Current tools and stack:
- Whisper for transcription (open-source/locally hosted)
- Llama 3.1 (local LLM for summarization/assistant functions)
- Python, Discord.py, Docker for deployment

### Future
Homelabbing:
- Personal NAS running TrueNAS
- Self-hosted email server via Proton
- Self-hosted everything else I can reasonably maintain

## Employment
I am actively seeking roles related to Systems Engineering, Software Engineering, and Infrastructure. I'm particularly interested in positions where I can combine systems-level thinking with practical[...]

Contact: You can reach me via GitHub or drop a line on my profile — happy to share more detailed write-ups, CV, or live demos on request.


(End of file)
