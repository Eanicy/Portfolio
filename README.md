# Project Portfolio

## Edwin N. Allanic Jr.

I’m a Computer Science student who enjoys turning ideas into practical, responsible AI applications. From making research assessment more evidence-based to helping farmers identify crop diseases and exploring earthquake detection through video, I build projects that connect technology with real-world needs. I’m always learning, experimenting, and excited to create useful solutions through web development, machine learning, and computer vision.

## Featured Projects

| Project | Focus | Highlights |
| --- | --- | --- |
| [CapstoneLens](https://github.com/Eanicy/CapstoneLens) | Evidence-grounded capstone assessment | Laravel, OpenAlex, local LLM, NLP Machine Learning |
| [CornDoctor](https://github.com/Eanicy/Corn-Leaf-Disease-Classifier) | Offline crop-disease recognition | Flutter, image classification, transfer learning |
| [SeismoWatch](https://github.com/Eanicy/Earthquake_Detection) | CCTV-based earthquake-shake detection | PyTorch, FastAPI, React, video classification |

---

## CapstoneLens

**An evidence-grounded platform for reviewing capstone proposals and managing a protected manuscript repository.**

**Role:** Developer - implemented the LLM/RAG assessment workflow and similarity-model capabilities.

CapstoneLens supports structured student proposal submissions, short pitch-video processing, qualitative assessment, and role-based academic workflows. Rather than presenting a numeric novelty score, it produces reasoned findings on novelty, technical depth beyond CRUD, scope, and team capacity.

### What it does

- Accepts structured proposals and verifies that a final MP4, WebM, or MOV pitch is three minutes or less.
- Transcribes pitch videos and uses English translations when available, while keeping pitch-derived evidence explicitly labelled.
- Retrieves and compares evidence from OpenAlex and published local manuscripts as separate sources.
- Ranks up to 100 candidate sources per collection, provides the strongest evidence to the assessment flow, and preserves lower-ranked results for review.
- Uses proposal-aware extractive evidence selection to keep relevant source excerpts concise and auditable.
- Runs qualitative generation through a local, OpenAI-compatible `llama.cpp` runtime, with validation, retry, and deterministic fallback behavior.
- Enforces role-aware access for students, faculty, and administrators; private files remain outside the public web root.

### Stack

`Laravel` · `PHP 8.3+` · `SQLite` · `Node.js` · `FFmpeg` · `Poppler` · `OpenAlex` · `llama.cpp` · `Qwen3`

### Thoughtful constraints

The assessment deliberately avoids judging appearance, accent, confidence, voice quality, or pitch-production quality. It also treats missing search results as insufficient evidence—not proof of novelty—and sends only minimal technical search terms to OpenAlex.

---

## CornDoctor

**A mobile app that identifies common corn-leaf diseases from photos, even without an internet connection.**

**Role:** Sole developer - led the project end to end, including model development, mobile-app implementation, and deployment workflow.

CornDoctor makes plant-health screening more accessible: users photograph a corn leaf or choose an image from their gallery, then receive an on-device classification and disease guidance. The app covers healthy leaves, Common Rust, Blight, and Gray Leaf Spot.

### Highlights

- Trained on **4,188** corn-leaf images across four classes.
- Reported held-out test accuracy: **93.64%**.
- Delivers a diagnosis in under one second and works offline.
- Rejects low-confidence results below 60% and prompts for a clearer image to reduce unreliable classifications.
- Includes an in-app AI chat experience for treatment and prevention questions.
- Provides a reproducible path for retraining a custom model and converting it for mobile deployment.

### Stack

`Flutter` · `Python` · `PyTorch` · `Transfer Learning` · `TensorFlow Lite`

### Practical use

The experience is designed around real field conditions: clear, well-lit photos of actual corn leaves work best; blurry, dark, non-corn, or screen-photographed images are flagged instead of being treated as reliable diagnoses.

---

## SeismoWatch

**A proof-of-concept system that estimates earthquake-shake intensity from CCTV video.**

**Role:** Sole developer - led the project end to end, from data preparation and model training through backend, frontend, and user experience implementation.

SeismoWatch analyzes camera motion in uploaded CCTV clips and classifies the observed shaking as stable, low, medium, or violent. When an earthquake event is detected, the web interface surfaces a map heatmap and sends a notification.

### Highlights

- Uses **R(2+1)D-18**, pretrained on Kinetics-400, for four-class video classification.
- Processes 16-frame clips at 112 × 112 resolution.
- Achieved a best validation accuracy of **63.38%** using 992 training videos.
- Combines 32 real stable CCTV clips from Cebu City with 960 augmented clips representing low, medium, and violent shake.
- Simulates realistic multi-frequency sinusoidal camera motion with OpenCV for augmentation.
- Includes a FastAPI inference backend and a React + Leaflet interface with camera selection, upload, event log, map overlay, and notifications.

### Stack

`Python 3.11` · `PyTorch` · `OpenCV` · `FastAPI` · `Uvicorn` · `React` · `Leaflet`

### Known limitations

This is a research prototype. Its synthetic augmentations may not fully reflect real earthquake footage; camera shake can also come from non-earthquake sources such as traffic or machinery; and the medium-intensity class is currently the most difficult to distinguish.

---

## Skills Demonstrated

- Web application design and role-based workflow implementation
- Retrieval-augmented, evidence-grounded AI workflows
- Local/offline model deployment and privacy-aware system design
- Image and video classification with deep learning
- Dataset preparation, augmentation, model evaluation, and deployment pipelines
- Mobile development and interactive geospatial web interfaces

## Certifications

### Fortinet Training Course Completions

- **NSE 1 - Cybersecurity and Cloud Fundamentals 1.0** - completed October 15, 2026
- **NSE 2 - Introduction to Next Generation Firewall 1.0** - completed October 16, 2026
- **NSE 3 - FortiGate 7.6 Operator Self-Paced** - completed October 16, 2026


## Explore the Work

- [CapstoneLens repository](https://github.com/Eanicy/CapstoneLens)
- [CornDoctor repository](https://github.com/Eanicy/Corn-Leaf-Disease-Classifier)
- [SeismoWatch repository](https://github.com/Eanicy/Earthquake_Detection)
map are particularly strong candidates because they make the result understandable at a glance.

## Contact

I’m interested in building useful, responsible applications at the intersection of AI and real-world decision-making. Feel free to explore the project repositories or get in touch through the links on my GitHub profile.
