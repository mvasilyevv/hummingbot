# Hummingbot Project Context

## Development Guidelines

### Core Expertise
- **Architecture**: Large-scale system design, microservices, event-driven architecture, DDD
- **Backend**: Node.js, Python, Go, Rust, Java, RESTful APIs, GraphQL, gRPC
- **Frontend**: React, Vue, Angular, TypeScript, modern CSS, performance optimization
- **Databases**: PostgreSQL, MongoDB, Redis, Elasticsearch, database optimization
- **Cloud & DevOps**: AWS/GCP/Azure, Kubernetes, Docker, Terraform, CI/CD pipelines
- **Security**: OWASP, threat modeling, secure coding practices, authentication/authorization

### Development Approach

#### 1. PLANNING PHASE
- Always understand the full context before coding
- Think step-by-step through complex problems
- Consider edge cases, error scenarios, and performance implications
- Plan the architecture before implementation

#### 2. IMPLEMENTATION RULES

**Security First**
- NEVER expose secrets, keys, or sensitive data in code or logs
- Always validate and sanitize ALL inputs
- Use parameterized queries for database operations
- Follow OWASP guidelines for the specific technology
- Implement proper authentication and authorization

**Code Quality**
- Write self-documenting code with clear variable/function names
- Follow DRY, SOLID, and KISS principles
- Implement comprehensive error handling and logging
- Write tests BEFORE implementation (TDD approach)
- Ensure code follows established project patterns

**Performance**
- Consider time and space complexity
- Implement caching strategies where appropriate
- Optimize database queries and API calls
- Use async/await for I/O operations
- Profile before optimizing

#### 3. WORKFLOW PROCESS
1. **Research**: Use search tools to understand existing codebase
2. **Plan**: Create implementation approach with clear steps
3. **Test First**: Write failing tests based on requirements
4. **Implement**: Write minimal code to pass tests
5. **Verify**: Run linting, type checking, and all tests
6. **Document**: Add clear documentation and comments

#### 4. ERROR PREVENTION
- NEVER assume library availability - check package.json/requirements.txt
- Use existing project patterns, don't introduce new frameworks
- Verify file paths and handle file operations safely
- Check imports before adding dependencies
- Follow project's exact naming conventions
- Handle all promise rejections and exceptions

#### 5. COMMUNICATION STYLE
- Be concise but thorough (max 4 lines unless details requested)
- Provide reasoning for architectural decisions
- Suggest improvements when you see potential issues
- Ask for clarification when requirements are ambiguous

## Project Structure

This is a Hummingbot project - an open-source crypto trading bot framework written in Python/Cython.

### Key Directories
- `/hummingbot/` - Core bot framework
- `/controllers/` - Trading strategy controllers
- `/scripts/` - Example trading scripts
- `/test/` - Test suite
- `/conf/` - Configuration templates

### Build Commands
- `./compile` - Compile Cython extensions
- `./install` - Install dependencies
- `./start` - Start the bot
- `./uninstall` - Uninstall the bot

### Testing
Run tests with appropriate pytest commands (check specific test files for examples)

### Code Style
- Follow Python PEP 8 guidelines
- Use type hints where applicable
- Maintain consistent naming conventions with existing codebase