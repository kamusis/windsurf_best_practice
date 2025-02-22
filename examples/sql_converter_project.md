# SQL Converter Project Documentation

## Project Objectives

1. Create an open-source Python program that:
   - Uses AI models and ANTLR grammar trees
   - Analyzes SQL from various databases
   - Rewrites SQL into different database formats

2. Design repository structure following best practices:
   - Easy to understand for GitHub users
   - Attractive to Python programmers
   - Potential for high GitHub stars

## Clarifying Questions and Answers

### Scope and Scale
- **Q:** Focus solely on Oracle-to-PostgreSQL or design for extensibility?
  **A:** Not limited to Oracle-to-PostgreSQL
- **Q:** Expected SQL complexity?
  **A:** Complex single SQL and stored procedures

### AI Integration
- **Q:** Specific AI model?
  **A:** OpenAI-compatible model (user will handle)
- **Q:** Include model training?
  **A:** No, keep as separate service

### Library Design
- **Q:** Abstraction level?
  **A:** Three main libraries:
  1. SQL Segmentation
  2. SQL Rewriting (includes segmentation)
  3. Test Case Generation
- **Q:** Include CLI tools?
  **A:** Yes, alongside libraries

### Repository Structure
- **Q:** Example implementations/demos?
  **A:** CLI tools as examples
- **Q:** Documentation level?
  **A:** API docs and tutorials
- **Q:** Contribution guidelines?
  **A:** Only issue templates

### Performance
- **Q:** CI/CD pipelines?
  **A:** No
- **Q:** Performance expectations?
  **A:** Focus on correctness first
- **Q:** Benchmarking tools?
  **A:** Yes

## Designed Repository Structure

```
sql-converter/
├── src/
│   ├── segmentation/        # SQL segmentation library
│   ├── rewriting/           # SQL rewriting library
│   ├── testing/             # Test case generator
│   └── cli/                 # Command line interface
├── benchmarks/              # Performance benchmarking
├── docs/                    # API documentation and tutorials
├── issue_templates/         # GitHub issue templates
├── examples/                # Example usage (via CLI)
├── requirements.txt         # Python dependencies
├── LICENSE                  # Open source license
└── README.md                # Project overview
```

## Core Components Overview

1. **SQL Segmentation Library**
   - Input: SQL text
   - Output: Tokenized SQL components
   - Features: ANTLR grammar parsing, syntax validation

2. **SQL Rewriting Library**
   - Input: SQL text
   - Output: Converted SQL text
   - Features: 
     - Database-specific rule engine
     - AI integration for semantic analysis
     - Error handling and validation

3. **Testing Case Generator Library**
   - Input: SQL text
   - Output: Test cases
   - Features:
     - AI-generated test scenarios
     - Edge case detection
     - Result verification
