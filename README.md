# 🚀 Sarvam AI Playground

A comprehensive playground repository for experimenting with [Sarvam AI](https://sarvam.ai/)'s powerful Indian language models and building multilingual AI applications.

## 🎯 About

This repository serves as a learning and experimentation environment for:
- **Multilingual AI applications** using Sarvam AI's models
- **Python development best practices** with comprehensive linting and formatting
- **Machine Learning engineering** workflows and patterns
- **Pre-commit hooks** for maintaining code quality

## ✨ Features

- 🔧 **Professional Development Setup** - Pre-commit hooks with Black, Isort, Flake8, and Pylint
- 🌏 **Multilingual Support** - Ready for Indian language processing with Sarvam AI
- 📚 **Learning-Focused** - Comprehensive linting rules to improve Python skills
- 🤖 **ML-Ready** - Configured for machine learning and AI projects
- 📝 **Well-Documented** - Clear examples and documentation for learning

## 🛠️ Setup

### Prerequisites
- Python 3.8+
- Git
- Sarvam AI API access ([Get API key](https://sarvam.ai/))

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/sarvam-ai-project.git
   cd sarvam-ai-project
   ```

2. **Create virtual environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt  # Create this file with your dependencies
   ```

4. **Install pre-commit hooks**
   ```bash
   pip install pre-commit
   pre-commit install
   ```

5. **Set up environment variables**
   ```bash
   cp .env.example .env
   # Edit .env with your Sarvam AI API credentials
   ```

## 📁 Project Structure
```markdown
sarvam-ai-project/
├── .pre-commit-config.yaml         # Code quality automation
├── .pylintrc                       # Python linting configuration
├── .gitignore                      # Patterns for git to ignore
└── README.md                       # Repo Documentation
```


### Development Workflow

1. **Create a new feature branch**
   ```bash
   git checkout -b feature/new-experiment
   ```

2. **Write your code** - Pre-commit hooks will automatically:
   - Format code with Black
   - Sort imports with isort
   - Check style with Flake8
   - Analyze code quality with Pylint

3. **Run tests**
   ```bash
   python -m pytest tests/
   ```

4. **Commit your changes**
   ```bash
   git add .
   git commit -m "Add new multilingual chatbot experiment"
   ```

## 🔧 Development Tools

### Pre-commit Hooks
This project uses comprehensive pre-commit hooks for code quality:

- **Black** - Code formatting
- **isort** - Import sorting
- **Flake8** - Style and error checking
- **Pylint** - Advanced code analysis

Run manually on all files:
```bash
pre-commit run --all-files
```

### Code Quality Standards
- **Line length**: 100 characters
- **Naming**: snake_case for functions/variables, PascalCase for classes
- **Docstrings**: Required for all public functions
- **Type hints**: Encouraged for better code documentation

## 📚 Learning Resources

### Sarvam AI Documentation
- [Official API Documentation](https://docs.sarvam.ai/)
- [Supported Languages](https://sarvam.ai/languages)
- [Model Capabilities](https://sarvam.ai/models)

### Python Best Practices
- Understanding pylint messages and fixes
- Writing clean, maintainable code
- ML engineering patterns and practices
- Testing strategies for AI applications

## 🧪 Examples

### Multilingual Chatbot
```python
# examples/multilingual_chatbot.py
from src.models.sarvam_integration import SarvamChatbot

chatbot = SarvamChatbot()
response = chatbot.chat(
    message="आप कैसे हैं?",
    language="hi",
    context="casual_conversation"
)
```

### Language Detection
```python
# examples/language_detection.py
from src.utils.language_utils import detect_language

text = "यह हिंदी में लिखा गया है"
language = detect_language(text)  # Returns: "hi"
```


# Sarvam AI Configuration
SARVAM_API_KEY=your_api_key_here
SARVAM_BASE_URL=https://api.sarvam.ai

# Development Configuration
DEBUG=True
LOG_LEVEL=INFO
```

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🤝 Acknowledgments

- [Sarvam AI](https://sarvam.ai/) for providing excellent Indian language AI models
- Pre-commit community for amazing development tools
- Python community for best practices and conventions

---
