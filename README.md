# power.css
The reset that gives power back to CSS.


## What you can do with this
Most browsers declare default styling on most elements. When styling a website, you have to override browsers’ stylesheets to get what you want.

With this reset, you don’t have to think about this. All elements have no style by default.
You are free to use them semantically in your HTML page. Then, depending on context, style them as you need.

You still deal with the browsers’ *rendering* quirks, but not with their default stylesheet quirks.

This can make for some more elegant, shorter, and more readable CSS.


## Get started
To use this reset, download the `power.css` file and include it in your HTML page, before any other CSS. Feel free to customize things.

It will make your HTML-only page look even more bare-bones than it normally would. You can now begin adding your custom styles. You might start with a custom font. For example, you could add this style to the `:root` element.
```css
:root {
  font-family: "Inter", Helvetica, Arial, sans-serif;
}
```
If you have [Inter](https://github.com/rsms/inter) on your computer, all text would be set using it, but that’s an understatement. Usually, browsers redeclare fonts on some elements, notably forms. None of that with this reset. By default, this will change the font of **all** inheriting elements.

It’s as simple as that.


## Compatibility
Support for `all` has been widely available in major browsers since 2020, so this reset should be pretty safe to use.

[See the support table here.](https://caniuse.com/#feat=css-all)
