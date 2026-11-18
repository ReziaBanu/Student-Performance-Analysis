# Student Performance Analysis Using Python

## Project Overview
This project focuses on analysing student academic performance using Python libraries such as **Pandas, Matplotlib, and Seaborn**.

The dataset contains marks obtained by five students in three subjects: Mathematics, Science, and Social Science. The data is imported, organised, analysed, and visualised to understand students' performance across different subjects.

## Objectives
- To understand data ingestion using Python.
- To import and organise data using Pandas.
- To create and manipulate a DataFrame.
- To analyse students' marks in different subjects.
- To create meaningful visualisations using Matplotlib and Seaborn.
- To compare student performance using graphs and heatmaps.

## Technologies Used

| Technology | Purpose |
|---|---|
| Python | Programming language |
| Pandas | Data ingestion and data manipulation |
| Matplotlib | Data visualisation |
| Seaborn | Statistical data visualisation |
| Google Colab | Python programming environment |

## Dataset Description

The dataset contains the academic marks of five students.

| Student Name | Maths | Science | Social Science |
|---|---:|---:|---:|
| Arun | 85 | 78 | 90 |
| Banu | 75 | 88 | 82 |
| Charan | 90 | 92 | 85 |
| Divya | 80 | 75 | 88 |
| Ezhil | 95 | 85 | 92 |

## Data Ingestion

The dataset is imported into Python using Pandas.

```python
import pandas as pd

df = pd.read_csv("students_marks.csv")

print(df)
```

For Excel files, the following function is used:

```python
df = pd.read_excel("students_marks.xlsx")
```

## Data Visualisation

The project uses different visualisation techniques to represent student performance.

### 1. Bar Plot
Used to compare students' marks in different subjects.

### 2. Line Plot
Used to represent and compare subject-wise marks.

### 3. Scatter Plot
Used to identify the relationship between marks obtained in two subjects.

### 4. Heatmap
Used to display student marks using different colour shades.

```python
import seaborn as sns
import matplotlib.pyplot as plt

sns.heatmap(df.set_index('students').astype(int),
            annot=True,
            cmap='Blues',
            linewidths=0.5)

plt.title("Student Performance Analysis")
plt.xlabel("Subjects")
plt.ylabel("Students")
plt.show()
```

## Key Learnings
- Understanding data ingestion.
- Working with Pandas DataFrames.
- Reading CSV and Excel files.
- Using Matplotlib for graphical representation.
- Using Seaborn for attractive statistical visualisations.
- Understanding and interpreting heatmaps.

## Project Structure

```text
Student-Performance-Analysis/
│
├── students_marks.csv
├── Student_Performance_Analysis.ipynb
└── README.md
```

## How to Run the Project

1. Clone or download this repository.
2. Open the Jupyter Notebook in Google Colab or Jupyter Notebook.
3. Upload the dataset or connect Google Drive.
4. Install the required libraries if necessary.

```python
pip install pandas matplotlib seaborn openpyxl
```

5. Run the Python cells to analyse and visualise the dataset.

## Conclusion

This project demonstrates how Python libraries can be used to ingest, organise, analyse, and visualise student performance data. Pandas helps manage the dataset, while Matplotlib and Seaborn help present the information through meaningful graphical representations.

The project provides a practical introduction to Data Analytics and Data Visualisation using Python.

---

**Developed as a Python Data Analytics Learning Project.**
