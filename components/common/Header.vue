<template>
  <div class="header" aria-label="グローバルヘッダー">
    <div class="header__inner">
      <div class="header__twitterButton">
        <a href="http://twitter.com/share?url=https://exh-room.com/&text=3D%E7%A9%BA%E9%96%93%E3%80%81AR%E6%8A%80%E8%A1%93%E3%82%92%E5%8F%96%E3%82%8A%E5%85%A5%E3%82%8C%E3%81%9FRooo%20Lou%20Exhibiton%E3%80%8CRoom%E3%80%8D" target="_blank">
          <img src="~assets/img/btn_tw@2x.png">
        </a>
      </div>
      <div class="header__logo">
        <a href="/">
          <HeaderLogo></HeaderLogo>
        </a>
      </div>
      <div class="header__eclink">
        <a href="https://rooostore.thebase.in/" target="_blank">
          <p class="header__eclink--text">GOODS</p>
        </a>
      </div>
    </div>
  </div>
</template>

<script>
  import HeaderLogo from '@/assets/svg/logo_02.svg';
	export default {
		name: "Header",
    components: {
      HeaderLogo
    },
    data () {
      return {

      }
    },
	}
</script>

<style lang="scss" scoped>
  .header {
    width: 100%;
    height: auto;
    position: fixed;
    top: get-vw(50px);
    left: 0;
    z-index: 10;
  }
  .header__inner {
    width: get-vw(668px);
    height: get-vw(37px);
    margin: 0 auto;
    display: flex;
    align-items: center;
    position: relative;
  }
  .header__twitterButton {
    width: get-vw(38px);
    height: get-vw(31.5px);
    a {
      display: block;
      width: 100%;
      height: 100%;
      img {
        width: 100%;
        height: auto;
      }
    }
  }
  .header__logo {
    width: get-vw(142px);
    height: auto;
    margin: 0 auto;
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    svg {
      width: 100%;
      height: auto;
    }
  }
  .header__eclink {
    margin-left: auto;
    a {
      display: block;
      width: 100%;
      height: auto;
      text-decoration: none;
      .header__eclink--text {
        @include poppinsMedium();
        font-size: get-vw(24px);
        color: #000;
      }
    }
  }
</style>
