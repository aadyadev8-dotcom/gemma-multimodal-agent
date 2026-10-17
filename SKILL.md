name: gemma-cpp-code-analyzer
description: An Agent Skill that uses Gemma 4 to analyze handwritten code diagrams, flowcharts, and C++ source code to output optimized code and bug reports.
allowed-tools:
  - python-execution

# Gemma C++ Code & Diagram Analyzer Skill

## Overview
This skill instructs an AI agent on how to process text and multimodal image inputs (diagrams, flowcharts, whiteboard code) using the Gemma 4 open model via the Gemini API.

## Instructions
1. Parse the incoming prompt or image file.
2. If an image is provided, identify all visual elements (flowchart decision nodes, handwritten C++ code, or logic diagrams).
3. Translate the visual logic into structured step-by-step pseudo-code.
4. Output production-ready C++ code adhering to modern standards (C++17/C++20).
5. Provide a time complexity analysis ($O(N)$, $O(N \log N)$) and check for common memory bugs.

## Expected Output Format
- **Summary of Input**: Brief breakdown of code/diagram.
- **C++ Implementation**: Clean code block.
- **Complexity Analysis**: Time and space bounds.
