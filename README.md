## CSS Chapter 24
It is my coding practice with the TUTORIAL of Dave Gray. 

## Source
### Dave Gray 的 CSS 課程
https://youtube.com/playlist?list=PL0Zuz27SZ-6Mx9fd9elt80G1bPcySmWit

### Dave Gray 的 YouTube 頻道
https://www.youtube.com/@DaveGrayTeachesCode

## CSS Chapter 24
   Quick Concept outline
   中文摘要說明與重點提問

###  1. Intro
        教學影片固定的開頭

###  2. Welcome
        歡迎觀眾，說明工具與資料位置

###  3. Project Intro
        專案介紹

###  4. Starter Code
        初始程式碼

###  5. HTML head and meta tags
        (1)新增 about.html 的 html, head, body 的架構
        (2)新增 RWD 至 home.html, hours.html, contact.html
        (3)新增 about.html 的網頁描述，title，圖標和匯入 css 樣式
        (4)修改網頁的描述和 title

###  6. HTML header, nav and hero
        home.html:
        (1)在 header 下面新增 section，並貼上 figure 和移除 hr
        (2)使用 BEM: Block Element Modifier 命名常規，
        新增 header 的 class 為 header, h1 的 class 為 header__h1, 
        nav 的 class 為 header__nav, ul 的 class 為 header__ul
        (3)將 about 的超連結移動至最下方，連結至 about.html
        (4)修改連結文字為 Menu, Hours, Contact, About
        (5)在 section 中新增 h2，文字為 Bienvenidos!。
        使用 BEM，新增 section 的 class 為 hero，h2 的 class 為 hero__h2
        (6)修改圖片解析度較高的圖片，圖片檔案為 tacos_and_drink_1000x667.png，
        預設寬度為 1000px，高度為 667px
        (7)新增 figcaption 的 class 為 offscreen

        about.html:
        (1)複製 home.html 的 header 和 section 至 about.html
        (2)將 about 的超連結移動至最上方，連結至首頁 home.html，文字修改為 Home，
        第二個超連結至 home.html 的 menu 的位置
        (3)修改 h1 的文字為 Little Taco Shop
        (4)移除 section 的 h2
        (5)修改圖片檔案為 tacos_delicioso_1000x667.png，預設寬度為 1000px，高度為 667px，
        圖片未顯示時的文字為 Tacos Delicioso，title 為 Tacos Delicioso!
        (6)修改 figcaption 文字為 Try these Delicious Tacos

        hours.html:
        (1)移動第二個超連結至最後，連結至 about.html
        (2)修改連結文字為 Home, Menu, Contact, About
        (3)在 header 下面新增 section，並貼上 figure 和移除 hr
        (4)修改圖片檔案為 tacos_tray_1000x667.png，預設寬度為 1000px，高度為 667px
        (5)新增 figcaption 的 class 為 offscreen，section 的 class 為 hero
        (6)新增 header 的 class 為 header, h1 的 class 為 header__h1, 
        nav 的 class 為 header__nav, ul 的 class 為 header__ul

        contact.html
        (1)新增 header 的 class 為 header, h1 的 class 為 header__h1, 
        nav 的 class 為 header__nav, ul 的 class 為 header__ul
        (2)移動第二個超連結至最後，連結至 about.html
        (3)修改連結文字為 Home, Menu, Hours, About
        (4)在 header 下面新增 section，並貼上 figure 和移除 hr
        (5)新增 figcaption 的 class 為 offscreen，section 的 class 為 hero
        (6)修改圖片檔案為 tacos_close_up_1000x649.png，預設寬度為 1000px，高度為 649px

###  7. Importing Google fonts
        匯入 Nurito 文字的 CSS 樣式

###  8. CSS Reset
        (1)重置 *, *::before, *::after
        (2)重置 img
        (3)重置 input, button, textarea

###  9. CSS Variables
        字體: 
        (A1)設定 font-family 變數 --FF 為 "Nunito", sans-serif
        (A2)設定 --FF-HEADGINGS 為 "Fugaz One", cursive
        (A3)設定 font-size 變數 --FS 為 clamp(1rem, 2.2vh, 1.5rem)

        顏色: 
        (B1)設定 background-color 變數 --BGCOLOR 為橘色
        (B2)設定 --BGCOLOR-FADE 為 rgb(252, 220, 160)
        (B3)設定 --BGIMAGE 為 linear-gradient(to bottom, var(--BGCOLOR), var(--BGCOLOR-FADE))
        (B4)設定 --BODY-BGCOLOR 為白色
        (B5)設定 --FONT-COLOR 為黑色

