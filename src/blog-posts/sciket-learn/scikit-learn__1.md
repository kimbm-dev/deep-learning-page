---
title: 'scikit-learn'
date: '2018-11-23'
tags: ['Python']
---

これから scikit-learn の練習をします。このレポジトリーはそれの記録を撮りために作成しました。

# NumPy

NumPy は、Python で科学技術計算をする際の基本的なツールの 1 つである。
多次元配列機能や、線形代数やフーリエ変換、擬似乱数生成器（ぎじるいらんすうせいせいき）などの、高レベルの数学関数が用意されている。

NumPy の使い方

```python
import numpy

x = numpy.array([[1, 2, 3], [4, 5, 6]])
print("x:\n{}".format(x))

# 結果
# x:
#  [[1 2 3]
#   [4 5 6]]
```

scikit-learn では NumPy の ndarray クラス沢山使いますって、？

# SciPy

SciPy は、Python で科学技術計算を行うための関数を集めたものです。高度な線形代数ルーチンや、数学関数の最適化、信号処理、特殊な数学関数、統計分布などの機能を持ちます。scikit-learn は、アルゴリズムを実装する際に SciPy の関数群を利用しています。我々にとって最も重要な SciPy の要素は、scipy.sparse（疎行列：sparse matrix）であります。

```python
from scipy import sparse
import numpy

# 対角成分が１でそれ以上が0の、２次元NumPy配列を作る
eye = numpy.eye(4)
print("NumPy array:\n{}".format(eye))

# 結果
# NumPy array:
# [[1. 0. 0. 0.]
#  [0. 1. 0. 0.]
#  [0. 0. 1. 0.]
#  [0. 0. 0. 1.]]
```
