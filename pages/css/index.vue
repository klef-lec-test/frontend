<template>
  <div>
    <h1>2 CSSによるスタイリング</h1>
    <h2>2.1 font</h2>
    <p>fontは、フォントや文字サイズなどの一括設定プロパティです。</p>
    <Example>
      <p class="text-lg">18px</p>
      <p class="text-xl">1.5em</p>
    </Example>
    <h2>2.2 border</h2>
    <p>borderは、枠線を設定するプロパティです。</p>
    <Example>
      <div class="border">
        [MEMO]margin、paddingはともに10pxです。<br/>
        borderの色はblueで、幅は2pxです。
      </div>
    </Example>
    <h2>2.3 color</h2>
    <p>colorは、文字の色を設定するプロパティです。</p>
    <Example>
      <p class="red">Red</p>
      <p class="blue">Blue</p>
      <p class="green">Green</p>
    </Example>
    <h2>2.4 padding</h2>
    <p>paddingは、borderの内側のコンテンツまでのすき間を設定するプロパティです。</p>
    <Example>
      <p class="padding-5">padding:5px</p>
      <p class="padding-10">padding:10px</p>
    </Example>
    <h2>2.5 margin</h2>
    <p>marginは、borderの外側のすき間を設定するプロパティです。</p>
    <Example>
      <p class="margin-5">margin: 5px</p>
      <p class="margin-10">margin: 10px</p>
    </Example>
    <h2>2.6 text-align</h2>
    <p>text-alignは、テキストの揃え位置を設定するプロパティです。</p>
    <Example>
      <p class="start">行頭揃え</p>
      <p class="end">行末揃え</p>
      <p class="center">中央揃え</p>
    </Example>
    <h2>2.7 子孫結合子</h2>
    <p>子孫結合子は、入れ子構造になっている親要素のクラスなどの中にある特定の子要素にスタイルを適用する時に使います。</p>
    <Example>
      <div class="children">
        <p>親要素(div)にクラスを設定</p>
        <label>labelにstyleを設定</label>
      </div>
      <label>divの外のlabelには設定されない</label>
    </Example>
    <h2>2.8 :hover</h2>
    <p>:hoverはCSS擬似クラスの1つで、ホバー(マウスオーバー)時に適用するスタイルを設定できます。</p>
    <Example>
      <p class="hover">ホバーすると下線が表示されます。</p>
    </Example>
  </div>
</template>

<style>
.text-lg{
  font-size: 18px;
}
.text-xl{
  font-size: 1.5em;
}
.border{
  border: 2px solid #0000FF;
  margin: 10px;
  padding: 10px;
}
.red{
  color: #FF0000;
}
.blue{
  color: #0000FF;
}
.green{
  color: #00FF00;
}
.padding-5{
  border: 2px solid #0000FF;
  padding: 5px;
}
.padding-10{
  border: 2px solid #0000FF;
  padding: 10px;
}
.margin-5{
  border: 2px solid #0000FF;
  margin: 5px;
}
.margin-10{
  border: 2px solid #0000FF;
  margin: 10px;
}
.start{
  text-align: start;
}
.end{
  text-align: end;
}
.center{
  text-align: center;
}
.children label{
  color: #0000FF;
}
.hover:hover{
  border-bottom: 2px solid #00FFFF;
}
h1{
  border-left: 5px solid #c7d2fe;
  border-bottom: 5px solid #818cf8;
  padding: 2px 6px;
}
h2{
  border-left: 3px solid #fb7185;
  padding: 2px 6px;
}
</style>
