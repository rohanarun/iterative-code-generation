Iterative Code Generation Tester
A browser-based tool that demonstrates AI-powered code generation with visual line-by-line execution testing.

Iterative Code Generation Tester Screenshot

Overview
This tool demonstrates an interactive approach to code generation using Large Language Models (LLMs) through OpenRouter's API. Instead of generating code in one pass and hoping it works, this tool:


Generates complete JavaScript code solutions to user-specified tasks

Visually executes the code line-by-line in real-time

Intelligently identifies real errors versus expected execution artifacts

Automatically fixes genuine code issues by consulting the AI

Features

Two-Phase Generation Process: First generates complete solutions, then tests incrementally

Visual Step Execution: Watch code execute line-by-line with current line highlighting

Intelligent Error Detection: Distinguishes between expected errors in partial execution and real code problems

Automatic Error Analysis & Fixing: Leverages AI to fix identified issues

Adjustable Execution Speed: Control how quickly the code steps through execution

Full Console Output Capture: See all logs, warnings, and errors during execution

Getting Started
Prerequisites

An OpenRouter API key (sign up at OpenRouter.ai if you don't have one)

Any modern web browser

Using the Tool

Clone this repository:

code

git clone https://github.com/yourusername/iterative-code-generation-tester.git

Open index.html in your web browser (no server required)


Enter your OpenRouter API key in the designated field


Type in a description of what you'd like the AI to code, such as:

"Create a function that calculates the Fibonacci sequence"
"Build a simple to-do list with add and remove functionality"
"Write a binary search implementation"

Click "Generate Full Code" to generate the complete solution


Once code is generated, click "Test Line by Line" to watch it execute incrementally


If errors are found, the tool will automatically analyze and attempt to fix them


Adjust the execution speed slider to control the pace of line-by-line testing


How It Works
Code Generation
The tool uses Claude 3.7 Sonnet (through OpenRouter) to generate a complete JavaScript solution to the specified task. A specialized system prompt guides the AI to create well-formed, functional code.

Line-by-Line Testing
After generating the solution, the tool:


Executes the code line-by-line, highlighting the current line

Captures all console output (logs, errors, warnings)

Analyzes any errors to determine if they're:
Expected errors: Natural artifacts of partial execution (like undefined variables that will be defined later)
Real errors: Actual bugs, syntax problems or logic issues

Error Fixing
When real errors are detected:


The complete code and error context is sent back to the AI model

A specialized error-fixing system prompt guides the AI to analyze and fix the issue

The AI returns a fixed version of the code with explanations

The fixed code replaces the original solution

Use Cases

Educational Tool: Learn how code executes line-by-line

Debugging Practice: Understand how to identify and fix common code errors

AI Capabilities Demo: Showcase how AI can generate and fix code interactively

Development Sandbox: Quickly prototype solutions to coding problems

Limitations

Currently only supports JavaScript code execution

Runs in the browser's JavaScript environment, so certain operations may be restricted

Some complex code may not be suitable for line-by-line execution due to scope/closure issues

Relies on heuristics to distinguish expected vs. real errors

Privacy & Security

Your OpenRouter API key is only stored in memory during the current session and is never saved

All code execution happens locally in your browser

API calls are made directly from your browser to OpenRouter

Contributing
Contributions are welcome! Please feel free to submit a Pull Request.

License
This project is licensed under the MIT License - see the LICENSE file for details.

Acknowledgments

This tool uses the OpenRouter API to access Claude 3.7 by Anthropic

Inspired by the potential of AI-assisted programming and debugging workflows

⭐️ If you found this tool helpful, please consider starring the repository!
