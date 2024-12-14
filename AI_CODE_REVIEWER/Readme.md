# **AI Code Reviewer**

This project implements an **AI-powered code reviewer** using Google's Gemini AI model. The application allows developers to input their Python code, and the AI provides detailed feedback on the code's quality, functionality, security, efficiency, readability, and more.

## **Features**

- **Code Review**: Analyze Python code for issues such as bugs, security vulnerabilities, performance bottlenecks, and readability problems.
- **Feedback**: Receive actionable feedback with suggestions for improvement, including fixed code snippets.
- **Multiline Input**: Users can input multiple lines of code, making it easy to submit larger code blocks for review.
- **Customizable**: Tailor feedback based on the developer's skill level (beginner or advanced).

## **Requirements**

- **Python 3.7 or higher**
- **Streamlit**
- **google-generativeai** library (for connecting to the Gemini AI model)
- **API key** for Google Gemini AI

## **Installation**

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/ai-code-reviewer.git
   cd ai-code-reviewer
