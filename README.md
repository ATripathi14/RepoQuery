# RepoQuery

**An AI-powered codebase search and question-answering tool that helps developers understand software repositories.**

RepoQuery aims to help developers explore unfamiliar codebases, locate relevant implementation details, and understand how different parts of a project work together.

The project is being developed incrementally, starting with basic repository inspection and keyword search before progressing toward semantic retrieval and Retrieval-Augmented Generation (RAG).

## Problem Statement

Understanding an unfamiliar codebase can require manually searching files, following function calls, reading documentation, and tracing execution flows.

RepoQuery aims to simplify this process by allowing developers to ask questions about a repository and receive answers grounded in relevant source code and documentation.

## Objectives

- Discover and inspect files within a local Git repository.
- Search source code and documentation using keywords.
- Identify relevant code sections and their locations.
- Explore strategies for splitting source code into searchable chunks.
- Implement semantic retrieval using embeddings.
- Generate context-grounded answers using an LLM.
- Provide source references so developers can verify answers.
- Evaluate retrieval quality and improve reliability through testing.

## Initial Scope

The first version will focus on understanding repository structure and implementing a basic search system.

The initial development stages are:

1. Repository and filesystem inspection.
2. File filtering and safe text extraction.
3. Keyword search with file paths and line numbers.
4. Code chunking and metadata extraction.
5. Semantic search using embeddings.
6. Retrieval-Augmented Generation (RAG).
7. Source references and retrieval evaluation.

These stages describe the intended development direction. Features will be marked as implemented only after they have been developed and tested.

## Test Repository

**DevMentor-AI** will serve as the primary test repository during development.

Repository: https://github.com/ATripathi14/DevMentor-AI

Using a familiar, actively developed codebase will help evaluate whether RepoQuery can locate relevant implementation details, explain component interactions, and identify appropriate source files for real developer questions.

Example questions include:

- Where is the `/analyze` endpoint implemented?
- How does the application handle local service connection failures?
- Where is error fingerprinting implemented?
- How does the application prevent repeated error notifications?

DevMentor-AI is a test input for RepoQuery, not a dependency of the RepoQuery package itself.

## Intended Workflow

The planned question-answering workflow is:

1. Select a local repository.
2. Discover and filter relevant files.
3. Extract and process source code and documentation.
4. Retrieve code sections relevant to a user's question.
5. Construct context from the retrieved information.
6. Generate an answer using an LLM.
7. Present source references for verification.

The initial implementation will establish a keyword-search baseline before introducing semantic retrieval and generation.

## Technology Direction

- **Python** — primary programming language.
- **Git** — source control and repository management.
- **Embeddings** — semantic representation of code and queries.
- **Vector search** — retrieval of semantically relevant content.
- **LLMs** — natural-language explanations grounded in retrieved context.
- **Testing and evaluation** — measurement of correctness and retrieval quality.

Specific frameworks, models, and storage technologies will be selected as implementation requirements become clear.


## Project Status

**Status: Early development — requirements and fundamentals.**

Repository inspection, keyword search, semantic retrieval, and RAG are planned development stages. Their implementation status will be updated as the project progresses.

## License

See the [LICENSE](LICENSE) file for licensing information.