# power.css
The reset that gives power back to CSS.

Have you discovered [the owl selector](https://alistapart.com/article/axiomatic-css-and-lobotomized-owls/), only to find out that is basically useless in practice because of all the default user-agent styles? When is the last time you *actually* used inheritance in CSS?
This is the reset for people who think Cascading Stylesheets should cascade. With this reset you can fully take advantage of inheritance, cascading and axiomatic CSS.

## What you can do with this
This reset gives you full control over the style of every HTML element. With it, you'll spend less time fighting with the styles browsers add to a page and more time writing *exactly* what you want.
The idea is that it forces you to write more general styles. You can write basic rules first:
```
* + * { margin-top: 1em }
```
And then specialize depending on context:
```
main section + section { margin-top: 100px }
```
You work from the general to the specific, hopefully writing less code more beautifully.
You still deal with the browsers' *rendering* quirks, but not their *opiniated* stylesheets.

###Making HTML semantic again
How often do you use unordered lists to display a text-book style list in an article? HTML is *semantic*. Lists should be used whenever the concept of *listing* something is appropriate. We use `ul` all the time to enumerate various elements, and we constantly have to remove their default stylings, which assumes we are typesetting a recipe book. By removing the default styles, you can think specifically about your website and what you are most likely to do with lists. If you never ever use them with bullets, why ever declare a `list-style` property.
With this reset, you don't have to think about this. Lists have no styles by default. You can use semantically in your HTML page. Then, depending on context, add whatever you need. If you do use them in a text with bullet points, then perhaps something like this is more *semantically* relevant.
```
article ul li {
	/* Style actual text lists here. */
}
```
And if you don't need it, then you never see it!

## Get started
To use this reset, simply download the power.css file and include it in your HTML page, before any other CSS. Feel free to customize things.
This will make your HTML-only page look even more bare-bone than it normally would. You can now begin adding your custom styles. You might start a custom font. For example, you could add this style to the `:root` element.
```
:root {
	font-family: "Inter", Helvetica, Arial, sans-serif;
}
```
And if you have Inter on your computer, all text would be set using it. But that is an understatement. Usually, browsers redeclare fonts on some elements, notably forms. None of that with this reset. By default, this will change the font of **all** inheriting elements.
It's as simple as that.
You can now write your code as it should be, without thinking about what the browser thinks it should be.

## Compatibility
Unfortunately support for `all` is limited to modern browsers. This reset won't work in Internet Explorer, which is probably the least of your worries if you're interested in this.
[See the support table here.](https://caniuse.com/#feat=css-all)
