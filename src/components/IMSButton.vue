<template>
  <div>
    <CenterTitle title="Komm zu uns ins Team" />
    <a href="https://www.renuo.ch/en/jobs/ims-internship-2023-2024">
      <p class="main-text">
        IMS Internship
        <CurrentYearComponent
          :augustchange="true"
          :increment="1"
        />/<CurrentYearComponent :augustchange="true" :increment="2" />
      </p>
      <p class="sub-text">100 %</p>
    </a>
  </div>
</template>

<script>
import CenterTitle from "@/components/CenterTitle";
import CurrentYearComponent from "@/components/CurrentYearComponent";

export default {
  name: "IMSButton",
  components: { CurrentYearComponent, CenterTitle }
};
</script>

<style scoped lang="scss">
@use "@/stylesheets/variables.scss";

@media screen and (max-width: 510px) {
  a {
    margin: 0px 10px !important;
  }
}

a {
  background-color: variables.$renuo-base-color;
  background-image: url("https://www.renuo.ch/images/header-gray-c059a3ec41d8322d3e3fa1656b578ccb.svg?vsn=d");
  padding: 10px 125px 25px 10px;
  border-radius: 0;
  border: none;
  display: block;
  width: fit-content;
  margin: 20px auto;
  .main-text {
    font-size: 1.75rem;
    color: white;
    font-weight: bold;
    margin-bottom: 0;
    transition: all ease-in-out 200ms;
  }
  .sub-text {
    letter-spacing: 0.7px;
    color: #3a4440;
    line-height: 2.2rem;
    font-size: 1.12rem;
  }
  &:hover {
    .main-text {
      color: #151513;
    }
  }
}
</style>
