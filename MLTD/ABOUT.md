# シアターデイズCSS

## button.css

ボタン要素のCSSです

以下のセレクタで構成されます

|セレクタ|用途|
|:--|:--|
|.button|ボタン要素|
|.button:hover|ボタンをホバー(カーソルを載せた)状態|
|.button:active|ボタンをクリックorタップした状態|

以下はオプションです

|セレクタ|用途|
|:--|:--|
|.il|ボタンをインラインブロックにします|

.il はボタンに説明を加えるためなどでボタン内が二行以上になる場合に活用できます [使用例(MediaSearchセクション)](https://millionlive.miyacorata.net/idol?name=matsuritokugawa)

### HTMLコード例
```html
<a href="#" class="button">普通のボタン</a>

<a href="#" class="button il">インラインブロックボタン<br>改行を含むことができます</a>
```

## list.css

アイコン込みのリスト要素のCSSです(li要素ではありません)

以下のセレクタで構成されます

|セレクタ|用途|
|:--|:--|
|.idol|親要素になります|
|.idol p|子のp要素|
|.idolicon|リスト内のアイコン|
|.idolinfo|リスト内の説明文等|
|.idolinfo .name|リスト内のタイトル(アイドル名)|
|.idol a, .idol a:hover|リンク色の定義|
|.idol a:visited|リンク色の定義(訪問済み)|

```html
<div class="idol">
    <img src="/path/to/icon.png" class="idolicon">
    <div class="idolinfo">
        <p class="name">徳川まつり</p>
        <p>
            ここにちょっとした説明とかを入力するのです。...ね？
        </p>
    </div>
</div>
```

## msgbox.css

メッセージボックス要素のCSSです

以下のセレクタで構成されます

|セレクタ|用途|
|:--|:--|
|.msgbox|メッセージボックスの親要素|
|.msgboxtop|タイトルバー|
|.msgboxtop::before|タイトルバー左端のあれ|
|.msgboxbody|本文 メイン部分|
|.msgboxfoot|下部ボタン部分(閉じるボタンとか)|

top,body,footはmsgboxの子要素でなければなりません。

### HTMLコード例
```html
<div class="msgbox">
    <div class="msgboxtop">タイトルバー</div>
    <div class="msgboxbody">
        <h3>メイン要素</h3>
        <p>ここに段落等任意の要素を置くことができます</p>
    </div>
    <div　class="msgboxfoot">
        <a href="#" class="button">ここにボタンを置けます</a>
    </div>
</div>
```

