---
marp: true
theme: default
header: "**ヘッダータイトル1** __ヘッダータイトル2__"
footer: "by **＠NISHIZONO**"

size: 16:9
paginate: true

style: |
    section.split {
        overflow: visible;
        display: grid;
        grid-template-columns: 500px 500px;
        grid-template-rows: 100px auto;
        grid-template-areas: 
            "slideheading slideheading"
            "leftpanel rightpanel";
    }

    /* debug */
    section.split h3, 
    section.split .ldiv, 
    section.split .rdiv { border: 1.5pt dashed dimgray; }
    section.split h3 {
        grid-area: slideheading;
        font-size: 50px;
    }
    section.split .ldiv { grid-area: leftpanel; }
    section.split .rdiv { grid-area: rightpanel; }

---
<!-- _class: split -->
### A split slide

#### Title for the left panel 1
- listed item 1-1
- listed item 1- 2
- listed item 1-3
- listed item 1-4

#### Title for the left panel 2
- listed item 2-1
- listed item 2-2
- listed item 2-3
- listed item 2-4
