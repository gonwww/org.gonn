# org.gonn

![gonn.org](https://gonn.org/dsyim.svg "DSYiM")

- v1.0.0
    - 1/3/2022, Updated DSYiM to version v51. DSYiM v51 has simpler "Y" (similar to `++`) 
        and text representation will be `[++]`. It is modified "Yo" 
        character to make it symmetry vertically and horizontally.
        - Also, PNG and ICO have been updated accordingly.
        - Added meta description tags.
- v1.0.7
    - 1/18/2022, Able to download DSYiM created in https://gonn.org/logo/
        - eg. https://gonn.org/logo.svg#size=250&fill=red&stroke=white
        - eg. https://gonn.org/logo.svg?size=250&fill=red&stroke=white
        - eg. https://gonn.org/logo/
- v1.0.9
    - 1/18/2022, now /logo/ can set background color of the page.


## Todo

- [X] G100 -- Make it a structural outline -- instead of `section/h2` for title, 
    use `h1`, so it can be structured.
- [X] G101 -- Except for the main entry point (/), separate CSS and SVG into separate
    files.
- [X] G102 -- Change the color on `/enc` page to have more contrast.
- [X] G103 -- Recreated DSYiM from the scratch. (1/4/2023, v52)


## Notes

(1) Alternate way to deal with image

```html
<div>
	<object data="/dsyim-bg.svg" type="image/svg+xml">
              <img src="/dsyim-bg.svg" title="Gonn">
	</object>
</div>	
```	


(2) QR Code

For future, create some library that can add QR code when the page
is printed. create a hidden div in the header with an ID="qrCode", 
on-before-print, it will generate QR code and show, 
and on-after-print, it will be hide it back.

```javascript
window.onbeforeprint = () => doSomething();
window.onafterprint = () => undoSomething();
```




	