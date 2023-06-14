# Standards

Standards for officiated CSX Labs open-source projects to adhere to.

## Documentation

### README.md

All projects must have a README.md file in the root directory of the project. This file must contain the following information:

- Name
- Brief Description
- User Setup Instructions (if applicable)
- Overview of the project
  - Mission & Vision
  - Problem & Solution
  - Functionality
  - Purpose
  - Current State or Future Directions
- Links to any relevant documentation
- Contact information for the project's maintainer(s)

### REQUIREMENTS.md

If not included in the project's README.md, a REQUIREMENTS.md file must be included in the root directory of the project. This file must contain the following information:

- Mission & Vision
- Functional Requirements
- Non-Functional Requirements
- Technical Requirements
- Security Requirements

### CONTRIBUTING.md

If not included in the project's README.md, a CONTRIBUTING.md file must be included in the root directory of the project. This file must contain the following information:

- Developer Setup Instructions
- Contributing Instructions
- Project Structure
- Project-Specific Standards and Practices
  - Code-Style
  - Documentation
  - Code-Review Process
  - Project Management
- Contact information for the project's maintainer(s)
- Link to the code of conduct

### CODE_OF_CONDUCT.md

All projects must have a CODE_OF_CONDUCT.md file in the root directory of the project.
CSX Labs' projects adopt the [Contributor Covenant](https://www.contributor-covenant.org/) Code of Conduct.

## Code Standards

### Testing

All projects must include a unified test suite that can be run with a single command.
All HTTP endpoints must be mocked and tested, and all user-facing interfaces must be tested.

### Static Analysis

All projects must include static analysis tools such as linters and formatters for their corresponding language.
CSX Labs' projects adopt [Trunk](https://trunk.io/products/check) for linting and prefer to use Google's style guides when available.

### Inline Documentation

All projects must include inline documentation for ALL user-facing interfaces.

### Idiomatic Practices

All projects must adhere to the idiomatic practices of their corresponding language. Using appropriate
design patterns and language features is encouraged. Try to adhere to an opinionated style guide or philosophy
and stick to it throughout the project (for example, Robert C. Martin's philosophy of "Clean Code").

## DevOps

### Version Control

All projects must use a version control system. CSX Labs' projects use Git.

### Continuous Integration / Continuous Deployment (CI/CD)

All projects must have a CI/CD pipeline that can be run with a single command or linked
to an action such as a push to a branch or a pull request. CSX Labs' projects use GitHub Actions.
The CI/CD pipeline must include the following steps:

- Static Analysis
- Unit Testing
- Release (when applicable)

### Release

All projects must use a release system that can be run with a single command or linked
to an action such as a push to a branch or a pull request. The release names must follow
semantic versioning.

### Environments

All projects must have a logical separation of development and production environments, prioritizing the security of credentials and data.

### Security

There must be no exposed or hard-coded credentials in the project's source code. All credentials must be stored in a secure location and accessed through environment variables or a private config.
