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
   git clone https://github.com/Vidhyalakshmib1305/ai-code-reviewer.git (change it accordingly to your username and repository)
   cd ai-code-reviewer

2. **Set up a virtual environment (optional but recommended)**:
   ```bash
   python -m venv .env
   source .env/bin/activate  # On Windows use `.env\Scripts\activate`

3. **Install dependencies**:
   ```bash
   pip install -r requirements.txt

4. **Get your Gemini API key**:
   - Sign up for access to Google Gemini AI and obtain an API key.
   - Save your API key in a file named `gemini_api.txt` under the `keys/` directory in your project folder.

# **Usage**

1. **Run the Streamlit app**:
   ```bash
   streamlit run app.py

2. **Open the application**:
- After running the command, open your browser and navigate to the address shown in the terminal (usually http://localhost:8501).

3. **Enter your Python code**:
   - In the input box, paste your Python code that you want to be reviewed.
   - Click the "Generate" button to receive feedback from the AI.

4. **Review the feedback**:
   - The AI will provide structured feedback, highlighting bugs, performance improvements, and security vulnerabilities, along with suggestions for improvement.

# **Example Input**
      python
      
      def sub(a, b):     
          return a - b  
      print(add(5, '10'))

# **Example Output**


## **Bug Report**:

## **Issue**: 
The function add() is called, but it is not defined.

## **Impact** :
This will raise a NameError because the function add() is not available in the scope.

## **Suggestions for Improvement** : 
Define the add() function or replace it with the correct function.

## **Educational Tip** : 
Provide additional tips to understand deeper about the concepts.

## **Fixed Code** :
      python
      
         def sub(a, b):     
             if isinstance(a, int) and isinstance(b, int):         
                  return a - b     
             else:         
                  return "Invalid input types"


## **Contributing**:
Feel free to fork the repository and submit pull requests if you want to contribute to the project. We welcome improvements and bug fixes!

## **License**:
This project is licensed under the MIT License - see the LICENSE file for details.
