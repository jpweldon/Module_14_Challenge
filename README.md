# Module_14_Challenge

# Algorithmic Trading

---

## Introduction:

The premise of this project is that I am a financial advisor at one of the top five financial advisory firms in the world. My firm constantly competes with the other major firms to manage and automatically trade assets in a highly dynamic environment. In recent years, my firm has heavily profited by using computer algorithms that can buy and sell faster than human traders.

The speed of these transactions gave my firm a competitive advantage early on. But, people still need to specifically program these systems, which limits their ability to adapt to new data. I am planning to improve the existing algorithmic trading systems and maintain the firm’s competitive advantage in the market. To do so, I am enhancing the existing trading signals with machine learning algorithms that can adapt to new data.

I am creating an algorithmic trading bot that learns and adapts to new data and evolving markets. I am implementing an algorithmic trading strategy that uses machine learning to automate the trade decisions, adjusting the input parameters to optimize the trading algorithm, and training a new machine learning model. I am comparing the new models performance to that of the baseline model.

I have created a Jupyter notebook containing my analysis, including text and comments to document my findings.

---

## Technologies

This project leverages python 3.7 with the following modules:

* [pandas](https://github.com/pandas-dev/pandas) - For reading data into a DataFrame and analyzing data via statistics and plots.

* [numpy](https://numpy.org) - For computation.

* [hvplot](https://hvplot.holoviz.org) - For plotting in various formats working with a wide array of datatypes in the PyData ecosystem.

* [csv](https://docs.python.org/3/library/csv.html) - For reading and writing tabular data in CSV (Comma Seperated Values) format.

* [pathlib](https://docs.python.org/3/library/pathlib.html) - For representing the file system path to a csv.

* [sklearn](https://scikit-learn.org/stable/user_guide.html#) - For machine learning.

* [matplotlib](https://matplotlib.org/stable/users/index.html) - For embedding plots in the application.

---

## Installation Guide

Before running the application first install the following dependencies:

```python
  pip install pandas
  pip install hvplot
  pip install -U scikit-learn
  pip install mkdocs
```

---

## Usage

To use the Algorithmic Trading application:

Clone the Module_14_Challenge repository from GitHub:

'git clone https://github.com/jpweldon/Module_14_Challenge.git'

Run the machine_learning_trading_bot.ipynb program.

Examine the data analysis, text, and comments that document my findings.

Run the tune_baseline_trading_algorithm_slice_dates.ipynb and tune_baseline_trading_algorithm_adjust_windows.ipynb programs.

Examine the data analysis, text, and comments that document my findings.

In the Resources folder, reference the SVM_Model_Returns_Plot, SVM_Classification_Report, LogisticRegression_Model_Returns_Plot, LogisticRegression_Classification_Report, SVM_Model_Sliced_Returns_Plot, SVM_Sliced_Classification_Report, SVM_Model_50DayShortWindow_Returns_Plot, and SVM_Model_50DayShortWindow_Classification_Report .png files. This information can also be found in the Evaluation Report section of the machine_learning_trading_bot, tune_baseline_trading_algorithm_slice_dates, and tune_baseline_trading_algorithm_adjust_windows .ipynb files.

---

## Evaluation Report

From the classification reports, it is shown that the svm model has a higher accuracy of 0.55 compared to the logistic regression model accuracy of 0.52. From the plots of the actual returns versus the strategy returns, we can see that the SVM model's strategy returns cross over the actual returns in 2018 and then stay above the actual returns through 2020. We also see in the plots that the Logistic Regression model's strategy returns cross over the actual returns in 2018 but then cross back under the actual returns in 2020.

Based on the classification reports and the plots of the actual returns versus the strategy returns, the SVM model is the better model between the two.

I subsequently changed the training window to a different period, from "2019-03-20 09:45:00" to "2019-06-20 09:45:00." This change resulted in a plot that appears to show less of a spread between the strategy returns and the actual returns in 2020. The original training window appears to be the better model.

I subsequently changed the short window to 50 days, and changed the training window back to that of the original model. This change resulted in a plot that appears to show the strategy returns perfectly aligning with the actual returns, versus the strategy returns being greater than the actual returns in 2020 in our original model. In addition, the updated model has "0.00" for precision and recall which is concerning. The original model is still the better model.

---

## Contributors

John P Weldon

Email: johnpweldon01@gmail.com

[LinkedIn:] (www.linkedin.com/in/john-weldon-333b0695)

---

## License

MIT

---