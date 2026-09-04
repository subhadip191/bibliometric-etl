# 📚 Bibliometrix Python

### A Python-Based Bibliometric Analysis and Science Mapping Platform

**Bibliometrix Python** is a Python-based implementation of core bibliometric analysis and science-mapping functionality inspired by the established [`bibliometrix`](https://github.com/massimoaria/bibliometrix) R ecosystem.

The project provides a modern Python environment for importing, processing, analyzing, and visualizing bibliographic data from multiple scholarly databases. It combines an ETL-oriented data pipeline with interactive analytical tools to support researchers in exploring scientific literature, research trends, collaboration networks, citation structures, and thematic development.

> **Academic Project**
> Developed collaboratively by a four-member team under the supervision of **Professor Vincenzo Moscato**.

---

## ✨ Features

### 📥 Bibliographic Data Import

Import and process bibliographic records from multiple scholarly data sources, including:

* 🌐 Web of Science
* 📊 Scopus
* 📚 OpenAlex
* 📐 Dimensions
* 🔍 The Lens
* 🧬 PubMed
* ⚕️ Cochrane

The system is designed to work with commonly used bibliographic export formats while providing a unified processing workflow.

---

### 🔄 Bibliometric ETL Pipeline

The project follows an **Extract → Transform → Load** workflow for bibliographic data:

```text
Bibliographic Sources
        │
        ▼
     Extract
        │
        ▼
     Transform
        │
        ├── Metadata normalization
        ├── Author processing
        ├── Keyword processing
        ├── Citation processing
        └── Data cleaning
        │
        ▼
       Load
        │
        ▼
Structured Bibliometric Dataset
        │
        ▼
 Analysis & Visualization
```

This architecture allows data from different sources to be transformed into a consistent structure suitable for downstream bibliometric analysis.

---

## 📊 Bibliometric Analysis

The platform supports analytical workflows for exploring:

* 📈 Publication trends
* 👥 Author productivity
* 🏛️ Institutional collaboration
* 🌍 Country and geographic contributions
* 📑 Citation analysis
* 🔗 Co-authorship networks
* 🔑 Keyword analysis
* 🧩 Co-occurrence networks
* 📚 Bibliographic coupling
* 🔄 Co-citation analysis
* 🧠 Thematic analysis
* 📌 Research impact indicators
* 📊 Science-mapping visualizations

The goal is to provide researchers with an integrated workflow for moving from raw bibliographic records to interpretable research insights.

---

## 🖥️ Interactive Interface

The application provides an interactive interface for:

1. Importing bibliographic datasets
2. Selecting analytical workflows
3. Processing bibliographic metadata
4. Generating statistical summaries
5. Exploring networks and relationships
6. Creating visualizations
7. Exporting analytical results

The interface is designed to make bibliometric workflows accessible without requiring users to manually implement each analytical procedure.

---

## 🏗️ Project Architecture

The project is organized around separate components for data processing, analysis, visualization, and application functionality.

```text
bibliometrix-python/
│
├── app.py                  # Main application entry point
├── requirements.txt        # Python dependencies
├── README.md              
│
├── functions/             # Analysis functions
│   ├── get_annualproduction.py
│   ├── get_averagecitations.py
│   ├── get_bradfordlaw.py
│   ├── get_relevantauthors.py
│   ├── get_relevantsources.py
│   └── ... (35+ analysis modules)
│
├── www/                   # Web application components
│   ├── services/          # Core bibliometric services
│   │   ├── parsers.py
│   │   ├── format_functions.py
│   │   ├── networkplot.py
│   │   ├── thematicmap.py
│   │   └── utils.py
│   └── static/            # Static assets (CSS, JS)
│       └── biblioshiny.css
│
└── sources/               # Sample datasets and test files
    ├── Web_of_Science/
    ├── Scopus/
    ├── PubMed/
    ├── Dimensions/
    ├── Lens/
    └── Cochrane/
```

The modular structure is intended to make the system easier to maintain, extend, and integrate with additional bibliographic data sources and analytical methods.

---

## 🛠️ Technology Stack

| Technology              | Purpose                                   |
| ----------------------- | ----------------------------------------- |
| **Python**              | Core programming language                 |
| **Pandas**              | Data manipulation and processing          |
| **NumPy**               | Numerical computation                     |
| **SciPy**               | Scientific computing                      |
| **Scikit-learn**        | Statistical and machine-learning analysis |
| **NetworkX / igraph**   | Network analysis                          |
| **Matplotlib / Plotly** | Data visualization                        |
| **GeoPandas**           | Geographic analysis                       |
| **Shiny for Python**    | Interactive application interface         |
| **NLTK**                | Natural-language processing               |
| **WordCloud**           | Keyword visualization                     |
| **Selenium**            | Web-based data workflows                  |

---

## 🚀 Getting Started

### Prerequisites

* Python **3.10 or higher**
* `pip`
* Git

### 1. Clone the repository

```bash
git clone https://github.com/subhadip191/bibliometric-etl.git
cd bibliometric-etl
```

### 2. Create a virtual environment

#### Windows

```powershell
python -m venv .venv
.venv\Scripts\activate
```

#### macOS / Linux

```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the application

```bash
python app.py
```

Follow the application's interface to import bibliographic data and begin the analysis workflow.

---

## 🧪 Testing

The project includes automated tests covering important components of the application.

Run the test suite with:

```bash
pytest
```

For more detailed output:

```bash
pytest -v
```

Testing is used to verify data-processing functionality and reduce regressions as the project evolves.

---

## 📁 Supported Data Workflow

A typical analysis can be performed through the following workflow:

```text
1. Export bibliographic records
              │
              ▼
2. Import dataset
              │
              ▼
3. Validate and normalize metadata
              │
              ▼
4. Build structured bibliometric data
              │
              ▼
5. Select analysis
              │
              ▼
6. Generate statistics / networks
              │
              ▼
7. Visualize results
              │
              ▼
8. Interpret research trends
```

This workflow is designed to support reproducible bibliometric research from raw bibliographic records through final analytical outputs.

---

## 🔬 Relationship to Bibliometrix

This project is inspired by and implements functionality associated with the **bibliometrix** ecosystem developed for comprehensive science mapping analysis.

The original `bibliometrix` project is an R-based open-source project developed by **Massimo Aria and Corrado Cuccurullo**, together with its broader contributor community.

This repository contains the **Python implementation developed by our team** and is **not an official Python distribution of the original bibliometrix R package**.

For the original project and its complete contributor history, please refer to:

**bibliometrix — R-tool for comprehensive science mapping analysis**
https://github.com/massimoaria/bibliometrix

---

## 👨‍💻 Development Team

This project was developed collaboratively as an academic/research project by a four-member team under the supervision of:

### 🎓 Supervisor

**Professor Vincenzo Moscato**

### 👥 Team Members

* **Subhadip Maity**
* **Vedant Gajanan Pawar**
* **Deepak Kushwaha**
* **Vishal Kumar**

All members contributed to the development, implementation, testing, documentation, and refinement of the project.

---

## 📖 Citation

If you use this project or its implementation in academic work, please acknowledge the original bibliometrix research:

> Aria, M., & Cuccurullo, C. (2017). *bibliometrix: An R-tool for comprehensive science mapping analysis*. Journal of Informetrics, 11(4), 959–975.

**DOI:** 10.1016/j.joi.2017.08.007

The citation acknowledges the original bibliometrix research and methodology on which this project builds.

---

## 📜 License

This project is distributed under the **GNU General Public License v3.0 (GPL-3.0)**.

See the [`LICENSE`](LICENSE) file for the complete license text.

---

## 🙏 Acknowledgements

We would like to acknowledge:

* **Massimo Aria and Corrado Cuccurullo** for the original bibliometrix project and its contributions to bibliometric and science-mapping research.
* The **bibliometrix contributor community** for the development and continued evolution of the original ecosystem.
* **Professor Vincenzo Moscato** for academic supervision and guidance throughout the development of this project.
* All members of the development team for their collaborative contributions.

---

## 📌 Project Status

**Academic / Research Project**

The current implementation focuses on providing core bibliometric data-processing, analysis, and visualization capabilities in a Python environment.

The architecture is designed to be extensible, allowing additional data sources, analytical methods, visualization techniques, and bibliometric indicators to be incorporated in future development.

---

## 📫 Repository

**GitHub:**
https://github.com/subhadip191/bibliometric-etl

---

### ⭐ Acknowledgement

If this project is useful for your research or development work, consider giving the repository a ⭐ on GitHub.
