# Resume-Preparation-Agent

## Overview
The Resume Preparation Agent is an AI-powered agent designed to analyze, optimize, and tailor resumes for specific job and internship roles. It focuses on ATS keyword optimization, role-specific resume tailoring,
and high-quality bullet-point rewriting while maintaining strict formatting.

This agent is designed to integrate seamlessly into a Multi-Agent AI System.

## Purpose
This agent is responsible for:
- Parsing resumes (PDF / text)
- Extracting relevant skills and keywords
- Performing ATS keyword matching
- Rewriting resume bullet points for impact
- Tailoring resumes for specific roles

## Workflow

Resume (PDF)
    │
    ▼
Text Extraction (pdfminer)
    │
    ▼
Resume Keyword Extraction (spaCy)
    │
    ▼
Job Description Fetch (Google Serper)
    │
    ▼
Job Keyword Extraction (spaCy)
    │
    ▼
ATS Keyword Matching
    │
    ▼
Bullet Point Rewriting (GPT-4o)
    │
    ▼
LaTeX PDF Generation
    │
    ▼
Optimized Resume


## Tech Stack

### LLM
- GPT-4o (primary)
- 
### Frameworks
- LangChain (agent creation and tools)
- LangGraph (workflow orchestration – future integration)

### Libraries
- pdfminer.six – resume parsing
- spaCy – keyword extraction and matching
- Google Serper - To look up current job descriptions/keywords for specific roles
- LaTeX - high-quality PDF generation
