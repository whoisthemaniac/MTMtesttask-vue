<template>
    <nav>
        <img class="m-navmenu" :src="require('../assets/img/tmp-navmenu.png')" alt="no function">
        <div class="m-navpersona">
            <div class="m-txt">Persona</div>
            <input type='text' id='mpname' name='mpname' value='Tess' readonly='readonly' size="5"/>
            <div class="m-edit"><i class="far fa-edit"></i></div>
        </div>
    </nav>
</template>

<script>
    export default {
        name: 'NavBox',
        components: {
        },
        props: {
        }

    }
</script>

<style>
    nav {
        height: 6.4rem;
        background: linear-gradient(180deg, #FFFFFF 0%, #F0F0F0 100%);
        position: fixed;
        top: 3.6rem;
        width: 100%;
    }
    nav .m-navmenu {
        position: absolute;
        right: 0;
        top: .3em;
    }
    .m-navpersona {
        display: flex;
        align-items: center;
        height: 6.4em;
        background-image: url("../../img/tmp-navpersona-icon.png");
        background-repeat: no-repeat;
    }
    .m-navpersona .m-txt, .m-navpersona input {
        font-size: 2em;
        color: #6c7575;
    }
    .m-navpersona .m-txt {
        margin-left: 2.8em;
    }
    .m-navpersona .m-edit {
        font-size: 1.4em;
        margin: 0;
        color: #6c7575;
    }
    .m-navpersona input {
        color: #3C4646;
        font-weight: bold;
        width: auto !important;
        margin: 0 !important;
        background-color: transparent;
        border-color: transparent;
        box-shadow: none;
    }
</style>