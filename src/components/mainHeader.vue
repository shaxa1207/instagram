<template>
    <div class="container">
        <header class="header">
        <div class="logo">
            <img src="../assets/images/logo.svg" alt="">
        </div>
        <div class="input">
            <input type="text">
            <span class="_6RZXI coreSpriteSearchIcon"></span>
        </div>
        <div></div>
    </header>
    </div>
</template>

<script>
export default {
    name: "mainHeader",
}
</script>

<style lang="scss" scoped>
    .input{
        input{
            font-size: 16px;
            background: rgba(var(--b3f,250,250,250),1);
        }
    }
</style>