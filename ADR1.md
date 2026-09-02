# ADR 1: Selection of Tech Stack for Basic AI Agent

## Context

We are building a basic AI Agent as part of the AI-Augmented Workflow course.

The AI Agent will accept user input, send the request to an AI model, and return an appropriate response.

The project is designed for a beginner student, so the technology should be easy to learn, simple to implement, well documented, and compatible with AI-assisted coding tools such as GitHub Copilot.

The project should also be flexible enough to support future features such as memory, tools, databases, and web applications.

Positive Consequences
Python offers a simple and easy-to-understand environment for developing AI-based applications.
The OpenAI API makes it convenient to integrate intelligent features into software projects.
Python supports numerous libraries and frameworks that simplify AI, automation, and data-processing tasks.
GitHub Copilot helps developers by suggesting code, identifying errors, explaining programs, and supporting debugging.
Git and GitHub provide an organized way to maintain source code, track changes, and showcase project progress.
The system can be enhanced in the future by adding databases, memory, external tools, and Retrieval-Augmented Generation (RAG).
Ollama can be considered as a future option for experimenting with locally hosted and open-source AI models.
Negative Consequences
Applications using the OpenAI API generally need an active internet connection to communicate with the service.
API services can have usage restrictions, quotas, or charges depending on the selected plan and usage.
API credentials are sensitive and must be stored safely rather than exposing them in public repositories such as GitHub.
Local AI solutions such as Ollama can demand considerable RAM, storage, and processing power depending on the model.
AI-based coding tools may sometimes produce inaccurate or unsuitable solutions, so generated code should always be checked, tested, and corrected before use.

AI-Assisted Development

GitHub Copilot will be utilized as a supportive AI tool throughout the software development process. It will assist the student in improving productivity and understanding different programming tasks.

It will be mainly used for:

Creating and suggesting Python program structures.
Providing explanations for complex or unfamiliar programming concepts.
Identifying possible errors and recommending suitable fixes.
Assisting in the preparation of software test cases.
Suggesting cleaner and more efficient coding approaches.
Helping prepare comments and technical documentation.

Any code or suggestions provided by the AI tool will be carefully examined by the student. The generated code will be understood, manually reviewed, tested, and modified wherever necessary before it is integrated into the final project.

This AI-assisted approach demonstrates how human knowledge and decision-making can be combined with AI tools to develop software more efficiently while maintaining accuracy and reliability.

Alternatives Considered
Java

Java was evaluated as one of the possible technologies for building the AI Agent. However, Python was chosen because it offers simpler programming syntax and has extensive support for Artificial Intelligence, Machine Learning, and automation.

JavaScript / Node.js

JavaScript with Node.js can also be used to develop AI-enabled applications and handle API-based communication. Nevertheless, Python was preferred due to its straightforward learning curve and wide range of AI-related libraries and tools.

Ollama as an Alternative

Ollama was considered as another approach because it allows AI models to be executed locally without depending entirely on cloud-based services.

For the initial version of the project, the OpenAI API was selected because it provides an easier and more practical way to understand AI model integration and API-based development. Ollama may be explored in future versions if local model execution is required.

Security Considerations

Security will be given importance throughout the development and maintenance of the project. The following measures will be implemented:

API credentials will be stored separately from the application source code.
Sensitive keys and authentication details will never be committed to public GitHub repositories.
Environment variables will be used to manage confidential settings and configuration values.
A local .env configuration file can be used during development to keep credentials separate.
The .env file will be excluded from version control through the .gitignore file.
Any code generated or suggested by AI tools will be checked, tested, and validated before implementation.
All external libraries and project dependencies will be properly recorded to improve maintainability and security.
Regular checks will be performed to ensure that confidential information is not accidentally exposed in the project files.

Future Improvements

The proposed AI Agent can be further enhanced with additional features to make it more intelligent, flexible, and useful. Possible future enhancements include:

Adding memory to retain relevant information from previous interactions.
Integrating external tools and functions to perform specific tasks automatically.
Providing controlled web-search functionality for accessing updated information.
Connecting the system with databases for storing and retrieving useful data.
Implementing Retrieval-Augmented Generation (RAG) for better responses based on external documents or knowledge sources.
Developing a user-friendly web interface for easier interaction with the AI Agent.
Exploring locally hosted AI models through platforms such as Ollama.
Introducing automated testing to improve the reliability of the application.
Adding detailed logging and monitoring features to track system activities and errors.
Developing multi-step workflows where the AI Agent can complete complex tasks through a sequence of actions.

Decision Summary

The initial development of the AI Agent will use Python, OpenAI API, GitHub, and GitHub Copilot as the primary technology stack. This combination offers an accessible development environment, strong AI support, easy version control, and useful AI-assisted programming features, making it appropriate for developing a beginner-friendly AI Agent.

Ollama will be kept as a potential future option for testing and implementing locally running open-source AI models.

Status Review

The current status of this Architecture Decision Record (ADR) is Proposed.

It will be moved to Accepted once the selected technologies have been configured successfully and the basic AI Agent has been implemented, tested, and demonstrated successfully.
