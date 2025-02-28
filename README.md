# DQN-Recommender-with-Gemini

## توضیحات (فارسی)
این پروژه یک سیستم توصیه‌گر مبتنی بر یادگیری تقویتی است که از الگوریتم **Deep Q-Network (DQN)** استفاده می‌کند. این سیستم بر روی دیتاست **MovieLens 100K** آموزش داده شده است، که شامل امتیازات کاربران به فیلم‌ها می‌باشد. همچنین از **API Gemini** برای تحلیل مقادیر Q و ارائه توضیحات استفاده شده است. هدف این پروژه، توصیه آیتم‌ها (فیلم‌ها) به کاربران بر اساس ترجیحات آن‌ها است.

### اجزای اصلی
- **دیتاست**: زیرمجموعه‌ای از MovieLens 100K با 10 کاربر و آیتم‌های مرتبط.
- **محیط**: یک محیط سفارشی مبتنی بر **Gym** که کاربران و آیتم‌ها را مدل می‌کند.
- **عامل**: یک عامل DQN که یاد می‌گیرد کدام آیتم‌ها را به کاربران پیشنهاد دهد.
- **تحلیل**: استفاده از API Gemini برای تحلیل ماتریس Q-values و ارائه توضیحات.

## نحوه اجرا (فارسی)
برای اجرای این پروژه، مراحل زیر را دنبال کنید:

1. **پیش‌نیازها**:
   - Python 3.x
   - نصب کتابخانه‌های مورد نیاز: `numpy`, `pandas`, `gym`, `tensorflow`, `seaborn`, `matplotlib`, `requests`

2. **نصب کتابخانه‌ها**:
   ```bash
   pip install numpy pandas gym tensorflow seaborn matplotlib requests



DQN-Recommender-with-Gemini
Description (English)
This project is a reinforcement learning-based recommender system utilizing the Deep Q-Network (DQN) algorithm. It is trained on the MovieLens 100K dataset, which contains user ratings for movies. The system also leverages the Gemini API to analyze Q-values and provide insights. The goal is to recommend items (movies) to users based on their preferences.

Main Components
Dataset: A subset of MovieLens 100K with 10 users and related items.
Environment: A custom Gym-based environment modeling users and items.
Agent: A DQN agent that learns to recommend items to users.
Analysis: Utilization of the Gemini API to analyze the Q-values matrix and generate explanations.
How to Run (English)
To run this project, follow these steps:
Prerequisites:
```Python 3.x
Required libraries: numpy, pandas, gym, tensorflow, seaborn, matplotlib, requests
Install Libraries**:
```
```bash
pip install numpy pandas gym tensorflow seaborn matplotlib requests
```
Run the Code:
Save the code in a file named main.py.
Execute the following command in the terminal:
 ```bash
python main.py
```
Outputs:
A heatmap of Q-values for each user and item will be displayed.
The analysis from the Gemini API will be printed in the console.
Results (English)
Heatmap: A visual representation of Q-values indicating the value of each item for each user.
Gemini API Analysis: Insights and explanations provided by the Gemini API about patterns in the heatmap.
