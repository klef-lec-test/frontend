<template>
  <div>
    <h1>1. HTMLのタグとその役割</h1>
    <p>ここでは、さまざまなHTMLのタグとその役割について説明します。</p>
    <h2>h1〜h6タグ</h2>
    <p>h1〜h6タグは、見出しを表します。<br>h1タグが最も大きく、h6タグが最も小さいです。<br>h1タグによって定義される見出しを<b>第1レベル</b>見出し、h6タグによって定義される見出しを<b>第6レベル</b>見出しといいます。</p>
    <Example>
      <h1>第1レベル</h1>
      <h2>第2レベル</h2>
      <h3>第3レベル</h3>
      <h4>第4レベル</h4>
      <h5>第5レベル</h5>
      <h6>第6レベル</h6>
    </Example>
    <h2>pタグ</h2>
    <p>pタグは、段落、もとい本文を表します。ParagraphのPです。<br>HTMLのタグの中で一番よく使うタグです。</p>
    <h2>brタグ</h2>
    <p>brタグは、その場所での改行を表します。終了タグは必要ありません。</p>
    <h2>strongタグ・bタグ</h2>
    <p>strongタグとbタグは、ともに<strong>太字</strong>を表すタグです。<br>CSSで代用可能なので、できるだけCSSを使いましょう。</p>
    <h2>iタグ</h2>
    <p>iタグは<i>斜体(イタリック体)</i>を表すタグです。<br>こちらもCSSで代用可能なので、できるだけCSSを使いましょう。</p>
    <h2>uタグ</h2>
    <p>uタグは<u>アンダーライン</u>を表すタグです。<br>非推奨なのでCSSを使いましょう。</p>
    <h2>sタグ・strikeタグ・delタグ</h2>
    <p>sタグ・strikeタグは<s>取り消し線</s>を示すタグです。<br>delタグは<del>削除部分</del>を示すタグです。<br>どちらも非推奨なので、CSSを使いましょう。</p>
    <h2>tableタグ・trタグ・thタグ・tdタグ</h2>
    <p>これらのタグは、表を構成するタグです。<br>場合によってはtheadタグ・tbodyタグ・tfootタグも使われます。</p>
    <Example>
      <table>
        <thead>
          <tr>
            <th>Header1</th>
            <th>Header2</th>
            <th>Header3</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>Body1-1</td>
            <td>Body1-2</td>
            <td>Body1-3</td>
          </tr>
          <tr>
            <td>Body2-1</td>
            <td>Body2-2</td>
            <td>Body2-3</td>
          </tr>
        </tbody>
      </table>
    </Example>
    <h2>divタグ</h2>
    <p>divタグは、HTMLの一部を切り出して、その一部に対してclassなどを個別に設定するタグです。</p>
    <h2>spanタグ</h2>
    <p>spanタグは、ある要素の中身の一部を切り出して、個別にclassなどを設定するタグです。</p>
    <h2>imgタグ</h2>
    <p>imgタグは画像を表示するタグです。リンクになっているのでリンク切れを起こす可能性があります。<br>そのときには"alt"属性に設定されている代替テキストが表示されます。また、終了タグはありません。</p>
    <h2>buttonタグ</h2>
    <p>buttonタグは、ボタンを表すタグです。タグに囲まれた文字がボタンの中身として表示されます。</p>
    <Example>
      <button>Button</button>
    </Example>
    <h2>inputタグ</h2>
    <p>inputタグはさまざまなフォームの入力部品をかけるタグです</p>
    <h2>formタグ</h2>
    <p>フォームの範囲を指定するタグです</p>
    <h2>labelタグ</h2>
    <p>inputタグに対応するラベルを定義するタグです。</p>
    <Example>
      <form>
        <label for="btn1">button</label>
        <input type="button" value="button1" name="btn1" />
        <br />
        <label for="chk1">checkbox</label>
        <input type="checkbox" name="chk1" />
        <br />
        <label for="clr1">color</label>
        <input type="color" name="clr1" />
        <br />
        <label for="date1">date</label>
        <input type="date" name="date1" />
        <br />
        <label for="dtm1">datetime-local</label>
        <input type="datetype-local" name="dtm1" />
        <br />
        <label for="eml1">email</label>
        <input type="email" name="eml1" />
        <br />
        <label for="file1">file</label>
        <input type="file" name="file1" />
        <br />
        <label for="hdn1">hidden</label>
        <input type="hidden" name="hdn1" />
        <br />
        <label for="img1">image</label>
        <input type="image" name="img1" />
        <br />
        <label for="mnt1">month</label>
        <input type="month" name="mnt1" />
        <br />
        <label for="nmb1">number</label>
        <input type="number" name="nmb1" />
        <br />
        <label for="pwd1">password</label>
        <input type="password" name="pwd1" />
        <br />
        <label for="rdo1">radio</label>
        <input type="radio" name="rdo1" />
        <br />
        <label for="rng1">range</label>
        <input type="range" name="rng1" />
        <br />
        <label for="src1">search</label>
        <input type="search" name="src1" />
        <br />
        <label for="tel1">tel</label>
        <input type="tel" name="tel1" />
        <br />
        <label for="txt1">text</label>
        <input type="text" name="txt1" />
        <br />
        <label for="url1">url</label>
        <input type="url" name="url1" />
        <br />
        <input type="submit" value="submit" />
        <input type="reset" value="clear" />
      </form>
    </Example>
    <h2>aタグ</h2>
    <p>aタグは、リンクを設定するタグです。<br />href属性にリンク先を設定します。</p>
    <Example>
      <a href="#">このページ自体のリンク</a><br />
      <a href="/html"><button>見本ページへのリンク</button></a>
    </Example>
    <h2>ulタグ・olタグ・liタグ</h2>
    <p>ulタグとolタグ・liタグは、箇条書きを設定するタグです。</p>
    <Example>
      <p>ulタグ</p>
      <ul>
        <li>item1</li>
        <li>item2</li>
        <li>item3</li>
      </ul>
      <p>olタグ</p>
      <ol>
        <li>item1</li>
        <li>item2</li>
        <li>item3</li>
      </ol>
    </Example>
    <div class="sample" id="sample">
      <h2>Sample Page</h2>
      <form>
        <label for="txt2">User Name</label>
        <input type="text" name="txt2" v-model="id" />
        <br />
        <label for="pwd2">Password</label>
        <input type="password" name="pwd2" v-model="pwd" />
        <br />
        <input type="submit" value="Login" @click="login(id,pwd)" />
        <input type="reset" value="Clear" />
      </form>
      <br>
      <p>デフォルトの認証情報は以下のとおりです。</p>
      <table>
        <tbody>
          <tr>
            <th>User Name</th>
            <td>Admin</td>
          </tr>
          <tr>
            <th>Password</th>
            <td>Password</td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</template>

<style>
.sample{
  border: 4px solid #16a34a;
  padding: 4px;
  margin: 4px;
}
.sample h2{
  background: linear-gradient(transparent 60%, #7dd3fc60 30%);
}
.sample label{
  width: 6em;
  display: inline-block;
}
table,tr,th,td{
  border-collapse: collapse;
  border: 1px solid #000000;
  margin: 2px;
}
</style>

<script>
  import Vue from "vue";
  export default {
    el: "#sample",
    data() {
      return {
        id: "",
        pwd: ""
      }
    },
    methods: {
      login: function(id, pwd) {
        if (id == "Admin" && pwd == "Password") {
          alert("Login Successful!")
        }else{
          alert("Login Failed")
        }
      }
    }
  }
</script>

