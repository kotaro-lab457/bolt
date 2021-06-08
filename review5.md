# section11 bolt TAB,SP用

## 修正内藤

1. 画像をひとつ（七枚目）を足してしまうとmargin-topでの余白が取れていない。
  -  child指定を4番目,7番目を指定して余白を開けるようにしました。
  ```css
  461行目
  .content__item:nth-child(3n + 4) {
    margin-top: 80px;
  }

  ```