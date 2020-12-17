<template>
  <div class="px-2 font-ibm leading-tight">
    <!-- <div class="text-center">
      <input
        class="w-full h-12 bg-gray-200 text-gray-700 rounded shadow-md mt-10 px-4"
        placeholder="Search"
        type="text"
      />
    </div> -->
    <h1 class="mt-10 text-4xl">PROJECT</h1>

    <section>
      <h2 class="mt-2 font-semibold text-lg">모집중인 프로젝트</h2>
      <div class="mt-2 flex flex-wrap">
        <div
          v-for="item in items"
          :key="item.index"
          class="card m-1 shadow-md rounded"
        >
          <img class="w-full rounded-lg" src="@/assets/img/1.jpeg" alt="" />
          <div class="p-2">
            <p class="text-xs text-gray-600">{{ item.dev }}</p>
            <h2 class="text-sm text-gray-800">{{ item.title }}</h2>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'nuxt-property-decorator'

@Component({})
export default class MyClass extends Vue {
  data() {
    return {
      items: [
        {
          dev: 'APP',
          title: '계획부터 런칭까지 같이 시작하실 분 구합니다.',
          img: '@/assets/img/1.jpeg',
        },
        {
          dev: 'APP',
          title: '계획부터 런칭까지 같이 시작하실 분 구합니다.',
          img: '@/assets/img/2.jpeg',
        },
        {
          dev: 'APP',
          title: '계획부터 런칭까지 같이 시작하실 분 구합니다.',
          img: '@/assets/img/3.jpeg',
        },
        {
          dev: 'APP',
          title: '계획부터 런칭까지 같이 시작하실 분 구합니다.',
          img: '@/assets/img/4.jpeg',
        },
      ],
    }
  }
}
</script>

<style>
.card {
  width: calc(50% - 8px);
}
.img-wh {
  width: 224px;
  height: 224px;
}
</style>
