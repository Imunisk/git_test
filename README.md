### 표본분산

<p>$$\tt \sigma^{2}=\frac{1}{N}\sum_i^N(x_{i}-\mu)^{2}$$</p>

### 표준편차

<p>$$\sigma=\sqrt{\sigma^{2}}=\sqrt{\frac{1}{N-1}\sum_i^N(x_{i}-\mu)^{2}}$$</p>

### 공분산행렬

<p>$$Cov(x,y)=\begin{bmatrix}\sigma_{x}^{2} &amp; Cov(x,y) \\Cov(x,y) &amp; \sigma_{y}^{2} \end{bmatrix}$$</p>

### 상관행렬

<p>$$\tt Cov(x,y)=\begin{bmatrix}1 &amp; \rho_{xy} \\\rho_{xy} &amp; 1 \end{bmatrix}$$</p>

### 표준오차

<p>$$&#54364;&#51456;&#50724;&#52264;=\frac{\sigma}{\sqrt{N}}$$</p>


```python
# 링크사이트
# 테이블 하나
# 이미지 출력, 동영상
# 코드 출력
```

#### 링크사이트
레이텍 공식 링크 ==>   [Equation Editor](https://editor.codecogs.com/)  
깃허브 HTML 리드미 ==>   [Read Me]('https://github.com/microsoft/Web-Dev-For-Beginners?tab=readme-ov-file#readme')


```python
# 테이블 출력
import pandas as pd
exam = pd.read_csv('D:/data/CSV_example.csv')
exam.head()
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>id</th>
      <th>nclass</th>
      <th>math</th>
      <th>english</th>
      <th>science</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>1</td>
      <td>1</td>
      <td>50</td>
      <td>98</td>
      <td>50</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2</td>
      <td>1</td>
      <td>60</td>
      <td>97</td>
      <td>60</td>
    </tr>
    <tr>
      <th>2</th>
      <td>3</td>
      <td>1</td>
      <td>45</td>
      <td>86</td>
      <td>78</td>
    </tr>
    <tr>
      <th>3</th>
      <td>4</td>
      <td>1</td>
      <td>30</td>
      <td>98</td>
      <td>58</td>
    </tr>
    <tr>
      <th>4</th>
      <td>5</td>
      <td>2</td>
      <td>25</td>
      <td>80</td>
      <td>65</td>
    </tr>
  </tbody>
</table>
</div>




```python
import seaborn as sns
import matplotlib.pyplot as plt
sns.countplot(data=exam, x='english', hue='nclass')
plt.show()
```


    
![png](output_13_0.png)
    



```python
sns.scatterplot(data=exam, x='english', y='math', hue='nclass')
```




    <Axes: xlabel='english', ylabel='math'>




    
![png](output_14_1.png)
    



```python
# 씨본 로고 출력
# https://seaborn.pydata.org/_images/logo-tall-lightbg.svg
# <a href="url"><img src="이미지경로" border="0"></a>
```

<a href="url"><img src="https://matplotlib.org/devdocs/_static/logo_light.svg" width="400" height="100"></a>

<a href="url"><img src="https://seaborn.pydata.org/_images/logo-tall-lightbg.svg" border="0"></a>
