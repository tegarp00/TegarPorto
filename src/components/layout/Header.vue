<template>
  <div class="dizme_tm_header">
    <div class="container">
      <div class="inner">
        <div class="logo">
          <a href="#"
            ><img :src="`img/logo/${dark ? 'dark' : 'logo'}.png`" alt=""
          /></a>
        </div>
        <div class="menu">
          <ul class="anchor_nav">
            <li class="current"><a href="#home">Home</a></li>
            <li><a href="#portfolio">Portfolio</a></li>
            <li><a href="#service">Service</a></li>
            <li>
              <a href="https://medium.com/@TegarPratamaa" target="_blank"
                >Blog</a
              >
            </li>
            <!-- <li>
              <a href="https://wa.me/6285761652392" target="_blank">Whatsapp</a>
            </li>
            <li>
              <a
                href="https://www.linkedin.com/in/tegar-pratama-21a885213/"
                target="_blank"
                >Linkedin</a
              >
            </li> -->
            <li>
              <a
                href="https://www.upwork.com/freelancers/~019b2ef6d52ddd90a0?mp_source=share"
                target="_blank"
                >Upwork</a
              >
            </li>
            <!-- <li><a href="mailto:mail.tegarp00@gmail.com">Email Me</a></li> -->
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HeaderVue",
  props: {
    dark: { type: Boolean },
  },
};
</script>
