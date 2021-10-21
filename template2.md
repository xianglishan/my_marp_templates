---
marp: true
theme: default
header: "**ヘッダータイトル1** __ヘッダータイトル2__"
footer: "by **＠NISHIZONO**"

size: 16:9
paginate: true

style: |
    section.title {
        --title-height: 130px;
        --subtitle-height: 70px;

        overflow: visible;
        display: grid;
        grid-template-columns: 1fr;
        grid-template-rows: 1fr var(--title-height) var(--subtitle-height) 1fr;
        grid-template-areas: "." "title" "subtitle" ".";
    }

    section.title h1,
    section.title h2 {
        margin: 0;
        padding: 0;
        text-align: center;
        height: var(--area-height);
        line-height: var(--area-height);
        font-size: calc(var(--area-height) * 0.7);

        border: 1px dashed gray; /* debug */
    }

    section.title h1 {
        grid-area: title;
        --area-height: var(--title-height);
    }

    section.title h2 {
        grid-area: subtitle;
        --area-height: var(--subtitle-height);
    }

    section {
        justify-content: start;
    }

---
<!-- _class: title -->
# タイトル
## サブタイトル

---
# スライド1
## スライド1サブタイトル
- あああ
- いいい
- ううう

---
# スライド2
## スライド2サブタイトル
- あああ
- いいい
- ううう
