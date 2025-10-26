# Tutorial 1: Building Your First Application

## Overview

In this tutorial, you'll learn how to build a complete application from scratch.

**Duration:** 30 minutes  
**Difficulty:** Beginner

## Prerequisites

- Basic Python knowledge
- Completed [Installation](../getting-started/installation.md)

## Learning Objectives

By the end of this tutorial, you will:

- ✅ Understand the project structure
- ✅ Create a basic application
- ✅ Implement core functionality
- ✅ Test your application

## Step 1: Project Setup

Create a new project directory:

\\\ash
mkdir my-first-app
cd my-first-app
\\\

## Step 2: Create Main File

Create \main.py\:

\\\python
# main.py
def main():
    print("Hello, World!")
    
if __name__ == "__main__":
    main()
\\\

## Step 3: Add Functionality

Extend the application:

\\\python
# main.py
class Application:
    def __init__(self, name):
        self.name = name
    
    def run(self):
        print(f"Running {self.name}...")
        self.process()
    
    def process(self):
        # Core logic here
        pass

def main():
    app = Application("My First App")
    app.run()
    
if __name__ == "__main__":
    main()
\\\

## Step 4: Testing

Test your application:

\\\ash
python main.py
\\\

## Expected Output

\\\
Running My First App...
\\\

## Next Steps

!!! success "Completed!"
    Congratulations! You've built your first application.

Continue to [Tutorial 2](tutorial-2.md) to learn more advanced concepts.

## Exercises

Try these challenges:

1. Add command-line arguments
2. Implement error handling
3. Add logging functionality

