# section 11

## 修正内容

1. 画像のhoverが余計なところで反応している。(TAB,SP時)
   - widthとmarginで中央寄せにし、hoverのバグを修正。
   ```css
    .content__item {
      width: 300px;
       margin: 0 auto;
    }
   ```
2. ヘッダー部分でleft(or right)がなく、topだけのpositionになっている。
  - `left: 0;`を追加し、Y軸でもpositionをとった。

3. ヘッダーの`z-index`を他が追加されることを見込んで `z-index:999;`にする。
   - `z-index`の値を10から999にして修正。

4. aタグのtext-underline:noneを reset css へ書く
  - reset css へ aタグのデフォルト設定。
  ```css
  a {
    text-decoration: none;
  }
  ```

5. margin-bottomがかかって余分な余白ができている。「WHAT WE CAN DO?」
  - `margin: 0 0 20px 0;`を`margin: 0;`へ修正

6. 画像を上の方にだけ余白(margin)開けないと、画像を追加した時に影響してしまう。
  - 最初の三つmargin-top:0;にし、残りの三つをmargin-tpoで余白を開けました。TAB用SP用も見本通りに修正しました。

7. global-thumbのスタイル が重複している。
   - TAB用とSP用でスタイルを当てていたので削除。

8. ハンバーガーメニュに`cursor:pointer`があたっている。navタグはdivではなく、spanタグでやる。
   - `cursor:pointer`を削除し、`header-bar-line`を当てていたdivタグをspanタグ変更