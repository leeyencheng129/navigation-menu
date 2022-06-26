<template>
  <header :class="{'scrolled-nav':scrolledNav}">
    <nav>
      <div class="branding">
         <router-link :to="{name:'Home'}"><img src="@/assets/logo.svg" alt=""></router-link>
       
      </div>
      <ul v-show="!mobile" class="navigation">
        <li>
          <router-link class="link" :to="{name:'Brand'}">品牌介紹</router-link>
        </li>
        <li>
          <router-link class="link" :to="{name:'About'}">關於護膚</router-link>
        </li>
      
        <li>
          <router-link class="link" :to="{name:'Contact'}">聯絡我們</router-link>
        </li>
      </ul>
      <div class="icon">
        <i class="far fa-bars" v-show="mobile" @click="toggleMobileNav" :class="{'icon-active':mobileNav}"></i>
      </div>
      <transition name="mobile-nav">
        <ul v-show="mobileNav" class="dropdown-nav">
          <li>
            <router-link class="link" :to="{name:'Home'}">品牌介紹</router-link>
          </li>
          <li>
            <router-link class="link" :to="{name:'About'}">關於護膚</router-link>
          </li>
      
          <li>
            <router-link class="link" :to="{name:'Contact'}">聯絡我們</router-link>
          </li>
        </ul>
      </transition>
    </nav>
  </header>
</template>

<script>

export default {
  name: 'navigation',
  data() {
    return {
      scrolledNav: null,
      mobile: null,
      mobileNav: null,
      windowWidth: null
    }
  },
  created() {
    window.addEventListener('resize', this.checkScreen)
    this.checkScreen()
  },
  mounted(){
    window.addEventListener('scroll',this.updateScroll)
  },
  methods: {
    toggleMobileNav() {
      this.mobileNav = !this.mobileNav
    },

    updateScroll(){
      const scrollPosition = window.scrollY
      if(scrollPosition > 50){
        this.scrolledNav = true
        return
      }
      this.scrolledNav = false
    },

    checkScreen() {
      this.windowWidth = window.innerWidth
      if (this.windowWidth <= 750) {
        this.mobile = true
        return
      }
      this.mobile = false
      this.mobileNav = false
      return
    }
  }
}
</script>

<style lang="scss" scoped>
header {
  background-color: #fff;
  z-index: 99;
  width: 100%;
  position: fixed;
  transition: 0.5s ease all;
  color: #333;
  border-bottom: 1px solid #e43f94;
  nav {
  position: relative;
  display: flex;
  flex-direction: row;
  padding: 12px 0;
  transition: 0.5s ease all;
  width: 90%;
  margin: 0 auto;
  @media (min-width: 1140px) {
    max-width: 1140px;
  }

  ul,
  .link {
    font-weight: 500;
    color: #333;
    list-style: none;
    text-decoration: none;
  }
  li {
    text-transform: uppercase;
    padding: 16px;
    margin-left: 16px;

  }

  .link {
    font-size: 18px;
    transition: 0.5s ease all;
    padding-bottom: 4px;
    border-bottom: 1px solid transparent;

    &:hover {
      color:#333;
      border-color: #e43f94;
    }
  }

  .branding {
    display: flex;
    align-items: center;

    img {
      width: 140px;
      transition: 0.5s ease all;
      @media (max-width:600px){
         width: 80px;
      }
    }
  }
  .navigation {
    display: flex;
    align-items: center;
    flex: 1;
    justify-content: flex-end;
  }

  .icon {
    display: flex;
    align-items: center;
    position: absolute;
    top: 0;
    right: 24px;
    height: 100%;

    i {
      cursor: pointer;
      font-size: 24px;
      transition: 0.8s ease all;
    }
  }

  .icon-active {
    transform: rotate(180deg);
  }
  .dropdown-nav {
    display: flex;
    flex-direction: column;
    position: fixed;
    width: 100%;
    max-width: 250px;
    height: 100%;
    background: #fff;
    top: 0;
    left: 0;
    box-shadow: 0 0 20px 0 #ddd;
    li {
      margin-left: 0;
      .link {
        color: #000;
      }
    }
  }

  .mobile-nav-enter-active,.mobile-nav-leave-active{
    transition: 1s ease all;
  }
  .mobile-nav-enter-from,.mobile-nav-leave-to{
    transform: translateX(-250px);
  }
  .mobile-nav-enter-to{
    transform: translate(0);
  }
}
}

.scrolled-nav{
  background: rgba(255, 255, 255, 0.86);
  box-shadow: 0 4px 6px -1px rgba(0,0,0,0.1) , 0 2px 4px -1pxrgba(0,0,0,0.06);
  nav{
    padding: 8px 0;

    .branding{
      img{
        width: 100px;
        box-shadow:  0 4px 6px -1px rgba(0,0,0,0.1) , 0 2px 4px -1pxrgba(0,0,0,0.06);
         @media (max-width:600px){
         width: 70px;
      }
      }
    }
  }
}
</style>
