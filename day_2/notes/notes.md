- [1. Day 2](#1-day-2)
  - [1.1. em](#11-em)
    - [1.1.1. em as font size](#111-em-as-font-size)
  - [1.2. rem](#12-rem)

# 1. Day 2

"Learning about ems and rems"

"These help to make the site easier to change with things like media queries to change html font-size"

> 10/02/2021

## 1.1. em

"1em usually defaults to 16px if the parent has no font size set, setting it to 2.5em would mean it's 2.5x bigger than parent font size."

"This doesn't just apply to font-size, works for padding etc. When you are using em for the margin, it looks at the font size of the element to get the size e.g"

```css
    .element {
        font-size: 2.5em;
        margin: 1em;
    }
```
"In the snippet above the margin would be equal to the font size as it is 1x2.5em and 2.5 em is relevant to the parent font size, so if it is 16px font-size then it would be 16x2.5x1 = 40px"

"Useful for making padding that adapts to changes in a button size for example"

### 1.1.1. em as font size

"You have to be careful using ems for font sizes as it stacks, so a small increase in font size of a parent could cause a large increase in child components sizes"

"Use mainly for padding and margins so they can grow and change proportionally with the font sizes of the element"


## 1.2. rem

"Designed to fix the compounding nature of ems, stands for 'Root em'"

"Looks at the html font size (the root)"

"For margins with rems it will always look at the root, so if"

```css
    .html {
        font-size: 16px;
    }

    .element {
        margin: 2rem;
    }
```
"This will make the margin 32px"

"Rem is useful for making proportional margins, so the spacing between elements"