<template>
  <div>
  <!-- ここの間にHTMLを書いてください --->
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
      return{
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

