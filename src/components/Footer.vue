<template>
  <footer>
    <div class="footer-content">
      <ApplyNow />
      <section class="social-icon__wrapper">
        <ul>
          <a href="https://github.com/renuo/" target="_blank">
            <i class="fab fa-github"></i>
          </a>
          <a href="https://www.linkedin.com/company/3198067/" target="_blank">
            <i class="fab fa-brands fa-linkedin"></i>
          </a>
          <a href="https://www.facebook.com/RenuoAG/" target="_blank">
            <i class="fab fa-brands fa-facebook"></i>
          </a>
          <a href="https://twitter.com/renuo" target="_blank">
            <i class="fab fa-brands fa-twitter"></i>
          </a>
          <a href="https://www.instagram.com/renuo_ag/" target="_blank">
            <i class="fab fa-brands fa-instagram"></i>
          </a>
        </ul>
      </section>
      <!--
      <span id="footer_compiled_text"
        >hello@renuo.ch +41 44 500 83 50 Industriestrasse 44 8304
        Wallisellen</span
      >
      -->
      <div class="container-fluid footer-made-by">
        <div class="row">
          <div class="col-12 col-md-6">
            © 2022 Renuo AG — hello@renuo.ch
            <a href="https://renuo.ch/en/impressum">Privacy Policy</a>
          </div>
          <div class="col-12 col-md-6">
            <a
              class="a--no-underline"
              href="https://google.com/partners/agency?id=2492208531"
              target="_blank"
              ><img
                alt="Google Partner Badge"
                class="img-fluid"
                src="https://renuo.ch/images/renuo_partner_google-c129a8534df224352dce0c7f3e1835d1.jpg?vsn=d"
                style=""/></a
            ><a
              class="a--no-underline"
              href="https://www.swissmadesoftware.org/"
              target="_blank"
              ><img
                alt="Logo swiss made software"
                class="img-fluid"
                src="https://renuo.ch/images/renuo_partner_sms-3079a8bfb7886ddf7d71b178fce1f950.jpg?vsn=d"
                style=""
            /></a>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>
<script>
import ApplyNow from "./ApplyNow.vue";

export default {
  name: "Footer",
  data() {
    return {
      icons: []
    };
  },
  components: {
    ApplyNow
  }
};
</script>

<style scoped lang="scss">
footer {
  bottom: 0;
  width: 100%;
  height: 2.5rem;
  .footer-content {
    background-color: #27d79d;

    /*variables*/
    $white: #fff;
    $github-color: #585858;

    /*reset*/
    *,
    *::before,
    *::after {
      padding: 0;
      margin: 0;
      box-sizing: border-box;
    }
    a {
      text-decoration: none;
      cursor: pointer;
    }
    .social-icon__wrapper {
      ul {
        display: flex;
        flex-direction: row;
        flex-wrap: wrap;
        justify-content: center;
        margin-top: 30px;
      }
      li {
        padding: 1.5rem;
        list-style: none;
        .fab {
          display: flex;
          justify-content: center;
          align-items: center;
          width: 5vw;
          height: 5vw;
          font-size: 3vw;
          -webkit-transform: rotate(45deg);
          transform: rotate(45deg);
          -webkit-box-sizing: content-box;
          box-sizing: content-box;
          border-radius: 100px;
          overflow: hidden;
          transition: all 0.5s;
          &::before {
            -webkit-transform: rotate(-45deg);
            transform: rotate(-45deg);
          }
        }
        .fas {
          display: flex;
          justify-content: center;
          align-items: center;
          width: 5vw;
          height: 5vw;
          font-size: 3vw;
          -webkit-transform: rotate(45deg);
          transform: rotate(45deg);
          -webkit-box-sizing: content-box;
          box-sizing: content-box;
          border-radius: 100px;
          overflow: hidden;
          transition: all 0.5s;
          &::before {
            -webkit-transform: rotate(-45deg);
          }
        }
        .fa-github {
          color: $github-color;
          background: $white;
        }
        &:hover .fa-github {
          color: $white;
          background: $github-color;
        }
      }
    }
  }
}

.base_footer {
  padding: 0;
  margin: 0;
  background-color: white;
  width: 100% !important;
  max-width: 100% !important;
  text-align: left;
  img {
    max-width: 100%;
    max-height: 1.5rem;
    padding-left: 10px !important;
    margin: auto;
    float: none;
  }
}

#footer_compiled_text {
  font-size: 1vw;
  margin-bottom: 3% !important;
  color: white;
}

.container-fluid,
.container-sm,
.container-md,
.container-lg,
.container-xl {
  width: 100%;
  padding-right: 15px;
  padding-left: 15px;
  margin-right: auto;
  margin-left: auto;
  background-color: white;
}

.col-12 .col-md-6 {
  text-align: left !important;
}

.footer-made-by {
  text-align: left;
  padding: 0.8rem 2rem;
  font-size: 0.8rem;
  line-height: 1.7rem;
}

i {
  color: white;
  transition: all 0.2s ease-in-out;
  aspect-ratio: inherit;
}

i:hover {
  color: #dedede;
}
@media (max-width: 991.98px) {
  .footer-made-by {
    text-align: center;
    font-size: 0.7rem;
  }
}

.footer-made-by img {
  float: right;
  max-height: 1.7rem;
  margin-right: 2rem;
}

@media (min-width: 992px) {
  .fab {
    width: 50px;
    aspect-ratio: 1;
  }

  i {
    width: 100%;
    font-size: 100%;
    font-size: 50px !important;
  }

  ul > * {
    margin: 0px 7.5px !important;
  }

  ul {
    margin-bottom: 20px !important;
  }
}

@media (max-width: 991.98px) {
  i {
    font-size: 40px !important;
    margin: 0px 7.5px !important;
  }
  .footer-made-by img {
    max-height: 1.5rem;
    margin: auto;
    float: none;
    padding: 0 10px;
  }

  ul {
    margin-bottom: 20px !important;
  }
}

@media (max-width: 500px) {
  ul {
    margin-top: 60px !important;
  }
  #footer_compiled_text {
    font-size: 2.5vw;
    margin-bottom: 3% !important;
    color: white;
  }
  .fab {
    width: 10vw !important;
    height: 10vw !important;
    font-size: 7vw !important;
  }

  .fas {
    width: 10vw !important;
    height: 10vw !important;
    font-size: 7vw !important;
  }
}
</style>