### 10. CSS Utility Classes
        (1)設定 .offscreen 移除特定內容
        (2)設定 .nowrap 使特定文字不換行
        (3)設定 .center 使文字置中

### 11. General Styles
        html 通用樣式
        (1)設定 scroll-behavior 為 smooth
        (2)設定字體大小、字體家族、背景顏色和背景影像

        body 通用樣式
        (1)設定背景顏色和文字顏色
        (2)設定最低高度為 100vh，最大寬度為 800px
        (3)設定 margin 為 0 auto，使頁面置中。
        (B6)設定 --BORDER-COLOR 為 #333
        (C1)設定 --BORDERS 為 1px solid var(--BORDER-COLOR)
        (4)設定 border-left 和 border-right 為 var(--BORDERS)
        (5)設定 box-shadow 為 0 0 10px var(--BORDER-COLOR)

        h1, h2, h3 通用樣式
        (1)設定字體家族為 var(--FF)
        (2)設定字母間隔為 0.1em

        h2, h3 通用樣式
        (1)設定 margin-bottom 為 1em
        (B7)設定 --HIGHLIGHT-COLOR 為 rgb(51, 178, 51)
        (2)設定文字顏色為 var(--HIGHLIGHT-COLOR)

        p 通用樣式
        設定列高為 1.5

        超連結通用格式
        (B8)設定 --LINK-COLOR 為黑色
        (B9)設定 --LINK-HOVER 為 hsla(0, 0%, 0%, 0.6)
        (B10)設定 --LINK-ACTIVE 為橘色
        (1)設定 a:any-link 文字顏色為 var(--LINK-COLOR)
        (2)設定 a:hover, a:focus-visible 文字顏色為 var(--LINK-HOVER)
        (3)設定 a:active 文字顏色為 var(--LINK-ACTIVE)

### 12. header and nav styles
        header 樣式
        (1)設定 position 為 sticky
        (2)設定 top 為 0
        (3)設定 z-index 為 1

        h1 樣式
        (1)設定文字置中
        (B11)設定 header 背景顏色 --HEADER-BGCOLOR 為黑色
        (B12)設定 header 文字顏色 --HEADER-COLOR 為白色
        (B13)設定 nav 背景顏色 --NAV-BGCOLOR 為白色
        (D1)設定 padding 的上下範圍 --PADDING-TB 為 0.25em
        (D2)設定 padding 的左右範圍 --PADDING-SIDE 為 2.5%
        (E)設定 margin 的範圍 --MARGIN 為 clamp(1em, 2.5vh, 1.5em) 0
        (2)設定背景顏色、文字顏色、padding

        nav 樣式
        (1)設定背景顏色為 var(--NAV-BGCOLOR)
        (2)設定 border-bottom 為 var(--BORDERS)
        (3)設定字體粗細為 bold
        (4)設定 box-shadow 為 0 6px 5px -5px var(--BORDER-COLOR)

        ul 樣式
        (1)設定 padding 為 var(--PADDING-TB) var(--PADDING-SIDE)
        (2)設定 list-style-type 為 none
        (3)設定 display 為 flex
        (4)設定 justify-content 為 space-evenly
        (5)設定 gap 為 1rem

        修改 home.html 的文字為 Little Taco Shop


        hero (section 樣式)
        設定 position 為 relative

        h2 樣式
        (B14)設定 --HERO-BGCOLOR 為 rgba(51, 178, 51, 0.75)
        (1)設定背景顏色為 var(--HERO-BGCOLOR)
        (B15)設定 --HERO-COLOR 為白色
        (2)設定文字顏色為 var(--HERO-COLOR)
        (3)設定 padding 為 0.25em 0.5em
        (4)設定文字陰影為 2px 2px 5px var(--BORDER-COLOR)
        (5)設定 position 為 absolute
        (6)設定 left 為 20px
        (7)設定 top 為 -100px
        (8)設定 animation 為 showWelcome 0.5s ease-in-out 1s forwards

        動畫框架
        (1)設定名稱為 showWelcome
        (2)0%，top 為 -20px，transform 為 skew(0deg, -5deg) scaleY(0);
        (3)80%，top 為 30px，transform 為 skew(10deg, -5deg) scaleY(1.2);
        (4)100%，top 為 20px，transform 為 skew(-10deg, -5deg) scaleY(1);

