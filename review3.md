# section11

## 修正内容

1. headerのaタグがflexの影響でブロック要素（垂直）になってしまうので、`align-items`でアイコンと揃える必要がある。
   - `align-item:start`でブロック要素を上に揃えました。

2. ６つの画像にも、aタグをあてる必要がある。`<a href=""></a>`のhrefに「#」をあてる。
   - 画像（imgタグ）をaタグで囲いました。また、aタグのhref全てに「#」をあてました。

3. 本来aタグ要素は、`inline`要素になっているので`display:inline-block;`で親要素の値を引き継いでいく。
  - aタグに`display:inline-block;`を当て、ブロック要素化させました。