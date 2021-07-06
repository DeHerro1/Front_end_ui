<template>
  <div class="nav">
    <div class="logo">
      <BookOpenBlankVariant class="nav_logo"></BookOpenBlankVariant>
      <p>veryfy</p>
    </div>
    <div class="nav_list_container">
      <ul class="nav-ul">
        <li>Home</li>
        <li>How it works</li>
        <li>FAQ</li>
        <li>Contact</li>
        <li class="text-success">Login</li>
        <li><button class="btn" id="get_started">Get Started</button></li>
      </ul>
    </div>
    <div @click="showNav" class="collapse_nav">
      <div></div>
      <div></div>
      <div></div>
    </div>
    <div v-show="isVisible" class="closeDiv" @click.self="closeNav">
      <div class="show_nav">
        <ul class="collapse_ul">
          <li>Home</li>
          <li>How it works</li>
          <li class="faq">FAQ</li>
          <li>Contact</li>
          <li class="text-success">Login</li>
          <li><button class="btn" id="get_started">Get Started</button></li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
import { BookOpenBlankVariant } from "mdue";

export default {
  name: "HelloWorld",
  components: { BookOpenBlankVariant },
  props: {
    msg: String,
  },
  data() {
    return {
      isVisible: false,
    };
  },
  methods: {
    showNav() {
      this.isVisible = true;
    },
    closeNav() {
      this.isVisible = false;
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
.nav {
  background: #1a1357;
  color: white;
  z-index: 100;
  width: 100%;
  display: flex;
  justify-content: space-around;
  padding: 10px 0 0;
}

.collapse_nav {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.collapse_nav > div {
  width: 30px;
  height: 5px;
  margin: 1px 0;
  background: white;
}

.logo {
  display: flex;
  align-items: center;
}

.logo > p {
  font-size: 1.5rem;
  margin: 0;
}

.closeDiv {
  position: fixed;
  top: 0;
  bottom: 0;
  height: 100%;
  left: 0;
  right: 0;
  background-color: rgba(0, 0, 0, 0.5);
}

.show_nav {
  position: absolute;
  top: 0;
  min-height: 300px;
  right: -300px;
  background: #fff;
  text-align: left;
  color: black;
  overflow-x: auto;
  padding: 40px 10px 0;
  width: 50%;
  animation: navShow forwards 0.4s ease-in-out;
  z-index: 100;
}

.nav_logo {
  color: var(--btn_color--);
  margin-right: 2px;
  font-size: 1.5rem;
}

.nav_list_container {
  display: none;
}

.faq {
  display: none;
}

.nav-ul {
  display: flex;
  align-items: center;
  padding: 5px;
}

#get_started {
  background: #50b946;
  color: white;
  padding: 10px;
  border: none;
  border-radius: 5px;
}

@keyframes navShow {
  from {
    right: -300px;
  }
  to {
    right: 0;
  }
}

.collapse_ul > li {
  padding: 10px 0;
}

.nav-ul > li,
.collapse_ul > li {
  margin-right: 10px;
  list-style: none;
  cursor: pointer;
}

@media (min-width: 768px) {
  .collapse_nav {
    display: none;
  }
  .nav {
    padding: 10px 0;
  }

  .faq {
    display: block;
  }

  .nav_list_container {
    display: block;
    margin: 0;
  }

  .nav-ul {
    padding: 0;
  }

  .nav-ul > li {
    margin-right: 20px;
    list-style: none;
    cursor: pointer;
  }
}
</style>
