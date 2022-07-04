# Typora中使用TeX语法插入公式



## 行内公式

- 使用“\$”+“TeX公式代码“+”\$"进行输入，例如：$\begin{matrix}	0 & 1\\	1 & 0\end{matrix}$





## 公式块

- 使用“$$”+回车进入编辑模式，进入编辑模式后输入公式对应的Tex代码即可

$$
\frac{a}{2}
\\
\Sigma
\\
\Alpha_1
$$



## TeX 语法

### 上下标

#### 上标

- 使用 `^` 符号进行标记，注意在某些情况下需要添加`{}` 将所有上标囊括

#### 下标

- 使用 `_` 即下划线进行标记，同上标一样需要注意添加 `{}` 



### 希腊字母

- 使用 `\alpha` 、`\pi` 等表示小写希腊字母 $\alpha$ $\pi$

- 使用 `\Alpha` 、`\Pi` 等表示大写希腊字母 $\Alpha$ $\Pi$



### 数学函数

|     代码     | 对应数学函数 |
| :----------: | :----------: |
|    `\log`    |    $\log$    |
|    `\sin`    |    $\sin$    |
|    `\cos`    |    $\cos$    |
|  `\arcsin`   |  $\arcsin$   |
|  `\arccos`   |  $\arccos$   |
|    `\ln`     |    $\ln$     |
|  `\sqrt{}`   |  $\sqrt{}$   |
| `\sqrt[n]{}` | $\sqrt[n]{}$ |



### 分式表达

- 分式使用 `\frac{}{}` 函数，前一个 `{}` 内包含分子，后一个包含分母

- 示例
  $$
  \frac{3\pi}{4}
  $$

### 矩阵

- 使用matrix 环境编写矩阵

- 样例

  ```latex
  $$
  \begin{matrix}
  	0 & 1\\
  	1 & 0
  \end{matrix}
  % p 圆括号
  \begin{pmatrix}
  	0 & 1\\
  	1 & 0
  \end{pmatrix}
  % b 方括号
  \begin{bmatrix}
  	0 & 1\\
  	1 & 0
  \end{bmatrix}
  % B 大括号
  \begin{Bmatrix}
  	0 & 1\\
  	1 & 0
  \end{Bmatrix}
  % v 单竖线
  \begin{vmatrix}
  	0 & 1\\
  	1 & 0
  \end{vmatrix}
  % V 双竖线
  \begin{Vmatrix}
  \dots & \vdots\\
  	\ddots & -i
  \end{Vmatrix}
  
  $$
  ```

  效果如下
  $$
  \begin{matrix}
  	0 & 1\\
  	1 & 0
  \end{matrix}
  \begin{pmatrix}
  	0 & 1\\
  	1 & 0
  \end{pmatrix}
  \begin{bmatrix}
  	0 & 1\\
  	1 & 0
  \end{bmatrix}
  \\\\
  \begin{Bmatrix}
  	0 & 1\\
  	1 & 0
  \end{Bmatrix}
  \begin{vmatrix}
  	0 & 1\\
  	1 & 0
  \end{vmatrix}
  \begin{Vmatrix}
  	\dots & \vdots\\
  	\ddots & -i
  \end{Vmatrix}
  $$
  
