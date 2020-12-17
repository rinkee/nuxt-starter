<template>
  <div class="px-2 font-ibm leading-tight">
    <h1 class="mt-10 text-4xl">LOG IN</h1>

    <section class="text-center">
      <div class="mt-2 py-4">
        <input type="text" placeholder="Email" class="input-1" />

        <input class="input-1" type="password" placeholder="Password" />

        <div class="text-center">
          <button class="input-2">로그인</button>
        </div>
      </div>
      <div class="mt-10 text-gray-300 text-sub">
        <span class="px-2">회원가입</span>
        <span class="px-2">아이디 찾기</span>
        <span class="px-2">비밀번호 찾기</span>
      </div>
    </section>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'nuxt-property-decorator'

@Component({})
export default class MyClass extends Vue {}
</script>

<style>
.input-1 {
  width: 270px;
  height: 45px;
  margin: 10px 0px;
  padding: 0 0 0 10px;
  border-radius: 10px;
  font-size: 14px;
  background-color: #f7f7f7;
  box-shadow: #d3d3d3 2px 3px 8px 1px;
}

.input-2 {
  width: 270px;
  height: 50px;
  margin-top: 30px;
  border-radius: 10px;
  background-color: #eb5c60;
  color: #f7f7f7;
  font-size: 26px;
  box-shadow: #d3d3d3 2px 3px 8px 1px;
}

.spac {
}
</style>
