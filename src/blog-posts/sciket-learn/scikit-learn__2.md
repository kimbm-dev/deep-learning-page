---
title: 'scikit-learn 2'
date: '2018-11-23'
tags: ['Python']
---

# SciPy

SciPy は、Python で科学技術計算を行うための関数を集めたものです。高度な線形代数ルーチンや、数学関数の最適化、信号処理、特殊な数学関数、統計分布などの機能を持ちます。scikit-learn は、アルゴリズムを実装する際に SciPy の関数群を利用しています。我々にとって最も重要な SciPy の要素は、scipy.sparse（疎行列：sparse matrix）であります。

## 使い方

SciPy は

## COO 形式

### コード

```python
from scipy import sparse
import numpy

data = numpy.ones(4)
row_indices = numpy.arange(4)
col_indices = numpy.arange(4)

eye_coo = sparse.coo_matrix((data, (row_indices, col_indices)))
print("COO representation:\n{}".format(eye_coo))
```

### 結果

```python
COO representation:
  (0, 0)  1.0
  (1, 1)  1.0
  (2, 2)  1.0
  (3, 3)  1.0
```
