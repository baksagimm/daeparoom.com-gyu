<template lang="pug">
div#main
    .left
        .archive 
            div
                img(src="@/assets/image/folder_open.svg")
                h2 Cultivation
            a(href="/login")
                img.goto(src="@/assets/image/arrow_right.svg")

        .visitor
            div
                img(src="@/assets/image/pencil.svg")
                h2 Community
            a(href="/community")
                img.goto(src="@/assets/image/arrow_right.svg")

    .right
        img(src="@/assets/image/daepa_logo.svg")
        h3 Archive and Research-based<br>Art Movement
    
    p Built with skapi
</template>

<script setup>

</script>

<style scoped lang="less">
#main {
    width: 100vw;
    height: 100vh;
    display: flex;
    flex-wrap: nowrap;
    align-items: center;
    position: relative;

    p {
        position: absolute;
        right: 6vw;
        bottom: 3vw;
        font-size: 20px;
        font-weight: 500;
    }
}

.left {
    width: 50%;
    height: 100%;
    border-right: 1px solid #000;
    box-sizing: border-box;

    & > div {
        position: relative;
        width: 100%;
        height: 50%;
        padding: 40px;
        box-sizing: border-box;
        transition: all 0.3s;

        &:first-child {
            border-bottom: 1px solid #000;
        }

        &:hover {
            background-color: rgba(255,255,255,0.5);
        }

        & > div {
            line-height: 0.1;
        }

        img {
            width: 100px;
            height: 100px;

            &.goto {
                position: absolute;
                right: 40px;
                bottom: 40px;
                width: 120px;
                height: 120px;
            }
        }

        h2 {
            font-size: 7vw;
            font-size: clamp(16px, 7vw, 110px);
            font-weight: 700;
        }
    }
}

.right {
    width: 50%;
    // padding: 0 90px;
    padding: 0 6vw;
    display: flex;
    flex-wrap: wrap;
    box-sizing: border-box;

    img {
        width: 100%;
    }

    h3 {
        font-size: 2.1vw;
        font-weight: 700;
    }
}

@media (max-width: 780px) {
    #main {
        flex-wrap: wrap;
        align-items: flex-start;
        flex-direction: column;

        p {
            font-size: 14px;
            font-weight: 300;
            bottom: 0;
        }
    }
    .left {
        width: 100%;
        height: 360px;

        & > div {
            height: 180px;
            text-align: bottom;
            padding: 20px;

            &:last-child {
                border-bottom: 1px solid #000;
            }

            img {
                width: 60px;
                height: 60px;
            
                &.goto {
                    right: 100px;
                    bottom: 20px;
                    width: 60px;
                    height: 60px;
                }
            }

            & > div {
                position: absolute;
                left: 20px;
                bottom: 20px;
            }

            h2 {
                font-size: 36px;
            }
        }
    }
    .right {
        width: 100%;
        height: 180px;
        padding-top: 45px;

        h3 {
            font-size: 16px;
        }
    }
}
</style>