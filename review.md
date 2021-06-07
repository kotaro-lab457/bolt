# section 11

## 修正内容

1. コンテンツ幅の指定の幅がない。所々（Bolt Themeのセクション）また、共通スタイルを作成する。
    - コンテンツ幅の指定をし、共通クラス(`contents`)を作成しました。それぞれのセクションにクラス名を追加しました。
    ```css
    .contents {
      width: 1100px;
      margin: 0 auto;
     }
    ```

2. 画像とテキストを`margin-bottom`ではなく、`margin-top`で距離を取る形でやる！（全体）
    - それぞれのテキスト、画像を`margin-top`での距離を取りました。

3. 「WHAT WE CAN DO?」と「OUT LATEST WORK」 のテキストの幅を固定ではなく伸縮させる。
    - width: 650px; 👉 width: 60%; 「WHAT WE CAN DO?」
    - width: 580px; 👉 width: 53%; 「OUT LATEST WORK」

4. フォントファミリーをbodyで作成する。（共通）
   - css にbodyを作成し、共通化。
   ```css
   body {
     font-family: "Raleway", sans-serif;
   }
   ```
5. what we　、、、 `margin-top`で距離をを取る。（少し余白がある。）
   -  レスポンシブ時を見込み`margin-top: 20px;`で取りました。

6. `is-content` の`margin-bottom`を省く。。
   - `margin-bottom`を外し、兄弟要素の下のクラスに`margin-top`を使用して距離をとった。

7. ul liタグを使う。画像、SNS
   - 順序がある型式になるので、divタグをul,liタグへ修正。（画像,SNSボタン）
   - また、cssでの共通スタイルの追加。
   ```css
   ul {
     list-style: none;
   }
   ```