# Getting Started with Copilot CLI - Calculator Project

Welcome to the `2-copilot-cli` branch! This branch contains a Node.js calculator application built using **GitHub Copilot CLI**.

## Prerequisites
- Node.js version 22 or later
- GitHub Copilot CLI installed
- GitHub Copilot subscription (Free, Pro, Pro+, Business, or Enterprise)
- Familiarity with command line operations

## Project Structure

```
├── index.js                          # Main calculator application
├── test.js                           # Test suite
├── package.json                      # Project configuration
├── .github/
│   ├── agents/
│   │   └── calculator-assistant.md   # Custom Copilot CLI agent
│   └── ISSUE_TEMPLATE/
│       └── calculator-feature.md     # Feature request template
└── GETTING_STARTED.md               # This file
```

## Quick Start

### 1. Install Dependencies
```bash
npm install
```

### 2. Run the Calculator
```bash
npm start
# or
node index.js
```

### 3. Run Tests
```bash
npm test
# or
node test.js
```

## Using Copilot CLI

### Install Copilot CLI
If you haven't already, install the standalone Copilot CLI:
```bash
npm install -g @github-next/github-copilot-cli
```

### Authenticate
```bash
copilot auth login
```

### Use the Calculator Assistant Agent
```bash
copilot /delegate "Add a modulo operation to the calculator"
```

The calculator assistant agent (`.github/agents/calculator-assistant.md`) will help guide the AI to make better suggestions for your calculator features.

### Create Issues with Copilot CLI
Use the issue template to create feature requests:
```bash
copilot issue create --template calculator-feature "Add logarithm operation"
```

## Available Calculator Operations

### Basic Operations
- **add(a, b)** - Addition
- **subtract(a, b)** - Subtraction
- **multiply(a, b)** - Multiplication
- **divide(a, b)** - Division (with zero-check)

### Advanced Operations
- **power(base, exponent)** - Exponentiation
- **squareRoot(n)** - Square root (with negative number check)

## Exercises

### Exercise 1: Add a New Operation
Use Copilot CLI to add a new mathematical operation to the calculator:
```bash
copilot /delegate "Add a modulo (remainder) operation to the calculator, including tests"
```

### Exercise 2: Improve Error Handling
Ask Copilot CLI to review and improve error handling:
```bash
copilot /delegate "Review the calculator error handling and suggest improvements"
```

### Exercise 3: Add Documentation
Use Copilot CLI to enhance documentation:
```bash
copilot /delegate "Add JSDoc comments to all calculator methods"
```

## Helpful Copilot CLI Commands

### Get Help
```bash
copilot help
```

### Share Your Work
Save a chat session as a GitHub gist:
```bash
copilot /share
```

### Run in Headless Mode
For automated workflows:
```bash
copilot /delegate "task" -p
```

## Next Steps

1. **Explore the calculator code** - Review `index.js` and `test.js`
2. **Run the tests** - Execute `npm test` to verify everything works
3. **Try Copilot CLI** - Use `/delegate` to add new features
4. **Create issues** - Use the feature template to track your work
5. **Collaborate** - Use `/share` to save and discuss your progress

## Resources

- [GitHub Copilot CLI Documentation](https://docs.github.com/en/copilot/github-copilot-in-the-cli)
- [Node.js Documentation](https://nodejs.org/docs/)
- [Calculator Issues](../../issues)

## Troubleshooting

### Issue: Tests are failing
```bash
# Run tests with verbose output
node test.js
```

### Issue: Copilot CLI not recognized
```bash
# Ensure it's installed globally
npm list -g @github-next/github-copilot-cli
```

### Issue: Authentication failed
```bash
# Re-authenticate
copilot auth logout
copilot auth login
```

---

**Happy coding with Copilot CLI! 🚀**
