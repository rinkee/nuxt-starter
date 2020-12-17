<template>
  <div class="container mx-auto max-w-sm">
    <header class="p-4 justify-between">
      <nuxt-link to="/">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          width="45"
          height="35.185"
          viewBox="0 0 45 35.185"
        >
          <g
            id="그룹_14"
            data-name="그룹 14"
            transform="translate(-34 -59.022)"
          >
            <text
              id="Project_Studio"
              data-name="Project
Studio"
              transform="translate(34 73)"
              font-size="12"
              font-family="GmarketSansTTFLight, Gmarket Sans TTF"
              letter-spacing="0.07em"
            >
              <tspan x="0" y="0">Project</tspan>
              <tspan x="0" y="16">Studio</tspan>
            </text>
            <g
              id="그룹_1"
              data-name="그룹 1"
              transform="translate(-44.604 -58.771)"
            >
              <path
                id="패스_3"
                data-name="패스 3"
                d="M0,0H35.312"
                transform="translate(82.085 123.5)"
                fill="none"
                stroke="#fe725b"
                stroke-linecap="round"
                stroke-width="1"
              />
              <path
                id="패스_5"
                data-name="패스 5"
                d="M5,0,0,5"
                transform="translate(117.397 118.5)"
                fill="none"
                stroke="#fe725b"
                stroke-linecap="round"
                stroke-width="1"
              />
              <path
                id="패스_2"
                data-name="패스 2"
                d="M0,27.5V0"
                transform="translate(117.397 124.271)"
                fill="none"
                stroke="#fe725b"
                stroke-linecap="round"
                stroke-width="1"
              />
              <path
                id="패스_6"
                data-name="패스 6"
                d="M5,0,0,5"
                transform="translate(117.397 147.271)"
                fill="none"
                stroke="#fe725b"
                stroke-linecap="round"
                stroke-width="1"
              />
              <path
                id="패스_4"
                data-name="패스 4"
                d="M0,0V27.5"
                transform="translate(81.5 124.271)"
                fill="none"
                stroke="#fe725b"
                stroke-linecap="round"
                stroke-width="1"
              />
            </g>
          </g>
        </svg>
      </nuxt-link>
      <ul class="mt-3 flex justify-between">
        <li v-for="nav in navLinks" :key="nav.index">
          <nuxt-link :to="nav.to" class="text-sm font-ibm font-semibold">
            {{ nav.text }}
          </nuxt-link>
        </li>
      </ul>
    </header>
    <Nuxt />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'nuxt-property-decorator'

@Component({})
export default class MyClass extends Vue {
  data() {
    return {
      navLinks: [
        { to: '/', text: 'Home' },
        { to: '/project', text: 'Project' },
        { to: '/readme', text: 'Readme' },
        { to: '/user', text: 'User' },
        { to: '/login', text: 'Login' },
      ],
    }
  }
}
</script>
