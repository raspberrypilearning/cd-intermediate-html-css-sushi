## All the colours!

As you have seen, you can type in many different colour names as words and the browser will recognise them. But a more common way to set colours is to use something called a **HEX** code.

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

HEX codes allow you to mix any colour, even if it's not on any list of colours. 

+ Try making up your own colour code
   * The code must start with a `#`. This tells the browser that it is a HEX code instead of a colour name.
   * The rest of the code is made up of six characters. They can be  any number from **0-9** and any letter from **A-F**.

--- collapse ---
---
title: How does it work? 
---

Every colour is made by mixing three colors: **Red**, **Green**, and **Blue**. You will sometimes see this written down as **RGB**. Each of these colours is represented by two of the six digits in your HEX code. The higher the number, the more of the colour there is.

The HEX colour code doesn't use ordinary numbers that we're used to counting with, but another type called **Hexadecimal**. It's a special way of counting that uses the letters A-F as **extra digits** higher than 9. This makes the numbers shorter to write. 

Colours go from `0` up to `255`, or in Hexadecimal: from `00` up to `FF`. If you wrote the colour `#9ADC32` using plain RGB numbers, it would be `rgb(154,205,50)`.

You don't need to worry too much about learning to count with Hexadecimal numbers, but do experiment to get used to a few colours! Below are the three most basic colours. 

+ Try setting your background to each of these colours in turn. 
 `#FF0000` is red
 `#00FF00` is green
 `#0000FF` is blue
 
`FF` is the highest value you can set for a colour. What do you think will happen if you use **less** of a colour? 

+ Change `FF` to something smaller like `88` or `33` in each of the above colours and see.

You can mix HEX colours just like you can mix paint, by adding different amounts of red, green, or blue.

+ Try mixing **red** and **blue**, like this: `#FF00FF`. 

+ How about **red** and **green**? It looks like this: `#FFFF00`.

+ Try mixing with more of one colour and less of the other, for example `#FF8800`

--- /collapse ---

Mixing the perfect colour can take a lot of experimenting. Luckily, there are plenty of colour picking tools that help you get the HEX code for any colour you want. 

![](images/W3ColorPicker.png)

+ Go to [dojo.soy/html2-color-picker](http://dojo.soy/html2-color-picker) and try out the colour picker to choose some HEX colour codes to use for the rest of the styles on your website.



