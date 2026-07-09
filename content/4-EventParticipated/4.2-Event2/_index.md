---
title: "Event 2"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 4.2. </b> "
---

# Summary Report: "FCAJ Community Day"

### Event Objectives

- Bring together members of the First Cloud AI Journey (FCJ) community to share real project experience
- Provide a space for interns, mentees, and the AWS community to present hands-on work on AI, cloud infrastructure, and product building
- Encourage knowledge exchange across different tracks: prompt/context engineering, AI assistants, cloud architecture, LLM behavior, and product/hackathon experience
- Strengthen networking between interns, mentors, and the wider AWS Study Group community

### Speakers & Sessions

- **Tinh Truong** – Platform Engineer, GoTymeX – "Context Is Everything: Making AI Actually Work for You"
- **Pham Ng. Hai Anh** – AWS Community Builder, G-AsiaPacific Vietnam – "Friendly AI Assistant w/ Amazon Quick"
- **Nguyen Tuan Thinh** – DevOps Engineer, First Cloud AI Journey – "From Edge To Origin: CloudFront as Your Foundation"
- **Team VIB** – "36 hrs with LotusHacks – Building UTMorpho from Idea to Reality"
- **Duc Dao** – Solution Architect, Cloud Kinetics – "Non-Determinism of 'Deterministic' LLM Settings"
- **Vy Lam** – Senior Business Systems Analyst, VPBank – "Enterprise-Grade Multi-Agent System: The Case of Startup Credit Scoring"

### Key Highlights

#### Context Is Everything: Making AI Actually Work for You

- Argued that AI models are already powerful — the missing piece is often the **context** given to the model
- Broke down what "context" actually means: your goal, your data/environment, your constraints, and relevant evidence
- Called out common mistakes when working with AI, such as the "internet pull" problem (the model defaulting to generic internet knowledge instead of your actual context) and repeatedly telling the AI what it already knows

#### Friendly AI Assistant w/ Amazon Quick

- Described how a typical day for business users can be painful without the right AI assistant
- Introduced **Amazon Quick Suite**, AWS's newer offering for building friendly, agentic AI experiences for business users

#### From Edge To Origin: CloudFront as Your Foundation

- Positioned Amazon CloudFront not just as a CDN, but as a **foundation** layer for protecting and optimizing applications
- Walked through common challenges, how CloudFront works, its capabilities around cost, security, resilience, and performance, and real-world use cases/best practices

#### Building UTMorpho in 36 hours at LotusHacks

- Shared the experience of taking a product idea from concept to a working prototype within a 36-hour hackathon
- Highlighted the importance of scoping ruthlessly, dividing tasks across a team, and iterating quickly under time pressure

#### Non-Determinism of "Deterministic" LLM Settings

- Based on research by Atil et al. (2024) from Penn State University & Comcast AI Technologies
- Explained how LLMs choose the next token, and the role of temperature, top-p, and top-k
- Showed why LLM output can still be inconsistent even under settings that seem "deterministic," along with mitigation strategies

#### Enterprise-Grade Multi-Agent System: The Case of Startup Credit Scoring

- Presented the structural mismatch problem in traditional credit-scoring systems when applied to startups
- Presented a case study applying a multi-agent architecture to handle this credit-scoring problem more reliably than a single model

### Key Takeaways

- The context given to an AI matters as much as, sometimes more than, which model is used
- Building an AI assistant for business users is not only a modeling problem — the real workflow and experience of the end user is what actually matters
- Edge and CDN design choices (like CloudFront) have a direct impact on how applications perform for real users
- Even "deterministic" LLM settings can still produce inconsistent output — understanding temperature, top-p, and top-k helps control this better
- Multi-agent architectures are becoming a practical pattern for enterprise use cases that are too complex for a single LLM call
- Hackathon-style constraints (like a 36-hour build) force clearer prioritization and faster decision-making

### Applying to Work

- Pay attention to giving AI tools enough context (goal, data, constraints) when using them to assist with code or documentation during the internship
- Consider CDN-first thinking (CloudFront) when discussing how CloudDoc's frontend is delivered to users
- Keep the non-determinism of LLMs in mind when designing AI-assisted features, instead of assuming output will always be identical
- Keep an eye on multi-agent and AI-assistant patterns as a possible direction for future feature ideas
- Reflect on the LotusHacks approach to scoping and prioritizing when time is limited, and apply the same mindset to sprint-based project work

### Event Experience

Attending **FCAJ Community Day** was a valuable opportunity to see how other interns and community members apply AI, cloud, and product-building skills to real projects outside of my own internship track. Some highlights:

#### Learning from a diverse set of speakers
- Each speaker came from a different background and project context, which gave a broader view of what "building on AWS" can look like beyond my own CloudDoc project.
- The session on LLM non-determinism helped connect some concepts I had only used at a surface level before.

#### Exposure to real project pressure
- The LotusHacks story from Team VIB was a good reminder of how much can be built in a short time when the scope is clear and the team communicates well.
- It also reinforced that a working prototype is more valuable early on than a perfect one.

#### Networking and community connection
- The event created a natural setting to meet other interns and mentors in the FCJ community, which is useful for future learning and collaboration.

#### Event photos

<img src="/images/4-EventParticipated/4.2-Event2/event-2.jpg" alt="Photo from FCAJ Community Day" style="max-width: 90%; height: auto;">

> Overall, FCAJ Community Day gave me a wider perspective on how AI and cloud skills are applied across different teams and projects, beyond the scope of my own internship work.
