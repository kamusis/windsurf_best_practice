# Cascade Tools Usage Guidelines

## **General Rules**
1. **Tool Selection**: Use the appropriate tool for the task. For example:
   - Use `Codebase Search` for finding relevant code snippets.
   - Use `Run Command` for executing terminal commands.
   - Use `Edit File` or `Write File` for modifying or creating files.
2. **Tool Calls**: Always follow the tool schema exactly. Provide all necessary parameters and avoid calling unavailable tools.
3. **Safety**: Never auto-run unsafe commands (e.g., deleting files, installing system dependencies). Always prioritize safety.

## **Common Tools and Use Cases**
1. **Codebase Search**:
   - Use to find code snippets by semantic search.
   - Example: Search for a specific function or class definition.
2. **Edit File**:
   - Use to modify existing files.
   - Example: Add a new function or update a configuration.
3. **Find**:
   - Use to search for files or directories using glob patterns.
   - Example: Locate all `.py` files in a directory.
4. **Grep Search**:
   - Use to search for specific patterns within files.
   - Example: Find all occurrences of a variable name.
5. **List Directory**:
   - Use to list the contents of a directory.
   - Example: Check the files and subdirectories in a project folder.
6. **Read URL Content**:
   - Use to fetch content from a web URL.
   - Example: Retrieve documentation or API responses.
7. **Run Command**:
   - Use to execute shell commands.
   - Example: Run `npm install` or `python manage.py migrate`.
8. **Search Web**:
   - Use to perform web searches.
   - Example: Find relevant documentation or tutorials.
9. **View Code Item**:
   - Use to view specific code items (e.g., functions, classes).
   - Example: Inspect the implementation of a function.
10. **View File**:
    - Use to view the contents of a file.
    - Example: Read a configuration file or script.
11. **View Web Document Content Chunk**:
    - Use to view specific chunks of web content.
    - Example: Read a section of a long webpage.
12. **Write File**:
    - Use to create and write to new files.
    - Example: Generate a new configuration file or script.

## **Best Practices**
1. **Explain Changes**: Before making code changes, briefly describe what you’re doing and why.
2. **Ensure Runnability**: Always include necessary imports, dependencies, and configurations to make code immediately runnable.
3. **Use Logging**: Add descriptive logging and error messages to help with debugging.
4. **Test Changes**: Use test functions or commands to verify changes.
5. **Stay Organized**: Keep code modular, well-documented, and easy to maintain.

---

# **Explicit Tool Requests Guideline**

To explicitly instruct Cascade to use a specific tool, describe the task you want to accomplish in a way that naturally aligns with the tool's purpose. Here’s how you can phrase it:

## **Examples of Explicit Tool Requests**
1. **Codebase Search**:
   - "Search the codebase for the `calculate_total` function."
   - "Find all occurrences of the `User` class in the project."

2. **Edit File**:
   - "Edit `config.py` to add a new configuration setting."
   - "Update the `main.py` file to include error handling."

3. **Find**:
   - "Find all `.js` files in the `src` directory."
   - "Locate the `README.md` file in the project."

4. **Grep Search**:
   - "Search for the string `DEBUG_MODE` in all `.py` files."
   - "Find all occurrences of the word `error` in the `logs` directory."

5. **List Directory**:
   - "List the contents of the `templates` directory."
   - "Show all files and subdirectories in the `public` folder."

6. **Read URL Content**:
   - "Read the content from `https://example.com/api/docs`."
   - "Fetch the content of the GitHub repository page."

7. **Run Command**:
   - "Run `pip install -r requirements.txt` in the terminal."
   - "Execute `npm start` to start the development server."

8. **Search Web**:
   - "Search the web for Python Flask documentation."
   - "Find tutorials on React state management."

9. **View Code Item**:
   - "Show the implementation of the `process_data` function."
   - "View the `User` class definition in `models.py`."

10. **View File**:
    - "Display the contents of `settings.json`."
    - "Show the first 50 lines of `index.html`."

11. **View Web Document Content Chunk**:
    - "View the second chunk of content from `https://example.com/docs`."
    - "Read the third section of the article at `https://example.com/blog`."

12. **Write File**:
    - "Create a new file `utils.py` with a helper function."
    - "Write a configuration file `config.yaml` with default settings."

## **Key Points**
- Be specific about the task and the tool’s purpose.
- Avoid directly naming the tool; instead, describe the action you want to perform.
- Cascade will automatically select the appropriate tool based on your request.
