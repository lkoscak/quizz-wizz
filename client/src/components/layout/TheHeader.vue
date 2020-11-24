<template>
    <div class="header-container">
        <h1 class="header-title">QuiZZ-WiZZ</h1>
        <ul class="header-nav-links">
            <li class="header-nav-link"><a href="#">About this app</a></li>
        </ul>
    </div>
</template>

<style lang="scss" scoped>
    .header-container{
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: 6rem;
        width: 100%;
        background-color: $primary-back-color;
        color: $primary-text-color;
        padding: 0 1rem;

        .header-nav-links{
        list-style-type: none;
        font-size: 1rem;
        }

        .header-nav-link{
            display: inline-block;
        }

        a{
            text-decoration: none;
            color: $primary-text-color;
        }
    }
</style>