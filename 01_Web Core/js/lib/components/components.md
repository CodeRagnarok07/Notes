



%% Begin Waypoint %%
- **[[components]]**
	- **carrusel**
		- [[Carrusel With options]]
		- **controls**

		- **img_control**
			- [[Carrusel img-control]]
	- [[components]]

%% End Waypoint %%




#### ???
```js
/** re render products */
function setOrderAlf(e) {
    const filter_alf = $("#filter_alf")
    const products = $("#products")
    if (e) {
        filter_alf.children[0].innerHTML = "ORDEN: A - Z"
        products.innerHTML = `{% for i in page_obj|dictsort:"nombre" %}{% include './item_product.html' %}{% endfor %}`
    } else {
        filter_alf.children[0].innerHTML = "ORDEN: Z - A"
        products.innerHTML = `{% for i in page_obj|dictsortreversed:"nombre" %}{% include './item_product.html' %}{% endfor %}`
    }
}
```

### tooltip with options
```js
// 
(() => {
    const all_tooltip_options = document.getElementsByClassName("tooltip_options")

    for (const tooltip of all_tooltip_options) {

        const parent = tooltip.parentElement

        tooltip.className += " hidden"
        parent.className += " parent_tooltip_options"

        const svg_icons = document.createElement("div")
        svg_icons.innerHTML = ` 
        <svg width="12" height="7" viewBox="0 0 12 7" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path
                d="M6.00032 6.75008C5.80149 6.74922 5.61086 6.67072 5.46907 6.53133L0.469074 1.53133C0.328178 1.39043 0.249023 1.19934 0.249023 1.00008C0.249023 0.800823 0.328178 0.609726 0.469074 0.46883C0.609971 0.327934 0.801067 0.248779 1.00032 0.248779C1.19958 0.248779 1.39068 0.327934 1.53157 0.46883L6.00032 4.93758L10.4691 0.46883C10.61 0.327934 10.8011 0.248779 11.0003 0.248779C11.1996 0.248779 11.3907 0.327934 11.5316 0.46883C11.6725 0.609726 11.7516 0.800823 11.7516 1.00008C11.7516 1.19934 11.6725 1.39043 11.5316 1.53133L6.53157 6.53133C6.38979 6.67072 6.19916 6.74922 6.00032 6.75008Z"
                fill="white" />
        </svg>
        <svg class="hidden" width="12" height="7" viewBox="0 0 12 7" fill="none"
            xmlns="http://www.w3.org/2000/svg">
            <path
                d="M11.0003 6.74989C10.8015 6.74903 10.6109 6.67053 10.4691 6.53114L6.00032 2.06239L1.53157 6.53114C1.39068 6.67203 1.19958 6.75119 1.00032 6.75119C0.801067 6.75119 0.609971 6.67203 0.469074 6.53114C0.328178 6.39024 0.249023 6.19915 0.249023 5.99989C0.249023 5.80063 0.328178 5.60953 0.469074 5.46864L5.46907 0.468638C5.53875 0.398718 5.62155 0.343241 5.71271 0.305387C5.80387 0.267533 5.90161 0.248047 6.00032 0.248047C6.09903 0.248047 6.19677 0.267533 6.28794 0.305387C6.3791 0.343241 6.4619 0.398718 6.53157 0.468638L11.5316 5.46864C11.6015 5.53832 11.657 5.62111 11.6948 5.71227C11.7327 5.80344 11.7522 5.90118 11.7522 5.99989C11.7522 6.0986 11.7327 6.19634 11.6948 6.2875C11.657 6.37867 11.6015 6.46146 11.5316 6.53114C11.3898 6.67053 11.1992 6.74903 11.0003 6.74989Z"
                fill="white" />
        </svg>`

        const clicker = document.createElement("div")
        clicker.className = "clicker"


        const activador = () => {
            tooltip.classList.toggle("hidden")
            svg_icons.children[0].classList.toggle("hidden")
            svg_icons.children[1].classList.toggle("hidden")
        }

        clicker.onclick = () => activador()

        parent.appendChild(clicker)
        parent.appendChild(svg_icons)
    }
})();
```


//  Carrusel Slider with controls



// 

/** PROGRES FORM */





