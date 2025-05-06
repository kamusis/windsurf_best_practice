# Tool Usage Guidelines

## 1. Strategic Tool Selection
- Analyze codebase and user intent thoroughly before choosing tools
- Select the most appropriate tool for each specific task
- Avoid unnecessary tool calls
- Gather sufficient information before tool selection
- When attempting to read a file's contents, always attempt to read 200 lines of code at once. 

## 2. Efficient Information Gathering
- Plan to collect all necessary data in a single step
- Avoid multiple calls for the same information
- Use tools purposefully and efficiently

## 3. Focused Code Changes
- Make precise, targeted modifications
- Avoid broad, exploratory edits
- Anticipate the impact of each change
- Ensure every tool call contributes meaningfully

## 4. Tool Categories
### Code Exploration & Analysis
- codebase_search: Semantic search for relevant code
- view_code_item: View specific code definitions
- view_file: Inspect file sections
- grep_search: Exact pattern matching
- find_by_name: File/directory search
- list_dir: Directory listing with details

### Code Modification & Creation
- edit_file: Precise code changes
- write_to_file: Create new files

### Execution & Monitoring
- run_command: Execute terminal commands
- command_status: Monitor command status

### Context & Research
- search_web: Web searches
- read_url_content: URL content retrieval
- view_web_document_content_chunk: Web document chunks

### Memory & Context Management
- create_memory: Manage persistent memories
