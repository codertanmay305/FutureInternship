# Create README.md with full project documentation
@"
# 📄 Resume Screening System - Machine Learning Task 3

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![scikit-learn](https://img.shields.io/badge/scikit--learn-1.3.0-orange.svg)
![pandas](https://img.shields.io/badge/pandas-2.0.0-green.svg)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)

## 🎯 Overview
An ML-powered system that automatically screens and ranks resumes based on job requirements. Built for **Future Interns** Machine Learning Task 3 (2026).

### ✨ Key Features
✅ **Text Cleaning & Preprocessing** - Removes HTML, special characters, normalizes text  
✅ **Skill Extraction using NLP** - Matches against 92 HR skills database  
✅ **Resume-to-Job Matching** - Calculates match percentage with job requirements  
✅ **Candidate Ranking** - Sorts candidates by relevance  
✅ **Skill Gap Analysis** - Identifies missing critical skills  
✅ **TF-IDF Similarity** - ML-based text similarity scoring  

## 📊 Dataset
- **Source**: Resume Dataset from Kaggle
- **Total Resumes**: 2,484
- **Categories**: Multiple (HR, IT, Finance, Sales, etc.)
- **HR Resumes Analyzed**: 110

## 🏗️ Project Structure

TASK3_ML/
│
├── 📁 Data/
│ ├── Resume.csv # Raw resume dataset (2,484 resumes)
│ └── job_description.txt # HR Generalist job requirements
│
├── 📁 Notebooks/
│ └── InitialPhase.ipynb # Main ML pipeline notebook
│
├── 📁 Output/
│ ├── all_candidates_ranked.csv # Complete ranking of all candidates
│ ├── enhanced_hr_ranking.csv # HR-enhanced ranking with weights
│ ├── final_rankings_with_ml.csv # Final rankings with TF-IDF scores
│ ├── interview_shortlist.csv # Top candidates for interview
│ └── skill_gaps_analysis.csv # Detailed skill gap data
│
├── 📁 Reports/
│ ├── requirements.txt # Python dependencies
│ └── skills_gap_report.txt # Final analysis report
│
└── README.md # Project documentation


## 🔧 Tech Stack
| Technology | Purpose |
|------------|---------|
| **Python 3.8+** | Core programming language |
| **pandas, numpy** | Data manipulation & analysis |
| **scikit-learn** | TF-IDF vectorization, cosine similarity |
| **matplotlib, seaborn** | Data visualization |
| **NLTK/spaCy** | NLP text processing |
| **Jupyter Notebook** | Interactive development |

## 🚀 How It Works
### 1. Text Processing
- Removes HTML tags and special characters
- Converts to lowercase
- Removes extra whitespace

### 2. Skill Extraction
- 92 HR-specific skills database
- Categories: Recruitment, Employee Relations, Benefits, Compliance, HR Systems, Training, Software, Certifications

### 3. Matching Algorithm
- **Skill-based matching**: Counts matched skills vs required
- **TF-IDF similarity**: ML-based text similarity
- **Combined score**: 70% skill match + 30% TF-IDF

### 4. Ranking & Analysis
- Sorts candidates by match percentage
- Identifies missing skills
- Generates hiring recommendations

## 📈 Results
### Key Statistics
| Metric | Value |
|--------|-------|
| Total Resumes Processed | **2,484** |
| Average Match Score | 9.2% |
| Highest Score | **80.8%** |
| Lowest Score | 0.0% |
| Strong Matches (≥70%) | 1 candidate |
| Good Matches (50-69%) | 33 candidates |
| Weak Matches (30-49%) | 77 candidates |

### 🏆 Top Candidate
- **ID**: 17812897
- **Score**: 80.8%
- **Matched Skills**: 21 of 26 required
- **Missing Skills**: phr, talent acquisition, onboarding, microsoft office, workers compensation

### 🔍 Top Skill Gaps
| Skill | Missing % |
|-------|-----------|
| Paychex | 99.4% |
| PHR Certification | 99.2% |
| Employment Law | 99.1% |
| Talent Acquisition | 98.9% |
| SHRM Certification | 98.7% |

## 🚀 Quick Start

### Prerequisites
- Python 3.8 or higher
- Git

### Installation
```bash
# Clone the repository
git clone https://github.com/codertanmay305/Future_Intern_MachineLearning.git
cd Future_Intern_MachineLearning/TASK3_ML

# Install dependencies
pip install -r Reports/requirements.txt

# Download spaCy model (optional for advanced NLP)
python -m spacy download en_core_web_sm