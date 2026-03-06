# 🧬 BioRecruit: The High-Agency ATS
**Automating "Founder Intuition" for High-Intensity Hiring.**
BioRecruit is an AI-powered Applicant Tracking System built specifically for early-stage, YC-backed biotech startups. Unlike traditional ATS platforms that filter by keywords and Ivy League degrees, BioRecruit is engineered to detect "**Agency**" — the ability to get things done permissionlessly.
> Designed for the CEO who has seconds, not minutes.

<img width="1296" height="744" alt="Screenshot 2026-03-06 at 21 04 56" src="https://github.com/user-attachments/assets/34d4ee84-5bc0-43d4-b728-03c9abcae7e2" />

## The Problem
High-profile startups receive thousands of inbound applications. Traditional filters reject "outlier" candidates who:
- Have low formal experience but high trajectory.
- Don't fit the standard "Stanford/MIT" mold but have built impressive things.
- Write incredible cold emails that get lost in the noise.
### The "No False Negatives" Philosophy
If the AI encounters a candidate with low conventional data but high "signal" (or if it's simply unsure), **it does not reject them**. It flags them for Human Review.
Why? Because the best candidates often have non-linear paths. The creator of this app was hired via a cold email that a standard ATS would have blocked.

## The Brain: Two-Channel Scoring
BioRecruit parses both the **CV (PDF)** and the **Cold Email/Application (Context)** simultaneously. It scores candidates on two distinct axes:
1. **The Floor (Formal Qualifications):** Education, hard skills, years of experience.
2. **The Ceiling (Agency & Initiative):** A proprietary "Force of Nature" score based on:
    - **Thesis Alignment**: Does the candidate understand specific internal concepts (e.g., "Computational Sparsification," "MetaTrinity")?
    - **Proactivity**: Did they build something permissionlessly?
    - **Research Depth**: Did they just copy-paste a template, or did they research the CEO's specific papers?
### The "Twist"
The system is **weighted to prioritize Agency over Credentials**. A candidate with a 35% "Formal" score but a 93% "Agency" score is flagged as a "**Strong Yes**", whereas a generic applicant with perfect grades might be auto-rejected.

## Feature Walkthrough
### **1. The "Brutally Honest" AI Analyst**
The AI is prompted to abandon politeness. It acts as a psychoanalyst for the hiring team, flagging:
- **Retention Risks**: "Candidate plans to go to Med School in 2 years."
- **Behavioral Flags**: "Force of nature," "High operational bandwidth."
- **Thesis Mirroring**: Detects if the candidate speaks the internal language of the lab.


<img width="1112" height="645" alt="Screenshot 2026-03-06 at 21 05 13" src="https://github.com/user-attachments/assets/2d2b99d8-c7b8-4389-a1c9-35b37da8c111" />
<img width="1170" height="677" alt="Screenshot 2026-03-06 at 21 05 43" src="https://github.com/user-attachments/assets/0cea742d-2f80-4567-ac0c-6b0f8fafc6b1" />


_Above: The AI breaks down a candidate's profile, explicitly calling out "Outlier cold email" and verifying they understand the CEO's work on "MetaTrinity."_

### **2. The "Swipe-to-Hire" Interface**
- **Tinder-Style Decisioning**: The AI synthesizes the candidate's strengths and weaknesses into a single card.
- **Action**: The CEO swipes Right (Shortlist) or Left (Reject).
- **Velocity**: Reduces hiring time from hours of reading PDFs to minutes of swiping.

![bio](https://github.com/user-attachments/assets/7cf0be71-ef8c-483f-b8ef-a3c6f25dd4db)

### **3. Configurable Weight Matrix**
Founders can adjust the hiring algorithm on the fly. If the role requires pure execution over strategy, the weights can be shifted via sliders, instantly re-scoring the entire pipeline.

<img width="1343" height="775" alt="Screenshot 2026-03-06 at 21 06 05" src="https://github.com/user-attachments/assets/ef9ca782-75a5-4ea4-abd3-35ccbb072514" />

### **4. Post-Match Automation**
The moment the CEO swipes right, BioRecruit takes over:
- **Auto-Logistics**: Automatically composes and sends the invite email via the Gmail API.
- **Scheduling**: Handles link distribution and follow-up, requiring zero manual input from the founder.

### **5. Continuous Learning (RLHF)**
The system gets smarter with every swipe:
- **Feedback Loop**: When the CEO rejects a "High Score" candidate or accepts a "Low Score" one, the model updates its weights.
- **Tailored Values**: The prompt is dynamically injected with the company's specific core values (e.g., "Sparsification," "Operational Bandwidth"), ensuring the AI hunts for your culture, not generic "good employees."

### **6. Pipeline & Analytics**
A Kanban-style view of the funnel, with an auto-reject threshold for low-effort spam, ensuring the Founder only sees the top 10% of high-signal talent.

<img width="1134" height="658" alt="Screenshot 2026-03-06 at 21 06 17" src="https://github.com/user-attachments/assets/713df702-5a87-49b3-944d-0438e029264a" />

## Tech Stack
**Core Architecture**
- **Frontend**: React + Vite (Custom UI System)
- **Packaging**: Electron (Native macOS .dmg build)
- **Database**: Supabase (Real-time vector storage for candidate profiles)

**AI & Logic**
- **Model**: OpenAI GPT-5.2 (via API) — leveraging latest reasoning capabilities for behavioral psychoanalysis of candidates
- **Development**: Backend logic co-architected with Anthropic Claude
- **Techniques**: Custom prompt engineering for behavioral analysis; expanded context window for reading entire portfolios/papers

**Integrations**
- **Input**: Custom PDF Scraper & Raw Text Context Parser
- **Communication**: Gmail API for automated outreach
- (**In Development**): Google Search/Scraping API to verify external candidate links and GitHub repos in real-time

## Roadmap
- **A/B Testing Engine**: Automatically test different application formats to see which yields the highest "Hire Rate."
- **Link Verification**: Real-time scraping of candidate portfolio links to verify claims.

## License & Availability
**Private / Commercial Software**. This project is currently deployed internally. The source code is proprietary. This repository serves as a technical showcase of the architecture and product design.

### 💬 Interested in BioRecruit?

This system is currently in active development and deployed internally. If you're a founder dealing with high-volume hiring and interested in learning more about BioRecruit or exploring a custom deployment, feel free to reach out:

📧 **yas.feraru@gmail.com**  
🔗 [LinkedIn](https://www.linkedin.com/in/yasmyna-feraru)

*Note: Any commercial licensing or deployment would be subject to approval and partnership discussions.*
