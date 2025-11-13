# WordBloom

WordBloom is an AI-powered blog generator that transforms simple topics into comprehensive, well-structured blog posts. Built using LangChain and LangGraph frameworks with Groq's fast inference capabilities.

Built With

LangChain: Framework for developing applications with language models
LangGraph: State management and workflow orchestration
Groq: High-performance LLM inference
Python: Core programming language
FastAPI: Web framework for API endpoints

Getting Started

Prerequisites

Python 3.8+
Groq API key

Installation

1. Clone the repository
2. Install dependencies: pip install -r requirements.txt
3. Set up your Groq API key in environment variables
4. Run the application: python app.py

What It Can Do

WordBloom takes a simple blog topic as input and generates:

Structured Content: Well-organized blog posts with clear sections
SEO-Optimized: Content designed for search engine visibility
Multiple Formats: Supports various blog styles and tones
Fast Generation: Leverages Groq's optimized inference for quick results
Customizable Output: Adjustable length, style, and target audience
Multi-Language Support: Generate blogs in English, Hindi, and French

New Features

Multi-Language Blog Generation

Generate blog content in multiple languages:
- English: Default language for professional and casual content
- Hindi: हिंदी में ब्लॉग पोस्ट जेनरेट करें
- French: Générez des articles de blog en français

Language-Specific Optimization

Each language output is optimized for:
- Native language SEO keywords
- Cultural context and tone
- Proper grammar and syntax
- Regional audience preferences

Architecture

The application uses a graph-based architecture with distinct nodes:

Blog Node: Handles content generation logic
State Management: Maintains workflow state throughout generation
LLM Integration: Interfaces with Groq models for text generation
Language Detection: Automatically detects and processes language preferences

API Usage

Send POST requests to generate blog content:

{
  "topic": "Your blog topic here",
  "style": "professional",
  "length": "medium",
  "language": "english"
}

Supported Languages

{
  "topic": "आपका ब्लॉग विषय",
  "style": "professional", 
  "length": "medium",
  "language": "hindi"
}

{
  "topic": "Votre sujet de blog",
  "style": "professional",
  "length": "medium", 
  "language": "french"
}

The system processes the request through its graph workflow and returns a complete blog post ready for publication in the specified language.
