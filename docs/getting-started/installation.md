# Installation Guide

## Prerequisites

Before you begin, ensure you have the following installed:

- Python 3.8 or higher
- pip (Python package manager)
- Git

## Installation Steps

### Step 1: Clone the Repository

\\\ash
git clone https://github.com/eagleanalytix/mktest.git
cd mktest
\\\

### Step 2: Create Virtual Environment

\\\ash
python -m venv venv
\\\

### Step 3: Activate Virtual Environment

**Windows:**
\\\powershell
.\venv\Scripts\Activate.ps1
\\\

**Linux/Mac:**
\\\ash
source venv/bin/activate
\\\

### Step 4: Install Dependencies

\\\ash
pip install -r requirements.txt
\\\

## Verification

Verify your installation by running:

\\\ash
python --version
pip list
\\\

## Troubleshooting

!!! warning "Common Issues"
    If you encounter permission errors, try running with administrator privileges or use \--user\ flag with pip.

## Next Steps

Now that you have everything installed, proceed to the [Quick Start Guide](quick-start.md).

