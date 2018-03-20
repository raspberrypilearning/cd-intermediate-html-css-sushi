## All the colours!

As you have seen, you can type in many different colour names as words and the browser will recognise them. But a more common way to set colours is to use something called a **HEX** code (HEX is short for **hexadecimal**, a special way of counting).

+ Take a look at your **stylesheet**. That's the file that has `.css` in the name.

+ Inside the CSS rules for **body**, set the background colour to

```html
  background-color: #7B68EE;
```

Note: If you are using a Mac, the `#` is typed by holding the `alt` key and the number `3` key together.

Your website should now have a purple background. 

![](images/HexColourFirst.png) 
![](images/HexColourFirstResult.png)


+ Not a fan of purple? Go to [dojo.soy/html2-colors](http://dojo.soy/html2-colors) and choose another colour for your stylesheet. But instead of typing the name of the colour, type in the **HEX** code. 

![](images/ColorNamesHex.png)

Colour codes allow you to mix any colour, even if it's not on any list of colours. 

+ Try making up your own colour code. It must start with a `#`. This tells the browser that it is a HEX code instead of a colour name. The rest of the code is made up of six characters. They can be  any number from **0-9** and any letter from **A-F**.

--- collapse ---
---
title: How does it work? 
---

Every colour is made by mixing different amounts of **Red**, **Green**, and **Blue**. You will sometimes see this written down as **RGB**. Each of these colours is represented by two of the six digits in your HEX code. `00` is none and `FF` is the maximum.

**Hexadecimal** is a way of counting that makes numbers shorter to write by using the letters A-F as extra digits. The number `255` is written as `FF` in hexadecimal. 

You don't need to worry too much about learning to count with Hexadecimal numbers. Instead, experiment with different colour codes to get used to using them.

The table below shows some basic colours. They've been broken up so you can more clearly see the red, green, and blue parts.

| \# | Red | Green | Blue | Colour     |
|----|-----|-------|------|------------|
| \# | FF  |   00  |  00  | Red        |
| \# | 00  |   FF  |  00  | Green      |
| \# | 00  |   00  |  FF  | Blue       |
| \# | FF  |   FF  |  00  | Yellow     |
| \# | FF  |   00  |  FF  | Magenta    |
| \# | 00  |   FF  |  FF  | Cyan       |
| \# | FF  |   8c  |  00  | DarkOrange |

+ Try some of them out in your website and then try putting in smaller numbers instead of `FF` to see how the shades change.

--- /collapse ---

Mixing the perfect colour can take a lot of experimenting. Luckily, there are plenty of colour picking tools that help you get the HEX code for any colour you want. 

![](images/W3ColorPicker.png)

+ Go to [dojo.soy/html2-color-picker](http://dojo.soy/html2-color-picker) and try out the colour picker to choose some HEX colour codes to use for the rest of the styles on your website.



