# My Material Site

A comprehensive documentation site built with MkDocs Material theme.

## Features

- 📚 Comprehensive documentation structure
- 🎨 Modern Material Design theme
- 📊 Interactive Jupyter notebooks
- 🔍 Full-text search
- 📱 Mobile-responsive design
- 🌙 Dark/Light mode toggle

## Quick Start

### Prerequisites

- Python 3.8 or higher
- PowerShell 7+

### Installation

1. Clone the repository:
\\\ash
git clone https://github.com/eagleanalytix/mktest.git
cd my-material-project
\\\

2. Create and activate virtual environment:
\\\powershell
python -m venv mkdocs-env
.\mkdocs-env\Scripts\Activate.ps1
\\\

3. Install dependencies:
\\\ash
pip install -r requirements.txt
\\\

### Local Development

Build and serve the site locally:
\\\ash
mkdocs serve
\\\

Visit http://127.0.0.1:8000 in your browser.

### Build Static Site

Build the static site:
\\\ash
mkdocs build
\\\

## Project Structure

\\\
my-material-project/
├── docs/
│   ├── index.md                 # Home page with card grid
│   ├── getting-started/         # Getting started guides
│   ├── guides/                  # User guides
│   ├── tutorials/               # Step-by-step tutorials
│   ├── notebooks/               # Jupyter notebooks
│   ├── reference/               # API reference
│   └── assets/                  # Images and static files
├── mkdocs.yml                   # MkDocs configuration
├── requirements.txt             # Python dependencies
└── README.md                    # This file
\\\

## Documentation Sections

- **Getting Started**: Installation and quick start guides
- **User Guides**: Comprehensive feature documentation
- **Tutorials**: Step-by-step learning paths
- **Notebooks**: Interactive Jupyter notebooks
- **Reference**: API documentation

## Deployment

### GitHub Pages

Deploy to GitHub Pages:
\\\ash
mkdocs gh-deploy
\\\

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License.

## Support

For questions and support, please open an issue on GitHub.

