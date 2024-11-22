クワイン（Quine）とは、コンピュータプログラムの一種で、自身のソースコードと完全に同じ文字列を出力するプログラムを指します。 この名称は、自己参照に関する研究で知られる哲学者ウィラード・ヴァン・オーマン・クワインに由来しています。

**クワインの特徴:**

- **自己複製:** クワインは、実行時に自分自身のソースコードをそのまま出力します。
- **入力不要:** 外部からの入力やファイルの読み込みを行わず、プログラム内部のみで自己出力を実現します。
- **メタプログラミング:** 自身のコードを出力する性質から、メタプログラミングの一種とされています。

**クワインの例（Pythonの場合）:**

```python
s = 's = {!r}\nprint(s.format(s))'
print(s.format(s))
```

このプログラムを実行すると、以下のように自身のソースコードを出力します。

```
s = 's = {!r}\nprint(s.format(s))'
print(s.format(s))
```

**注意点:**

- **チート的解法の除外:** ソースコードを直接読み込んで出力する方法や、空のプログラムが何も出力しないことを利用する方法などは、クワインとは見なされません。