<a name="readme-top"></a>

<div align="center">
  <br/>

  <h3><b>Welcome to Obasity level classification model</b></h3>

</div>

<!-- TABLE OF CONTENTS -->

# 📗 Table of Contents

- [📖 About the Project](#about-project)
- [💻 Getting Started](#getting-started)
  - [Setup](#setup)
  - [Prerequisites](#prerequisites)
  - [Usage](#usage)
- [Key Features](#key-features)
- [👥 Authors](#authors)
- [🤝 Contributing](#contributing)
- [⭐️ Show your support](#support)
- [🙏 Acknowledgements](#acknowledgements)
- [📝 License](#license)

<!-- PROJECT DESCRIPTION -->

# 📖 AI-Based Classification of Obesity Levels Using Lifestyle Data from Latin America <a name="about-project"></a>

**Abstract** Obesity is a growing health concern globally, especially in developing regions. In this study, we present an AI-based approach to classify obesity levels using lifestyle and biometric data from individuals in Colombia, Peru, and Mexico. The dataset includes 17 features such as eating habits, physical activity, and body measurements. To improve model performance, categorical features were encoded using binary encoding, and Body Mass Index (BMI) was calculated and used to create additional binary features based on WHO obesity categories. We addressed class imbalance using the SMOTE technique. Multiple machine learning models were trained and compared, with the Neural Network model achieving the highest accuracy of 96.22%. Our findings demonstrate the effectiveness of feature engineering and deep learning in predicting obesity levels for personalized health monitoring.

**Introduction**
Obesity is a serious global health issue that affects people of all ages and social backgrounds. It increases the risk of various chronic conditions, such as cardiovascular disease, diabetes, and certain cancers. According to the World Health Organization (WHO), the global prevalence of obesity has nearly tripled since 1975. In Latin America, countries such as Colombia, Peru, and Mexico are experiencing a rise in obesity rates due to lifestyle changes, including unhealthy eating habits and reduced physical activity.
In this study, we aim to develop a machine learning model that can accurately classify individuals into different obesity categories based on their personal, behavioral, and physical information. We used a dataset that contains data from 2111 individuals in Colombia, Peru, and Mexico. The data includes features such as age, gender, weight, height, frequency of physical activity, alcohol consumption, number of meals per day, water intake, use of electronic devices, and more. These features provide insights into each individual's lifestyle and health habits.
To enhance the dataset and improve model performance, we applied several preprocessing steps. First, we handled both numerical and categorical variables by applying binary encoding to all categorical features. This method was chosen over one-hot encoding to reduce dimensionality while still making the data suitable for machine learning algorithms.
Second, we engineered a new feature—Body Mass Index (BMI)—calculated using the formula:
BMI = weight (kg) / height² (m²)
Based on WHO standards, we categorized BMI values into six obesity levels: Underweight, Normal, Overweight, Obese I, Obese II, and Obese III. Each BMI category was then transformed into a binary feature using one-vs-all encoding (e.g., BMI_Underweight, BMI_Normal, etc.). This additional feature set helped models better learn the relationship between health indicators and obesity levels. Model accuracy improved after adding these BMI category features.
To address the issue of class imbalance—common in health datasets—we applied the SMOTE (Synthetic Minority Oversampling Technique) method. This helped balance the distribution of obesity classes, especially those with fewer instances, and allowed the machine learning models to generalize better.
After preprocessing, we trained and evaluated five different machine learning models: Neural Network, Logistic Regression, Naive Bayes, k-Nearest Neighbors (k-NN), and Support Vector Machine (SVM). The Neural Network achieved the best performance with an accuracy of 96.22%, outperforming other models. This was an improvement from the initial model (without BMI categories), which had an accuracy of 95.98% using the same Neural Network architecture.
This research demonstrates how machine learning, combined with effective feature engineering and preprocessing techniques, can be used to build accurate models for predicting obesity levels. Such tools can be used in health monitoring applications, personalized fitness planning, and early risk detection for obesity-related diseases.

**Results**
The performance of five machine learning models was evaluated on the task of obesity level classification. Models were trained on a dataset that included lifestyle, biometric, and dietary features from individuals in Colombia, Peru, and Mexico. Accuracy was used as the main performance metric, and comparisons were made between models trained with and without BMI-based features.

Model	Accuracy (Before BMI)	Accuracy (After BMI)
Neural Network	95.98%	96.22%
Logistic Regression	95.74%	94.80%
Naive Bayes	89.36%	95.04%
k-NN	—	91.02%
SVM	89.36%	55.56%
		


### Tech Stack <a name="tech-stack"></a>

> Python

<details>
  <summary>Client</summary>
  <ul>
    <li><a href="#">Python</a></li>
       
  </ul>
</details>

<!-- LIVE DEMO -->

## 🚀 Live Demo <a name="live-demo"></a>

<a href="">Soon</a>

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- GETTING STARTED -->

## 💻 Getting Started <a name="getting-started"></a>


To get a local copy up and running, follow these steps.

### Prerequisites

In order to run this project you need:
* You need to have Python3 installed.

Import the following libraries:
* import pandas
* import matplotlib
* import seaborn
* import sklearn
  
### Setup

Clone this repository to your desired folder:

```bash
git clone https://github.com/tawakuliKH/AI-Based-Classification-of-Obesity-Levels-Using-Lifestyle-Data-from-Latin-America.git
```
2. Open terminal and cd into project
```bash
cd 
```



### Key Features <a name="key-features"></a>

- **Higher Accuracy**



<p align="right">(<a href="#readme-top">back to top</a>)</p>


## 👥 Authors <a name="authors"></a>

>

👤 **Morteza Tawakuli**

- GitHub: [@tawakuliKH](https://github.com/tawakuliKH)
- LinkedIn: [@Morteza Tawakuli](https://www.linkedin.com/in/morteza-tawakuli-904818170/)



<p align="right">(<a href="#readme-top">back to top</a>)</p>

## 🤝 Contributing

 Contributions, issues, and feature requests are welcome!
- Feel free to check the [issues page](https://github.com/tawakuliKH/Diabetes-Prediction-Django-Web-App/issues)

## ⭐️ Show your support <a name="support"></a>

> 

If you like this project give it a star

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- ACKNOWLEDGEMENTS -->

## 🙏 Acknowledgments <a name="acknowledgements"></a>

### Paper Citation

This project is implemented based on the following Dataset:

- Author(s): Fabio Mendoza Palechor, Alexis de la Hoz Manotas
- Title: Dataset for estimation of obesity levels based on eating habits and physical condition in individuals from Colombia, Peru and Mexi
- Published in: [ScienceDirect](https://www.sciencedirect.com/science/article/pii/S2352340919306985?via%3Dihub)




<p align="right">(<a href="#readme-top">back to top</a>)</p>
<!-- LICENSE -->

## 📝 License <a name="license"></a>

This project is [MIT](./LICENSE) licensed.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

