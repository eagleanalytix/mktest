# Tutorial 2: Working with Data

## Overview

Learn how to work with data effectively in your applications.

**Duration:** 45 minutes  
**Difficulty:** Intermediate

## Prerequisites

- Completed [Tutorial 1](tutorial-1.md)
- Understanding of Python data structures

## Learning Objectives

- 📊 Read and write data files
- 🔄 Transform data
- 📈 Visualize results
- 💾 Store data persistently

## Step 1: Reading Data

### CSV Files

\\\python
import csv

def read_csv(filename):
    with open(filename, 'r') as file:
        reader = csv.DictReader(file)
        return list(reader)

data = read_csv('data.csv')
\\\

### JSON Files

\\\python
import json

def read_json(filename):
    with open(filename, 'r') as file:
        return json.load(file)

data = read_json('data.json')
\\\

## Step 2: Data Transformation

Process and transform data:

\\\python
def transform_data(data):
    return [
        {
            'id': item['id'],
            'value': float(item['value']) * 2
        }
        for item in data
    ]

transformed = transform_data(data)
\\\

## Step 3: Data Analysis

Perform basic analysis:

\\\python
def analyze_data(data):
    values = [item['value'] for item in data]
    return {
        'count': len(values),
        'sum': sum(values),
        'average': sum(values) / len(values),
        'min': min(values),
        'max': max(values)
    }

stats = analyze_data(data)
print(stats)
\\\

## Step 4: Visualization

Create simple visualizations:

\\\python
import matplotlib.pyplot as plt

def plot_data(data):
    values = [item['value'] for item in data]
    plt.plot(values)
    plt.title('Data Visualization')
    plt.xlabel('Index')
    plt.ylabel('Value')
    plt.show()

plot_data(data)
\\\

## Step 5: Saving Results

Save processed data:

\\\python
def save_results(data, filename):
    with open(filename, 'w') as file:
        json.dump(data, file, indent=2)

save_results(transformed, 'results.json')
\\\

## Complete Example

Here's a complete working example:

\\\python
import csv
import json

class DataProcessor:
    def __init__(self, input_file):
        self.input_file = input_file
        self.data = None
    
    def load(self):
        with open(self.input_file, 'r') as file:
            self.data = json.load(file)
    
    def process(self):
        return [item['value'] * 2 for item in self.data]
    
    def save(self, output_file):
        with open(output_file, 'w') as file:
            json.dump(self.data, file)

# Usage
processor = DataProcessor('input.json')
processor.load()
results = processor.process()
processor.save('output.json')
\\\

## Practice Exercises

1. Load a CSV file with sales data
2. Calculate monthly averages
3. Create a bar chart of results
4. Export to JSON format

!!! tip "Bonus Challenge"
    Implement error handling for missing files and invalid data.

## Summary

You've learned:

- ✅ File I/O operations
- ✅ Data transformation techniques
- ✅ Basic data analysis
- ✅ Visualization basics

Continue to the [Notebooks section](../notebooks/analysis.ipynb) for interactive examples!

