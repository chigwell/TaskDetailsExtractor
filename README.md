[![PyPI version](https://badge.fury.io/py/TaskDetailsExtractor.svg)](https://badge.fury.io/py/TaskDetailsExtractor)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![Downloads](https://static.pepy.tech/badge/taskdetailsextractor)](https://pepy.tech/project/taskdetailsextractor)

# TaskDetailsExtractor

`TaskDetailsExtractor` is a Python tool designed to interact with GPT-3 in order to extract detailed task instructions based on a given coding task and project details. It integrates with OpenAI's GPT-3 API to analyze the feasibility of a task and to detail the necessary file operations to complete it.

## Installation

To install `TaskDetailsExtractor`, you can use pip:

```bash
pip install TaskDetailsExtractor
```

## Usage

### As a Python Module

TaskDetailsExtractor can be used as a Python module in your scripts for interacting with GPT-3 to analyze coding tasks.

Example:

```python
from taskdetailsextractor import TaskDetailsExtractor

# Initialize the extractor with the target project directory and your OpenAI API key
extractor = TaskDetailsExtractor('/path/to/your/project', 'your-openai-api-key')

# Example of analyzing task details
task_description = "Refactor the database schema to improve performance."
task_details = extractor.analyze_task_details(task_description)
print(task_details)
```

## Features

- **GPT-3 Integration**: Communicates with OpenAI's GPT-3 to analyze tasks and extract detailed instructions.
- **Task Analysis**: Provides detailed breakdowns of tasks including file operations needed, specific code blocks, and more.

## Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/chigwell/TaskDetailsExtractor/issues).

## License

This project is licensed under the [MIT License](https://choosealicense.com/licenses/mit/).
