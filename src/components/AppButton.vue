<template>
  <button class="cont-btn">
    <slot/>
  </button>
</template>

<style>
  .cont-btn{
    font-weight: 400;
    font-size: 18px;
    line-height: 140%;
    color: #FFFFFF;
    background: #EB276D;
    border-radius: 10px;
    outline: none;
    border: none;
    padding: 15px 25px;
    cursor: pointer;
    width: fit-content;
  }
</style>