### 13. HTML footer and main
        footer
        (1)新增 footer 的 class 為 footer
        (2)新增兩個 span 的 class 為 nowrap，
        文字為 Copyright © 和 Little Taco Shop。
        (3)修改 home.html, about.html, hours.html, contact.html 的 footer 格式

        main
        home.html
        (1)新增 main 的 class 為 main
        (2)移動 home.html，id 為 about 的 article 至 about.html
        (3)article 的 class 為 main__article

        about.html
        (9)新增 article 的 class 為 main__article

        hours.html
        (4)新增 main 的 class 為 main
        (5)新增 article，class 為 main__article
        (6)新增 h2 文字為 Hours

        contact.html
        (7)新增 main 的 class 為 main
        (8)將 section 改為 article，class 為 main__article
        (9)移動地址和聯絡電話的 article 至表單 article 上方
        (10)在兩個 article 之間新增水平線

### 14. footer styles
        (1)設定 position 為 sticky，bottom 為 0
        (2)設定背景顏色為 var(--HEADER-BGCOLOR)
        (3)設定文字顏色為 var(--HEADER-COLOR)
        (4)設定 padding 為 var(--PADDING-TB) var(--PADDING-SIDE)
        (5)設定文字置中

### 15. main styles
        main 樣式
        設定 padding 為 var(--PADDING-TB) var(--PADDING-SIDE)

        article 樣式
        (1)設定 scroll-margin-top 為 6.5rem
        (2)設定 margin 為 var(--MARGIN)
        (3)設定第一個 article 的 margin-top 為 1em
        (4)設定最後一個 article 的 min-height 為 calc(100vh - 20rem)

### 16. About styles
        about.html
        (1)在 main 中，新增 article 的 class 為 about
        (2)新增 aside 的 class 為 about__trivia
        (3)新增 p 的 class 為 about__trivia-answer

        about 樣式
        (1)設定 about__trivia 的 margin 為 var(--MARGIN)
        (2)設定 about__trivia-answer 的 margin-top 為 1em

### 17. Contact form styles
        contact.html
        (1)在 main 中，新增 article 的 class 為 contact
        (2)新增 h2 的 class 為 contact__h2
        (3)新增 form 的 class 為 contact__form
        (4)新增 fieldset 的 class 為 contact__fieldset
        (5)新增 legend 的 class 為 offscreen
        (6)新增 p 的 class 為 contact__p
        (7)新增 label 的 class 為 contact__label
        (8)新增 input 的 class 為 contact__input
        (9)新增 textarea 的 class 為 contact__textarea
        (10)新增 button 的 class 為 contact__button

        contact 樣式
        (1)設定 contact__h2 的 margin 為 0
        (2)設定 contact__fieldset 的 border 為 none
        (3)設定 contact__p 的 margin 為 1em 0
        (4)設定 contact__label 的 display 為 block，字體粗細為 bold
        (5)設定 contact__input 和 contact__textarea 的 padding 為 0.5em，
        border-radius 為 15px，border-width 為 2px，width 為 100%
        (B16)設定 --BUTTON-COLOR 為白色
        (6)設定 contact__button 的 padding 為 0.5em，border-radius 為 15px，
        背景顏色為 var(--HIGHLIGHT-COLOR)，文字顏色為 var(--BUTTON-COLOR)，
        字體粗細為 bold

### 18. Reviewing progress
        再次閱覽，並開啟 Google 開發工具

### 19. Heading and title consistency
        hours.html, contact.html
        修改 h1 為 Little Taco Shop

        about.html
        修改分頁名稱為 About LTS

### 20. Converting an HTML table to a CSS grid
        display: contents
        https://caniuse.com/?search=display%3A%20content

