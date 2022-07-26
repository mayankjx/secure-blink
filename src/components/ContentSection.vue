<template>
  <div class="content">
    <div class="sectionTitle">
      <slot name="title"></slot>
    </div>
    <div class="subHeading">
      <slot name="subHeading"></slot>
    </div>
    <slot name="container"></slot>
  </div>
</template>

<script></script>

<style>
.sectionTitle {
  text-align: center;
  font-size: 25px;
  font: normal normal normal 25px Noto Sans;
  letter-spacing: 0px;
  color: #01cb63;
  opacity: 1;
  font-style: italic;
}

.subHeading {
  text-align: center;
  font: normal normal bold 40px Noto Sans;
  letter-spacing: 0px;
  color: #1f2532;
  text-transform: capitalize;
  opacity: 1;
}
</style>
