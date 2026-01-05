# decked-select

*decked-select* provides an [html decking layer](https://github.com/bahrus/be-decked-with) that can surround the select element.

It makes the select element [customizable](https://developer.mozilla.org/en-US/docs/Learn_web_development/Extensions/Forms/Customizable_select), and adds some styling to make the entire decked select have a material UI look and feel.

This package contains a few alternative decking layers, depending on what type of UI is desired:

1.  material-outline-ext-label.html -- external label 
2.  material-outline-int-label.html -- places thee label inside the top option.

## Sample markup - external label

```html
<script type=importmap >
{
    "imports": {
        "decked-select/": "node_modules/decked-select/"
    }
}
</script>
<script type=module>
    import 'be-decked-with/😶‍🌫️.js';
</script>

<select id=select
    data-label=Country
    😶‍🌫️-src="decked-select/material-outline-ext-label.html">
    <button>
        <selectedcontent></selectedcontent>
    </button>
    <option value="">Select a country</option>
    <option value="us">United States</option>
    <option value="uk">United Kingdom</option>
    <option value="ca">Canada</option>
    <option value="au">Australia</option>
    <option value="de">Germany</option>
    <option value="fr">France</option>
    <option value="jp">Japan</option>
</select>

```

## Sample markup - internal label

```html
<select id=select1
        😶‍🌫️-src="decked-select/material-outline-int-label.html"
        💍
    >
    <button>
        <selectedcontent></selectedcontent>
    </button>
    <option class=nothing-selected value=""><label for=select1>Country</label></option>
    <option class=something-selected value="">None</option>
    <option value="us">United States</option>
    <option value="uk">United Kingdom</option>
    <option value="ca">Canada</option>
    <option value="au">Australia</option>
    <option value="de">Germany</option>
    <option value="fr">France</option>
    <option value="jp">Japan</option>
</select>
```

Having two empty options with classes nothing-selected and something-selected is optional.  This is only if you want what the option text to change when another option is selected.

## Recommended vscode extensions:

[json-in-html, custom link attributes, idref](https://marketplace.visualstudio.com/publishers/andersonbruceb)



