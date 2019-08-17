<template>
    <main>




        <div class="row m-main-toprow">
            <div class="columns small-2 shrink">
                <img class="m-main-toprow-profilepic" src="https://dummyimage.com/67x67" alt="">
            </div>
            <div class="columns auto">
                <div class="m-editbox" id="">
                    <div class="m-editbox-title">
                        PERSONA NAME
                    </div>
                    <div class="m-editbox-content">
                        Tess
                    </div>
                </div>
            </div>
            <div class="columns small-3">
                <div class="m-editbox" id="">
                    <div class="m-editbox-title">
                        SHORT NAME
                    </div>
                    <div class="m-editbox-content">
                        TES
                    </div>
                </div>
            </div>
        </div>

        <div class="row m-main-mainrow">
            <div class="columns small-4">
                <div class="m-editbox" id="">
                    <div class="m-editbox-title">
                        IMAGE
                    </div>
                    <div class="m-editbox-content">
                        <img class="m-main-toprow-profilepic" src="https://dummyimage.com/400x400/cccccc/999999.png&text=" alt="">
                    </div>
                    <div class="m-editbox-option m-option-trash">
                        <i class="fas fa-cog"></i>
                    </div>
                </div>

                <div class="m-editbox" id="">
                    <div class="m-editbox-title">
                        MOOD IMAGES
                    </div>
                    <div class="m-editbox-content">
                        <img class="m-main-toprow-profilepic" src="https://dummyimage.com/400x100/cccccc/999999.png&text=" alt="">
                        <img class="m-main-toprow-profilepic" src="https://dummyimage.com/400x400/cccccc/999999.png&text=" alt="">
                        <img class="m-main-toprow-profilepic" src="https://dummyimage.com/400x400/cccccc/999999.png&text=" alt="">
                    </div>
                    <div class="m-editbox-option">
                        <i class="fas fa-cog"></i>
                    </div>
                </div>

            </div>
            <div class="columns small-8">

                <div id="dropzone">

                    <div class="m-editbox" id="">
                        <div class="m-editbox-title">
                            OCCUPATION
                        </div>
                        <div class="m-editbox-content">
                            Researcher
                        </div>
                        <div class="m-editbox-option">
                            <i class="fas fa-cog"></i>
                        </div>
                    </div>

                    <div class="m-editbox" id="">
                        <div class="m-editbox-title">
                            NATIONALITY
                        </div>
                        <div class="m-editbox-content">
                            French
                        </div>
                        <div class="m-editbox-option">
                            <i class="fas fa-cog"></i>
                        </div>
                    </div>

                    <div class="m-editbox" id="">
                        <div class="m-editbox-title">
                            MARITAL STATUS
                        </div>
                        <div class="m-editbox-content">
                            Married, 3 kids
                        </div>
                        <div class="m-editbox-option">
                            <i class="fas fa-cog"></i>
                        </div>
                    </div>

                    <div class="m-editbox" id="">
                        <div class="m-editbox-title">
                            QUOTE
                        </div>
                        <div class="m-editbox-content">
                            <p>"Life may not be the party we hoped for, but while we're here, we should dance."</p>
                        </div>
                        <div class="m-editbox-option">
                            <i class="fas fa-cog"></i>
                        </div>
                    </div>

                    <div class="m-editbox" id="">
                        <div class="m-editbox-title">
                            DESCRIPTION
                        </div>
                        <div class="m-editbox-content">
                            <p>Tess is that friendly neighbour next door. She has a secure job at the national railway company. Together with her husband, she has a monthly household income of 5000 Euro net.</p>
                            <p>Tess loves to spend free time with her three kids. Marcus, her husband, loves being outdoors, so whenever possible the couple takes long hiking tours with their children.</p>
                            <p><strong>Tess is not interested in technology.<br>She wants things that just work.</strong></p>
                        </div>
                        <div class="m-editbox-option">
                            <i class="fas fa-cog"></i>
                        </div>
                    </div>


                </div>

            </div>
        </div>





    </main>
</template>





<script>
    export default {
        name: 'MainBox'
    }

</script>

<style>
    main {
        background-color: #F0F0F0;
        color: #3C4646;
        margin: 14.4em 49.9em 10em 11.7em;
        -webkit-box-shadow: 0 .1em 2em 0 rgba(0,0,0,0.3), 0 0 3em 0 rgba(0,0,0,0.3);
        box-shadow: 0 .1em 2em 0 rgba(0,0,0,0.3), 0 0 3em 0 rgba(0,0,0,0.3);
    }

    .m-main-toprow, .m-main-mainrow {
        padding: 1.6em .8em;
    }
    .m-main-toprow {
        background-color: #DCDCDC;
    }
    .m-main-toprow .m-editbox {
        min-height: 100%;
    }
    .m-main-toprow .m-main-toprow-profilepic {
        object-fit: contain;
    }

    /* *** DROP ZONE *** */

    .m-editbox.nodrag .m-editbox-title, .m-editbox.nodrag .m-editbox-content {
        cursor: no-drop !important;
    }

    main .m-editbox {
        background: #fff;
        padding: .8em 1.2em 1.2em;
        border-radius: .2em;
        margin-bottom: 1.6em;
        position: relative;
    }
    main .m-main-mainrow .m-editbox:last-child {
        margin-bottom: 0;
    }
    main .m-editbox-title {
        font-size: 1.2em;
        color: #B1B6B6;
        font-weight: bold;
        margin-bottom: .5em;
        cursor: grab;
    }
    main .m-editbox-content {
        font-size: 1.6em;
        color: #3C4646;
    }
    main .m-editbox-option {
        position: absolute;
        top: .7em;
        right: 1em;
        font-size: 1.2em;
        color: #B1B6B6;
        display: block;
        cursor: pointer;
    }
    main .m-editbox p:not(:last-child) {
        margin-bottom: .7em;
    }
    main .m-editbox img {
        object-fit: contain;
        padding-top: .8em;
    }
    /* special for dragging */
    .m-editbox-ghost {
        border: 1px solid #9CDBFB;
        background-color: #F0F8FC !important;
        -webkit-box-shadow: none;
        box-shadow: none;
    }
    .m-editbox-ghost .m-editbox-title {
        align-self: center;
        justify-self: center;
    }
    .m-editbox-ghost .m-editbox-title span {
        display: none;
    }
    .m-editbox-ghost .m-editbox-title:before {
        content: 'insert element here';
        font-style: italic;
        color: #646E6E;
    }
    .m-editbox-ghost .m-editbox-content {
        opacity: 0;
    }

</style>