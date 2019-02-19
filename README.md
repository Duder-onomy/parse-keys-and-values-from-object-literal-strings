# DEPRECATED!!!

There is a much better / still maintained, and as it turns out, the original version of this code over here: https://github.com/mbest/js-object-literal-parse

All credit goes to https://github.com/mbest

---

# Parse Keys And Values From Object Literal Strings

This library will turn a string like this:

`'{ yeah : bro, no : dawg }'`

Into:
```javascript
[
    {
        key : 'yeah',
        value : 'bro'
    },
    {
        key : 'no',
        value : 'dawg'
    }
]
```

Thats it!
Pretty cool huh?

Install it like so: 
`npm install --save-dev parse-keys-and-values-from-object-literal-strings`


I use it in my custom attribute library but it could be used in other places as well.


Inspiration: I was implementing something like this for my custom attribute library:

```html
<div on-event='{ click : handleClick, mouseover : handleMouseOver, mouseOut : handleMouseOut }'></div>
```

Knockout.js does it. Angular does it. Jade does it. Ember does it. Why cant I do it too?
Anyways, I reverse engineered it from knockout.js source code. Sue me.
