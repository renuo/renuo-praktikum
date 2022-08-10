<template>
  <div class="container-fluid footer-made-by">
    <div class="row">
      <div class="col-12 col-md-6">
        © 2022 Renuo AG — hello@renuo.ch
      </div>
      <div class="col-12 col-md-6">
        <a
          class="a--no-underline"
          href="https://google.com/partners/agency?id=2492208531"
          target="_blank"
          ><img
            alt="Google Partner Badge"
            class="img-fluid"
            src="../../public/img/footer/google_partner.jpg"
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
</template>

<script>
export default {
  name: "FooterMadeBy"
};
</script>

<style scoped lang="scss">
@media (max-width: 991.98px) {
  .footer-made-by {
    text-align: center;
    font-size: 0.7rem;
  }
  .footer-made-by img {
    max-height: 1.5rem;
    margin: auto;
    float: none;
    padding: 0 10px;
  }
}

.footer-made-by {
  text-align: left;
  padding: 0.8rem 2rem;
  font-size: 0.8rem;
  line-height: 1.7rem;
  background-color: white;
}

.footer-made-by img {
  float: right;
  max-height: 1.7rem;
  margin-right: 2rem;
}

div.footer-made-by {
  margin-top: 0px;
}
</style>
