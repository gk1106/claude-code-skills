# Claude Code Skills

A collection of reusable, developer-focused skills for Claude Code, designed to improve development workflows, code quality, architecture, and productivity.

These skills provide structured instructions that help Claude understand project conventions, follow engineering best practices, and perform development tasks consistently.

## Why This Repository?

Working across multiple projects often involves repeating the same instructions for code generation, debugging, API development, testing, and deployment.

This repository provides reusable skills that can be installed and shared across different projects.

**Write once. Reuse across projects.**

## Available Skills

| Skill | Description |
|---|---|
| Spring Boot Development | Build production-ready Spring Boot applications |
| Java Code Review | Review Java code for performance, readability, and maintainability |
| React Development | Develop reusable React components and application features |
| Frontend Design | Create responsive, modern user interfaces |
| API Integration | Implement REST API integrations and error handling |
| Docker Deployment | Containerize applications using Docker |
| AWS Deployment | Configure and deploy applications to AWS |
| Spring AI Development | Build AI-powered applications using Spring AI, RAG, and tool calling |

## Repository Structure

```text
claude-code-skills/
├── skills/
│   ├── spring-boot-development/
│   ├── java-code-review/
│   ├── react-development/
│   ├── frontend-design/
│   ├── api-integration/
│   ├── docker-deployment/
│   ├── aws-deployment/
│   └── spring-ai-development/
├── examples/
├── docs/
└── README.md
```

## Installation

Clone the repository:

```bash
git clone https://github.com/GK1106/claude-code-skills.git
cd claude-code-skills
```

### Option 1: Install Skills Globally

Copy individual skill folders into your personal Claude skills directory:

```text
~/.claude/skills/
```

Example:

```bash
cp -r skills/spring-boot-development ~/.claude/skills/
```

Skills installed here can be reused across projects.

### Option 2: Install Skills in a Project

Copy the required skills into your project's local Claude directory:

```text
your-project/
└── .claude/
    └── skills/
        ├── spring-boot-development/
        │   └── SKILL.md
        └── react-development/
            └── SKILL.md
```

This allows project-specific skill configuration.

## Creating a New Skill

Every skill must contain a `SKILL.md` file with YAML frontmatter.

Example:

```markdown
---
name: spring-boot-development
description: Build and maintain Spring Boot applications using Java, REST APIs, JPA, and production-ready engineering practices.
---

# Spring Boot Development

## Instructions

- Follow layered architecture.
- Use constructor-based dependency injection.
- Implement centralized exception handling.
- Validate incoming API requests.
- Follow REST API conventions.
- Write maintainable and testable code.

## Workflow

1. Understand the requirement.
2. Review the existing architecture.
3. Implement the solution.
4. Add validation and error handling.
5. Write or update tests.
6. Verify the implementation.
```

## Using Skills

After installing a skill, open Claude Code in your project.

Claude can discover relevant skills based on their descriptions.

You can also invoke a skill directly:

```text
/spring-boot-development
```

Example request:

```text
Use the spring-boot-development skill to implement
a JWT authentication module with Spring Security.
```

## Contributing

Contributions are welcome.

1. Fork the repository.
2. Create a feature branch.
3. Add or improve a skill.
4. Test the skill using Claude Code.
5. Submit a pull request.

## License

MIT License.

## Author

**Ganeshkumar V**

Java Full Stack Developer | Spring Boot | React | AWS | AI Engineering

GitHub: https://github.com/GK1106

---

Built for developers who want reusable AI-assisted engineering workflows.
