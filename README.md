# 핸드폰 사용량에 따른 탄소배출량 수집 웹페이지

사용된 언어 : HTML, CSS, Javascript

![IMG_6368](https://github.com/user-attachments/assets/b1aa3a35-c211-49d8-a3f5-68d14b6be445)

# 표준분포 그래프 출력 코드
```python
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns

data = [] # 데이터 읽기

# 평균값, 표준편차
avg = np.mean(data)
std_dev = np.std(data)

# 히스토그램, KDE Plot 표현
plt.figure(figsize=(10, 6))
sns.histplot(data, kde=True, stat="density", bins=40, color="green", linewidth=0.5)

# 그래프, 축 제목
plt.title('Data Distribution')
plt.xlabel('Value')
plt.ylabel('Density')

# 평균값 수직선으로 표현
plt.axvline(mean, color='red', linestyle='--', label=f'Average: {avg:.2f}')
plt.legend()

# 그래프 출력
plt.show()

```
![ed12e088-49bc-423b-abe2-de35c7572689](https://github.com/user-attachments/assets/d19435cc-b23c-472a-b25e-a2b601ceb5a7)
