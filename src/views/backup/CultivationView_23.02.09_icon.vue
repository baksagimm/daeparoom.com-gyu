<template lang="pug">
.header
    .title 
        //- img.icon(src="@/assets/image/folder_open.svg")
        .icon
            svg(version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px" viewBox="0 0 24 24" enable-background="new 0 0 24 24" xml:space="preserve")
                g
                    g
                        path(d="M3.78,19.61c-0.47,0-0.88-0.18-1.24-0.54C2.18,18.71,2,18.29,2,17.83V6.19c0-0.48,0.18-0.9,0.54-1.26s0.77-0.54,1.24-0.54h6.09l1.49,1.49h7.53c0.48,0,0.9,0.18,1.26,0.54c0.36,0.36,0.54,0.78,0.54,1.26H3.78v10.19l2.3-8.84H22l-2.34,8.97c-0.17,0.57-0.43,0.98-0.79,1.23c-0.36,0.25-0.84,0.37-1.44,0.37H3.78z")
        h2 Cultivation
    .ec
        .ecBtn Edit Color
        .ecColor
            ul
                li Color1
                    input.bgColor.bgColor1(type="color")
                li Color2
                    input.bgColor.bgColor2(type="color")
                li Text
                    input.bgColor.bgColor3(type="color")
                input.sInput(type='submit' value='Save')
    .info User Name
    .mi
        .miBtn U
        .miMenu
            ul
                li
                    a(href="/accountsetting") Account Setting
                li
                    a(href="/logout") Log Out
                li
                    a(href="/meditcolor") Edit Color
.tableWrap
    table#resizeMe.table
        thead
            tr
                th.th Host
                th.th Title
                th.th Type
                th Date
        tbody
            tr.tit(@click='()=>changeActive(0)')
                td NIKE
                td “{{ titleArray[0] }}”
                td(style="font-size:16px;") 
                    | Illustration,
                    br
                    | Interactive Art
                td 2022.04
            tr.con(:class="{ 'active': showArray[0] }")
                td(colspan="4" style='overflow: hidden;')
                    .slider__wrap
                        .slider__img
                            .slider__inner
                                .slider.image-column
                                    img.icon(src="@/assets/image/image1111.svg")
                                .slider.text-column
                                    | Are you looking for a Nike logo font that will make your design stand out? If so, then you have come to the right place. Among the most popular typefaces available for Photoshop is the Nike font pack. You can also use the font pack to generate text in other applications. It is a typeface that is suitable for use on websites and in games due to its high accessibility and 22 styles. This typeface will be of great use in the development of websites and games due to the strength of its accessibility. The Nike font can be found here.
                                    | Designers have to figure out a way to encourage people to fill them out. Yet, if you add one form field too many, you can expect your conversion rate to plummet. How do some signup forms strike this balance? We’ll take a look at 20 inspiring signup forms and find out what makes them work.
                                    | Are you looking for a Nike logo font that will make your design stand out? If so, then you have come to the right place. Among the most popular typefaces available for Photoshop is the Nike font pack. You can also use the font pack to generate text in other applications. It is a typeface that is suitable for use on websites and in games due to its high accessibility and 22 styles. This typeface will be of great use in the development of websites and games due to the strength of its accessibility. The Nike font can be found here.
                                    | Designers have to figure out a way to encourage people to fill them out. Yet, if you add one form field too many, you can expect your conversion rate to plummet. How do some signup forms strike this balance? We’ll take a look at 20 inspiring signup forms and find out what makes them work.
                                .slider.image-column
                                    img.icon(src="@/assets/image/image1111.svg")
                        .slider__btn
                            img.icon.prev(src="@/assets/image/arrow_left.svg" alt="이전")
                            img.icon.next(src="@/assets/image/arrow_right.svg" alt="다음")
                img.icon.close(src="@/assets/image/up.svg")
                img.icon.mclose(src="@/assets/image/up1.svg")
            tr.tit(@click='()=>changeActive(1)')
                td NIKE
                td “{{ titleArray[1] }}”
                td(style="font-size:16px;") 
                    | Illustration,
                    br
                    | Interactive Art
                td 2022.04
            tr.con(:class="{ 'active': showArray[1] }")
                td(colspan="4" style='overflow: hidden;')
                    .slider__wrap
                        .slider__img
                            .slider__inner
                                .slider.image-column
                                    img.icon(src="@/assets/image/image1111.svg")
                                .slider.text-column
                                    | Are you looking for a Nike logo font that will make your design stand out? If so, then you have come to the right place. Among the most popular typefaces available for Photoshop is the Nike font pack. You can also use the font pack to generate text in other applications. It is a typeface that is suitable for use on websites and in games due to its high accessibility and 22 styles. This typeface will be of great use in the development of websites and games due to the strength of its accessibility. The Nike font can be found here.
                                    | Designers have to figure out a way to encourage people to fill them out. Yet, if you add one form field too many, you can expect your conversion rate to plummet. How do some signup forms strike this balance? We’ll take a look at 20 inspiring signup forms and find out what makes them work.
                                    | Are you looking for a Nike logo font that will make your design stand out? If so, then you have come to the right place. Among the most popular typefaces available for Photoshop is the Nike font pack. You can also use the font pack to generate text in other applications. It is a typeface that is suitable for use on websites and in games due to its high accessibility and 22 styles. This typeface will be of great use in the development of websites and games due to the strength of its accessibility. The Nike font can be found here.
                                    | Designers have to figure out a way to encourage people to fill them out. Yet, if you add one form field too many, you can expect your conversion rate to plummet. How do some signup forms strike this balance? We’ll take a look at 20 inspiring signup forms and find out what makes them work.
                                .slider.image-column
                                    img.icon(src="@/assets/image/image1111.svg")
                        .slider__btn
                            img.icon.prev(src="@/assets/image/arrow_left.svg" alt="이전")
                            img.icon.next(src="@/assets/image/arrow_right.svg" alt="다음")
                img.icon.close(src="@/assets/image/up.svg")
                img.icon.mclose(src="@/assets/image/up1.svg")
            tr.tit(@click='()=>changeActive(2)')
                td NIKE
                td “{{ titleArray[2] }}”
                td(style="font-size:16px;") 
                    | Illustration,
                    br
                    | Interactive Art
                td 2022.04
            tr.con(:class="{ 'active': showArray[2] }")
                td(colspan="4" style='overflow: hidden;')
                    .slider__wrap
                        .slider__img
                            .slider__inner
                                .slider.image-column
                                    img.icon(src="@/assets/image/image1111.svg")
                                .slider.text-column
                                    | Are you looking for a Nike logo font that will make your design stand out? If so, then you have come to the right place. Among the most popular typefaces available for Photoshop is the Nike font pack. You can also use the font pack to generate text in other applications. It is a typeface that is suitable for use on websites and in games due to its high accessibility and 22 styles. This typeface will be of great use in the development of websites and games due to the strength of its accessibility. The Nike font can be found here.
                                    | Designers have to figure out a way to encourage people to fill them out. Yet, if you add one form field too many, you can expect your conversion rate to plummet. How do some signup forms strike this balance? We’ll take a look at 20 inspiring signup forms and find out what makes them work.
                                    | Are you looking for a Nike logo font that will make your design stand out? If so, then you have come to the right place. Among the most popular typefaces available for Photoshop is the Nike font pack. You can also use the font pack to generate text in other applications. It is a typeface that is suitable for use on websites and in games due to its high accessibility and 22 styles. This typeface will be of great use in the development of websites and games due to the strength of its accessibility. The Nike font can be found here.
                                    | Designers have to figure out a way to encourage people to fill them out. Yet, if you add one form field too many, you can expect your conversion rate to plummet. How do some signup forms strike this balance? We’ll take a look at 20 inspiring signup forms and find out what makes them work.
                                .slider.image-column
                                    img.icon(src="@/assets/image/image1111.svg")
                        .slider__btn
                            img.icon.prev(src="@/assets/image/arrow_left.svg" alt="이전")
                            img.icon.next(src="@/assets/image/arrow_right.svg" alt="다음")
                img.icon.close(src="@/assets/image/up.svg")
                img.icon.mclose(src="@/assets/image/up1.svg")
.footer 
    img.icon(src="@/assets/image/plus2.svg")
.mfooter 
    img.icon(src="@/assets/image/plus.svg")
</template>

<script setup>
import { onMounted, ref } from 'vue';

let titleArray = [
    'Whatever Whenever',
    'blahblahblahblahblahblahsi',
    'hahahahahah'
]

let showArray = ref([
    false,
    false,
    false
])

function changeActive(idx) {
    showArray.value[idx] = !showArray.value[idx]
    // if(showArray[idx]) {
    //     showArray[idx] = false
    // }
    // else {
    //     showArray[idx] = true
    // }
}

onMounted(() => {
    ////////// column width
    const createResizableTable = function (table) {
        const cols = table.querySelectorAll('.th');
        [].forEach.call(cols, function (col) {
            const resizer = document.createElement('div');
            resizer.classList.add('resizer');

            resizer.style.position = 'absolute';
            resizer.style.top = '-8px';
            resizer.style.right = '-16px';
            resizer.style.width = `16px`;
            resizer.style.height = `8px`;
            resizer.style.backgroundColor = 'black';
            resizer.style.cursor = 'col-resize';
            resizer.style.userSelect = 'none';

            col.appendChild(resizer);

            createResizableColumn(col, resizer);
        });
    };

    const createResizableColumn = function (col, resizer) {
        let x = 0;
        let w = 0;

        const mouseDownHandler = function (e) {
            x = e.clientX;

            const styles = window.getComputedStyle(col);
            w = parseInt(styles.width, 10);

            document.addEventListener('mousemove', mouseMoveHandler);
            document.addEventListener('mouseup', mouseUpHandler);

            resizer.classList.add('resizing');
        };

        const mouseMoveHandler = function (e) {
            const dx = e.clientX - x;
            col.style.width = `${w + dx}px`;
        };

        const mouseUpHandler = function () {
            resizer.classList.remove('resizing');
            document.removeEventListener('mousemove', mouseMoveHandler);
            document.removeEventListener('mouseup', mouseUpHandler);
        };

        resizer.addEventListener('mousedown', mouseDownHandler);
    };

    createResizableTable(document.getElementById('resizeMe'));


    ////////// show content
    // let tr = document.querySelectorAll("tbody tr");

    // for(let i = 1; i<tr.length; i++) {
    //     tr[i].addEventListener('click', () => {
    //         tr[i+1].classList.toggle('active');
    //     })
    // }


    ////////// slider
    const sliderImg = document.querySelectorAll(".slider__img");       // 보여지는 영역
    const sliderInner = document.querySelectorAll(".slider__inner");   // 움직이는 영역
    const sliderBtnPrev = document.querySelectorAll(".prev");       //왼쪽버튼
    const sliderBtnNext = document.querySelectorAll(".next");       //오른쪽버튼

    for(let i=0; i<sliderImg.length; i++) {
        sliderBtnPrev[i].addEventListener("click", () => {
            sliderInner[i].style.transition = "all 400ms";
            sliderInner[i].style.transform = "translateX("+ 0 +"px)";
        });
    
        sliderBtnNext[i].addEventListener("click", () => {
            sliderInner[i].style.transition = "all 400ms";
            sliderInner[i].style.transform = "translateX("+ -(sliderInner[i].clientWidth - sliderImg[i].clientWidth) +"px)";
        });
    }



    ////////// close content(pc ver)
    let close = document.querySelectorAll('.close');

    for(let i=0; i<close.length; i++) {
        close[i].addEventListener('click', () => {
            showArray.value[i] = !showArray.value[i]
        })
    }

    ////////// close content(mobile ver)
    let mclose = document.querySelectorAll('.mclose');

    for(let i=0; i<mclose.length; i++) {
        mclose[i].addEventListener('click', () => {
            showArray.value[i] = !showArray.value[i]
        })
    }


    ////////// change backgroud-color
    let bodyId = document.getElementById('shell');
    let ecBtn = document.querySelector('.ecBtn');
    let ecColor = document.querySelector('.ecColor');
    let bgColor1 = document.querySelector('.bgColor1');
    let bgColor2 = document.querySelector('.bgColor2');
    let bgColor3 = document.querySelector('.bgColor3');
    let miBtn = document.querySelector('.miBtn');
    let miMenu = document.querySelector('.miMenu');

    // 색상 바꾸기
    function returnColor(){
        bodyId.style.background =
            "linear-gradient("
            + "180deg, "
            + bgColor1.value
            + ","
            + bgColor2.value
            + ")";
        bodyId.style.color = bgColor3.value;
    }

    bgColor1.addEventListener("input", returnColor)
    bgColor2.addEventListener("input", returnColor)
    bgColor3.addEventListener("input", returnColor)


    // click > 'block' or 'none'
    miBtn.addEventListener('click', () => {
        if(miMenu.style.display === 'none'){
            miMenu.style.display = 'block';
        } else {
            miMenu.style.display = 'none';
        }
    })

    ecBtn.addEventListener('click', () => {
        if(ecColor.style.display === 'none'){
            ecColor.style.display = 'block';
        } else {
            ecColor.style.display = 'none';
        }
    })



    // icon contrast
    let plus = document.querySelector('.footer img');
    let icon = document.querySelectorAll('.icon');

    plus.addEventListener('click', function(){
        icon.forEach((e) => {
            e.classList.toggle('contrast');
        })
    });

})





</script>

<style scoped lang="less">
.header {
    width: 100%;
    // height: 168px;
    padding: 40px 100px 100px;
    box-sizing: border-box;
    display: flex;
    flex-wrap: nowrap;
    justify-content: space-between;

    h2 {
        font-size: 24px;
        font-weight: 400;
    }

    .title {
        margin-right: 40px;
        line-height: 0.1;
        display: flex;

        img {
            width: 40px;
            height: 40px;
            margin-right: 4px;
        }

        .icon {
            width: 40px;
            height: 40px;
            margin-right: 4px;
        }
    }

    .ec {
        position: relative;

        .ecBtn {
            cursor: pointer;
            font-size: 24px;
            font-weight: 400;
            margin-top: auto;
        }
    
        .ecColor {
            position: absolute;
            content: '';
            left: 0;
            bottom: -230px;
            background-color: #fff;
            border-radius: 4px;
            box-shadow: 4px 4px 12px rgba(0, 0, 0, 0.25), inset -1px -1px 2px rgba(0, 0, 0, 0.25), inset 1px 1px 2px rgba(255, 255, 255, 0.65);
            z-index: 999;
            display: none;
    
            ul {
                width: 153px;
                box-sizing: border-box;
                list-style: none;
                margin: 0;
                padding: 20px; 
    
                li {
                    display: flex;
                    align-items: center;
                    justify-content: space-between;
                    font-size: 20px;
                    font-weight: 400;
                    line-height: 22px;
                    margin-bottom: 20px;
    
                    .bgColor {
                        width: 28px;
                        height: 28px;
                        padding: 0;
                        border: 0;
                        background-color: transparent;
    
                    }
                }
                .sInput {
                    width: 100%;
                    height: 40px;
                    font-size: 16px;
                    font-weight: 400;
                    line-height: 17px;
                    background: #FFFFFF;
                    border: 0.5px solid #595959;        
                    box-shadow: inset -1px -1px 2px rgba(0, 0, 0, 0.25), inset 1px 1px 2px rgba(255, 255, 255, 0.65);
                    border-radius: 4px;
                }
            }
        }
    }

    .info {
        font-size: 24px;
        font-weight: 400;
        margin-left: auto;
        margin-top: auto;
    }

    .mi {
        position: relative;
        display: none;

        .miBtn {
            position: relative;
            margin-top: auto;
            width: 40px;
            height: 40px;
            text-align: center;
            font-size: 24px;
            color: #fff;
            border-radius: 50%;
            background-color: #000;
        }

        .miMenu {
            position: absolute;
            content: '';
            right: 0;
            bottom: -200px;
            background-color: #fff;
            border-radius: 4px;
            box-shadow: 4px 4px 12px rgba(0, 0, 0, 0.25), inset -1px -1px 2px rgba(0, 0, 0, 0.25), inset 1px 1px 2px rgba(255, 255, 255, 0.65);
            z-index: 999;
            display: none;
    
            ul {
                width: 212px;
                box-sizing: border-box;
                list-style: none;
                margin: 0;
                padding: 20px 12px; 
    
                li {
                    padding: 10px 0 10px 10px;
                    margin-bottom: 8px;

                    &:last-child {
                        margin-bottom: 0;
                    }
                    &:hover {
                        background-color: rgba(0,0,0,0.04);
                        border-radius: 4px;
                    }

                    a {
                        text-align: center;
                        font-size: 20px;
                        font-weight: 400;
                        line-height: 22px;
                        text-decoration: none;
                        color: #000;
                    }
                }
            }
        }
    }

}

.tableWrap {
    width: 100vw;

    .table {
        width: 100%;
        border-collapse: collapse;

        thead {
            tr {
                height: 80px;
                th {
                    font-size: 24px;
                    font-weight: 400;
                    line-height: 26px;
                    text-align: left;
                    position: relative;   

                    &:first-child {
                        width: 200px;
                        padding-left: 100px;
                    }

                    &:nth-child(2) {
                        width: calc(100vw - 860px);
                        // width: 580px;
                    }

                    &:nth-child(3) {
                        width: 300px;
                    }

                    &:last-child {
                        width: 160px;
                        padding-right: 100px;
                    }

                    .resizable {
                        height: 100px;
                        width: 100px;
                        position: relative;
                    }
                }
            }
        }

        tbody {
            tr {
                height: 80px;
                transition: all 0.3s;

                &.tit {
                    // border-top: 1px solid #000;
                    position: relative;
                    cursor: pointer;

                    &::after {
                        position: absolute;
                        content: '';
                        left: 50%;
                        top: 0;
                        transform: translateX(-50%);
                        width: 999%;
                        height: 100%;
                        background-color: rgba(255,255,255,0.5);
                        opacity: 0;
                        z-index: -999;
                        transition: all 0.3s;
                    }
                    
                    // &:hover {
                    //     background-color: rgba(255,255,255,0.5);
                    // }

                    &:hover::after {
                        opacity: 1;
                    }

                    td {
                        font-size: 36px;
                        font-weight: 700;
                        line-height: 39px;
                        user-select: none;

                        &::after {
                            position: absolute;
                            content: '';
                            left: 50%;
                            top: 0;
                            transform: translateX(-50%);
                            width: 999%;
                            height: 1px;
                            background: #000;
                        }

                        &:first-child {
                            padding-left: 100px;
                        }

                        &:nth-child(3) {
                            font-size: 16px;
                            line-height: 17px;
                        }

                        &:last-child {
                            padding-right: 100px;
                        }
                    }
                }

                &.con {
                    position: relative;
                    // width: 1440px;
                    height: 595px;
                    box-sizing: border-box;
                    display: none;
                    flex-wrap: nowrap;


                    &.active {
                        display: table-row;
                    }

                    .close {
                        position: absolute;
                        content: '';
                        right: 40px;
                        bottom: 30px;
                        width: 52px;
                        height: 52px;
                        cursor: pointer;
                    }
                    
                    .mclose {
                        position: absolute;
                        content: '';
                        right: 40px;
                        bottom: 30px;
                        width: 40px;
                        height: 40px;
                        cursor: pointer;
                        display: none;
                    }

                    td {
                        .slider__wrap {
                            padding: 40px 100px 120px 100px;
                            width: 100%;
                            height: 100%;
                            display: flex;
                            align-items: center;
                        }
                        .slider__img {
                            position: relative;
                            width: calc(100vw - 200px);
                            height: 460px;
                            overflow: hidden;

                            &::before {
                                position: absolute;
                                content: '';
                                top: 0;
                                right: 0;
                                width: 100px;
                                height: 460px;
                                background: linear-gradient(to right, rgba(255,255,255,0) 0%, rgba(255, 255, 255, 0.7) 100%);
                                z-index: 9999;
                                // -webkit-backdrop-filter: blur(5px);
                                // backdrop-filter: blur(5px);
                            }

                            &::after {
                                position: absolute;
                                content: '';
                                top: 0;
                                left: 0;
                                width: 100px;
                                height: 460px;
                                background: linear-gradient(to left, rgba(255,255,255,0) 0%, rgba(255, 255, 255, 0.7) 100%);
                                z-index: 9999;
                                // -webkit-backdrop-filter: blur(5px);
                                // backdrop-filter: blur(5px);
                            }

                            .slider__inner {
                                display: flex;
                                flex-wrap: nowrap;
                                width: 120%;
                                height: 460px;

                                .slider {
                                    height: 460px;
                                    margin-right: 40px;

                                    &.image-column {
                                        column-width: 460px;
                                        column-gap: 40px;

                                        img{
                                            width: 460px;   
                                            height: 460px;
                                            object-fit: cover;
                                        }
                                    }

                                    &.text-column {
                                        column-width: 350px;
                                        column-gap: 40px;
                                        font-size: 24px;
                                        font-weight: 700;
                                        line-height: 26px;
                                    }

                                    &:last-child {
                                        margin-right: 0;
                                    }
                                }
                            }
                        }
                        .slider__btn {
                            img {
                                position: absolute;
                                transform: translate(-50%, -50%);
                                width: 52px;
                                height: 52px;
                                cursor: pointer;

                                &.prev {
                                    left: 50px;
                                }

                                &.next {
                                    right: 12px;
                                }
                            }
                        }
                    }
                }
            }
        }
    }
}

.footer {
    position: relative;
    text-align: center;
    margin-top: 20px;

    &::after {
        position: absolute;
        content: '';
        left: 50%;
        top: -20px;
        transform: translateX(-50%);
        width: 999%;
        height: 1px;
        background: #000;
    }

    img {
        width: 60px;
        height: 60px;
        cursor: pointer;
    }
}

.mfooter {
    position: relative;
    text-align: right;
    padding: 20px 20px 40px 20px;
    display: none;

    &::after {
        position: absolute;
        content: '';
        left: 50%;
        top: 0px;
        transform: translateX(-50%);
        width: 999%;
        height: 1px;
        background: #000;
    }

    img {
        width: 48px;
        height: 48px;
    }
}

@media (max-width: 780px) {
    .header {
        padding: 0 20px;
        padding-top: 40px;

        .ec {
            display: none;
        }
        .info {
            display: none;
        }
        .mi {
            display: block;
        }
    }

    .tableWrap {
        .table {
            thead {
                tr {
                    th {
                        &:first-child {
                            display: none;
                        }
    
                        &:nth-child(2) {
                            width: 100%;
                            padding: 20px;
                            font-size: 20px;

                            > div {
                                display: none !important;
                            }
                        }
    
                        &:nth-child(3) {
                            display: none;
                        }
    
                        &:last-child {
                            display: none;
                        }
                    }
                }
            }
            tbody {
                tr {
                    &.tit {
                        td {
                            &:first-child {
                                display: none;
                            }
        
                            &:nth-child(2) {
                                width: 100%;
                                padding: 20px !important;
                                font-size: 24px;
                            }
        
                            &:nth-child(3) {
                                display: none;
                            }
        
                            &:last-child {
                                display: none;
                            }
                        }
                    }

                    &.con {
                        .close {
                            display: none;
                        }

                        .mclose {
                            display: block;
                        }

                        td {
                            .slider__wrap {
                                padding: 0 20px 80px 20px;
                            }
                            .slider__img {
                                position: relative;
                                width: calc(100vw - 40px);
                                height: 100%;

                                &::before {
                                    display: none;
                                }

                                &::after {
                                    display: none;
                                }
                            }
                            .slider__inner {
                                flex-wrap: wrap;
                                width: 100%;
                                height: 100%;

                                .slider {
                                    height: 100%;
                                    margin-right: 0;
                                    margin-bottom: 20px;

                                    &.image-column {
                                        column-width: 350px;
                                        column-gap: 20px;

                                        img{
                                            width: 350px;   
                                            height: 350px;
                                            object-fit: cover;
                                        }
                                    }
                                }
                            }
                            .slider__btn {
                                display: none;
                            }
                        }
                    }
                }
            }
        }
    }

    .footer {
        display: none;
    }

    .mfooter {
        display: block;
    }
}
</style>