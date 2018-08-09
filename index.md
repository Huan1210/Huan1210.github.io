## 欢迎访问我的博客

从今天开始，要好好学习编程，在这里记录学习的足迹。

### 1、用Python生成器实现杨辉三角              ----2018/8/9

```markdown

# 期待输出:
# [1]
# [1, 1]
# [1, 2, 1]
# [1, 3, 3, 1]
# [1, 4, 6, 4, 1]
# [1, 5, 10, 10, 5, 1]
# [1, 6, 15, 20, 15, 6, 1]
# [1, 7, 21, 35, 35, 21, 7, 1]
# [1, 8, 28, 56, 70, 56, 28, 8, 1]
# [1, 9, 36, 84, 126, 126, 84, 36, 9, 1]


# 定义函数
def triangle():
  N = [1]
  while True:
    yield N
    N.append(0)
    N = [ N[i-1] + N[i] for i in range(len(N))]

n = 0
results = []
for t in trianglel():
  print(i)
  results.append(i)
  n += 1
  if n == 0:
    break
    
```
