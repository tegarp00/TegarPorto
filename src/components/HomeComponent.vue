<template>
  <div class="dizme_tm_section" id="home">
    <div class="dizme_tm_hero">
      <div
        class="background"
        :data-img-url="`/img/slider/${dark ? 2 : 3}.jpg`"
      ></div>
      <div class="container">
        <div class="content">
          <div class="details">
            <div class="hello">
              <h3 class="navyText"><strong>Hello, I am</strong></h3>
            </div>
            <div class="name">
              <h3>Tegar Pratama</h3>
            </div>
            <div class="job">
              <p>
                A <span class="">Fullstack Developer</span> From
                <span class="">Indonesia</span>
              </p>
            </div>
            <div class="text">
              <p class="navyText">
                A seasoned Full Stack Developer with over 5 years of expertise. I've successfully delivered 150+ projects, specializing in crafting robust web applications and custom solutions.
              </p>
            </div>
            <!-- <div class="button">
              <div class="dizme_tm_button">
                <a class="anchor" href="https://wa.me/6285761652392" target="_blank"><span>Whatsapp</span></a>
              </div>
            </div> -->
          </div>
          <div class="avatar">
            <div class="image">
              <img src="/img/slider/avatar2.png" alt="" />
              <span
                class="skills illustrator anim_moveBottom"
                v-html="htmlIcon"
              ></span>
              <span class="skills photoshop anim_moveBottom" v-html="cssIcon"></span>
              <span class="skills figma anim_moveBottom" v-html="jsIcon"></span>
            </div>
          </div>
        </div>
      </div>
      <div class="dizme_tm_down">
        <a class="anchor" href="#portfolio" v-html="dark ? mouseDark : mouse">
        </a>
      </div>
    </div>
  </div>
</template>

<script>
import { ai, cssIcon, figma, htmlIcon, mouse, mouseDark, ps, jsIcon } from "../svg";
export default {
  name: "HomeComponent",
  data() {
    return { ai, ps, figma, mouse, mouseDark, htmlIcon, cssIcon, jsIcon };
  },
  props: {
    dark: { type: Boolean },
  },
};
</script>