### 21. Menu styles
        home.html
        (1)在 main 中，新增 article 的 class 為 menu
        (2)新增 h2 的 class 為 menu__h2
        (3)新增 table 的 class 為 menu__container
        (4)新增 caption 的 class 為 offscreen
        (5)在 thead 中，新增 th 的 class 為 menu__header
        (6)設定 th 的 scope 為 col，修改文字為 Tacos, Quantity, Price

        (7)在 tbody 中，新增 td 的 class 為 menu__item
        (8)新增第一個 th 的 class 為 menu__item 和 menu_cr，cr 為 crunchy，
        第二個 th 的 class 為 menu__item 和 menu_sf，sf 為 soft
        (9)在 tfoot 中，新增 td 的 class 為 menu__item menu__cs，cs 為 chips and salsa
        (10)移除 br，設定 p 的 class 為 center，使 Back To Top 文字置中

        Menu 樣式
        (1)設定 thead, tbody, tfoot, tr 的 display 為 contents
        (2)設定 menu__container 的 display 為 grid，
        grid-template-columns 為 repeat(3, 1fr)
        (3)設定 menu__container 的 grid-template-areas
        "hd1 hd2 hd3"
        "cr cr1 cr1p"
        "cr cr2 cr2p"
        "cr cr3 cr3p"
        "sf sf1 sf1p"
        "sf sf2 sf2p"
        "sf sf3 sf3p"
        "cs cs cs"
        (4)設定 menu__container 的 gap 為 0.1em，margin-bottom 為 1em
        (5)設定 menu__cr 的 grid-area 為 cr
        (6)設定 menu__sf 的 grid-area 為 sf
        (7)設定 menu__cs 的 grid-area 為 cs
        (8)設定 menu__header, menu__cr, menu__sf, menu__cs 的 
        color 為 var(--HIGHLIGHT-COLOR)，字體粗細為 bold，高度為 100%，
        display 為 grid，place-content 為 center
        (9)設定 menu__header, menu__item 的寬度為 100%，padding 為 1em，
        border 為 medium ridge var(--BORDER-COLOR)
        (10)設定 menu__item 的 display 為 grid，place-content 為 center
        (11)選取表格中的 Tacos，設定左上角為圓角
        (12)選取表格中的 Price，設定右上角為圓角
        (13)選取表格中的 Chips & Salsa，設定左下角和右上角為圓角

        Contact 樣式
        (C2)設定 --BORDER-RADIUS 為 15px
        (1)設定 contact__input, contact__textarea 的 border-radius 為 var(--BORDER-RADIUS)
        (2)設定 contact__button 的 border-radius 為 var(--BORDER-RADIUS)

### 22. Evaluating desktop and mobile views
        評估桌上型電腦和行動裝置瀏覽頁面

### 23. Adding a media query
        (1)設定當寬度在 576px 以上，在 Little Taco Shop 前方和後方添加圖示🌮
        (2)設定當寬度在 576px 以上，表格的字體大小增加 25%

### 24. Adding dark mode
        設定偏好的顏色主題為暗色
        (B1)設定 --BGCOLOR 為黑色
        (B2)設定 --BGCOLOR-FADE 為灰色
        (B4)設定 --BODY-BGCOLOR 為 #333
        (B5)設定 --FONT-COLOR 為白煙色
        (B6)設定 --BORDER-COLOR 為白煙色
        (B7)設定 --HIGHLIGHT-COLOR 為白煙色
        (B8)設定 --LINK-COLOR 為白煙色
        (B9)設定 --LINK-HOVER 為橘色
        (B10)設定 --LINK-ACTIVE 為 rgb(252, 200, 103)
        (B12)設定 --HEADER-COLOR 為白煙色
        (B13)設定 --NAV-BGCOLOR 為 rgb(20, 20, 20)
        (B15)設定 --HERO-COLOR 為 #333
        (B16)設定 --BUTTON-COLOR 為黑色

### 25. Organizing the CSS
        按下 Ctrl + P，輸入>，選擇 Sort Line Ascending
        (1)排列顏色的變數
        (2)排列偏好的顏色主題變數

### 26. Preview: A touch of JavaScript
        (1)在 Copyright &copy; 後面，新增 time 的 id 為 year
        (2)新增 main.js 設定年份
        (3)匯入 main.js

### 27. Final Notes and changes
        可以依照個人喜好修改 CSS 樣式
