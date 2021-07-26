# Typography Notes
`Typography`
- – style or appearance of text,
- – the art of working with text.

## Terminology
### The Anatomy of a Typeface
`Ascender` - The portion of a letter that extends above the mean line of a font -- i.e., is taller than the font's x-height. (In this case, you will also notice the letter ‘h’ is taller than the x-height.) _(`5`)_

`Baseline` - The line where the letters sit. _(`5`)_

`Bowl` - The curved part of the character that encloses the circular or curved parts of some letters, like ‘d’, ‘b’, ‘o’, ‘d’, and ‘b’. (In the case, it is that round shape sticking off the letter ‘a’.) _(`5`)_

`Cap height` - The distance from the baseline to the top of the capital letter. _(`5`)_

`Cross bar` - The bar that goes across the inside of the letter and connects one side to another. (In this case, it is the bar inside the capital letter 'B’.) _(`5`)_

`Counter` - The empty space in the middle of letters such as ‘B’, ‘O’, or ‘A’. _(`5`)_

`Descender` - The longest point on a letter that falls beyond the baseline. _(`5`)_

`Finial` - The tapered end of letters such as ‘e’ or ‘c’. _(`5`)_

`Hierarchy` – is used to guide the reader’s eye to whatever is most important. In other words, it shows them where to begin and where to go next using different levels of emphasis. _(`1`)_

`Kerning` – is the space between specific characters. _`*`_ Some fonts have what we call `bad kerning`, making certain letters look improperly spaced. If a font you are using has bad kerning, it is best to cut your losses and choose something else. _(`1`)_

`Leading` – is the space between lines of text, also known as line spacing. _(`1`)_

`Ligature` - The stroke that joins adjacent letters. _(`5`)_

`Serif` - The slight projection finishing off a stroke of a letter in certain typefaces. (In this case, it is that little foot sticking off the letter ‘l’.) _(`5`)_

`Spine` - The curvy body of the letter 's' -- and only the letter ’s’. It gets its own term because the spine can be almost vertical or mostly horizontal, depending on the typeface. _(`5`)_

`Stem` - The base of a letter, like the stem of a flower. _(`5`)_

`Tracking` – is the overall space between characters, sometimes called character spacing. _(`1`)_

`Terminal` - A type of curve that you see at the top of the letter ‘f’ or the end of the letter ‘j’. _(`5`)_

`X-height` - Located in between the baseline and the cap height, it is the height of the body of the lowercase letter. (In this case, it is the letters ‘a’, ’u’, and ‘y’.) _(`5`)_

### Common Font Classification Types
`Type Families` - “type family” or “typeface family” is used to describe a range of designs that are all variations of one basic typeface. _(`5`)_

`Display` – Because of their decorative nature, display fonts are best for small amounts of text; for example, title and herders, and more graphic-heavy designs. _(`1`)_
-	Script
-	Blackletter
-	All-caps
-	Plain Fancy
- _`*`_ When deciding which fonts to use, less is more. It is best to limit yourself to one or two per project. If you need more contrast, try repeating one of your fonts in a different size, weight, or style.

`San serif` – fonts do not have that extra stroke-hence the name, which is French for “without serif”. _`*`_ This style is considered cleaner and more modern than serif fonts. Also, it tends to be easier to read on computer screens, including smartphones and tablets. _(`1`)_

`Serif` – fonts have little strokes called serifs attached to the main part of the letter. _`*`_ Because of their classic look, they are a good choice for more traditional projects. They are also common in print publications, like magazines and newspapers. _(`1`)_

## Typography Essentials
`Using letter as form` – Each letter is a shape unto itself, a shape that may serve as an illustration, as an icon, as a vessel, or as a graphic focal point, apart from its meaning as an alphabetic unit. _(`4`)_

`Using counter spaces as form` – The space inside and around the shape of a letter, called counter spaces, are often overlooked as design elements. _`*`_ Their shapes can be customized using color, pattern, or texture. The beauty of counter spaces, sometimes called “negative” spaces, is that they are the jewels that are already tucked into the letters… using them well is like discovering buried treasure. _(`4`)_

`Letterform details` – Specialized detailing can communicate apart from the literal message; whether customized or built in as alternate character within a typeface, even a simple swash or ligature can add an extra level of meaning or make the design more specific to the message. _(`4`)_

`Emotional content implied by the text` – Letterforms can amplify the emotional weight of the text. *The delicate tracery of a flowing italic might best convey a poem about nature. _(`4`)_

`Historical connotation` – typefaces area product of their era. A good design may be well served with a historically appropriate typeface choice when possible. _(`4`)_

`Vertical Rhythm` – Improves readability and helps to make the layout harmonious and organized. Vertical Rhythm on the web is contributed to by font-size, line-height, and margin size. _(`6`)_

`Combining fonts` - When deciding which fonts to use, less is more. It's best to limit yourself to one or two per project. If you need more contrast, try repeating one of your fonts in a different size, weight, or style. *You've probably heard that opposites attract.* _(`1`)_

## Typography Code Basics Essentials
### CSS
`Kerning`:
```css
CSS rule { letter-spacing: 1rem; }
```

`Leading`:
```css
CSS rule { line-height: 1.2; }
```

`Tracking`:
```css
CSS rule { word-spacing: 1rem; }
```

### SVG
`SVG` - An essential part of a text is the font in which it is displayed. SVG offers a set of attributes, many like their CSS counterparts, to enable font selection. _(`3`)_
```html
<text x="10" y="10">Hello World!</text>
```
#### Setting font properties
font-family:
- font-style
- font-weight
- font-variant
- font-stretch
- font-size
- font-size-adjust
- kerning
- letter-spacing
- word-spacing
- text-decoration

`Text-Anchor` – An attribute is used to align (`stat-`, `middle-`, or `end-alignment`) a string of pre-formatted text or auto-wrapped text where the wrapping area is determined from the inline-size property relative to a given point. _(`3`)_
```html
<text text-anchor="start" x="60" y="40">A</text>
```

`Dominant-Baseline` – An attribute specifies the dominant baseline, which is the baseline used to align the box’s text and inline-level contents. (`auto` | `text-bottom` | `alphabetic` | `ideographic` | `middle` | `central` | `mathematical` | `hanging` |` text-top`) _(`3`)_
```html
<text dominant-baseline="auto" x="30" y="20">Auto</text>
```

`Tspan` – element has the following custom attributes. _(`3`)_
```html
<text>
  This is <tspan font-weight="bold" fill="red">bold and red<tspan>
</text>
```
#### Attributes
- `textPath` - This element fetches via its *`xlink:href`* attribute an arbitrary path and aligns the characters, that it encircles, along this path. _(`3`)_

- `href` - The URL to the path or basic shape on which to render the text. If the path attribute is set, href has no effect. _(`3`)_
    - Value type: &lt;`URL`&gt;
    - Default value: `none`; 
    - Animatable: `yes`

- `lengthAdjust` - Where length adjustment should be applied to the text: the space between glyphs, or both the space and the glyphs themselves. _(`3`)_
   - Value type: `spacing` | `spacing` | `Glyphs`; 
   - Default value: `spacing`; 
   - Animatable: `yes`

- `method` - Which method to render individual glyphs along the path. _(`3`)_
   - Value type: `align` | `stretch`;
   - Default value: `align`;
   - Animatable: `yes`

- `path` - The path on which the text should be rendered. _(`3`)_
  -  Value type: &lt;`path_data`&gt; ;
  -  Default value: `none`;
  -  Animatable: `yes`

- `side` - Which side of the path the text should be rendered. _(`3`)_
  - Value type: `left` | `right`;
  - Default value: `left`;
  - Animatable: `yes`

- `spacing` - How space between glyphs should be handled. _(`3`)_
  - Value type: `auto` | `exact`; 
  - Default value: `exact`;
  - Animatable: `yes`

- `startOffset` - How far the beginning of the text should be offset from the beginning of the path. _(`3`)_
  - Value type: &lt;`length`&gt; | &lt;`percentage`&gt; &lt;`number`&gt;;
  - Default value: `0`;
  - Animatable: `yes`

- `textLength` - The width of the space into which the text will render. _(`3`)_
   - Value type: &lt;`length`&gt; | &lt;`percentage`&gt; | &lt;`number`&gt;; 
   - Default value: `auto`;
   - Animatable: `yes` 
```html
<svg viewBox="0 0 100 100" xmlns="http://www.w3.org/2000/svg">

  <!-- to hide the path, it is usually wrapped in a <defs> element -->
  <!-- <defs> -->
  <path id="MyPath" fill="none" stroke="red"
        d="M10,90 Q90,90 90,45 Q90,10 50,10 Q10,10 10,40 Q10,70 45,70 Q70,70 75,50" />
  <!-- </defs> -->

  <text>
    <textPath href="#MyPath">
      Quick brown fox jumps over the lazy dog.
    </textPath>
  </text>

</svg>
```

### HTML Canvas
`CANVAS` – The canvas rendering context provides two methods to render text. _(`2`)_

`fillText` – draws a text string at the specified, filling the string’s characters with the current fillStyle. _(`2`)_
```javascript
function draw() {
  var ctx = document.getElementById('canvas').getContext('2d');
  ctx.font = '48px serif';
  ctx.fillText('Hello world', 10, 50);
}
```

`strokeText` – Draws the outlines of – the characters of a text string at the specified coordinates. _(`2`)_
```javascript
function draw() {
  var ctx = document.getElementById('canvas').getContext('2d');
  ctx.font = '48px serif';
  ctx.strokeText('Hello world', 10, 50);
}
```

  #### Styling Text
-	`Font` - specifies the current text style to use when drawing text. This string uses the same syntax as the CSS font property. The default font is 10px sans-serif.  
*Loading fonts with the CSS Font Loading API* - help of the FontFace API, you can explicitly load fonts before using them in a canvas. _(`2`)_
```javascript
ctx.font = value;
```

-	`textAlign` - specifies the current text alignment used when drawing text. _(`2`)_
```javascript
ctx.textAlign = "left" || "right" || "center" || "start" || "end";
```

-	`textBaseline` - specifies the current text baseline used when drawing text.
    - `top` - The text baseline is the top of the em square.
    - `hanging` - The text baseline is the hanging baseline.
    - `middle` - The text baseline is the middle of the em square.
    - `alphabetic` - The text baseline is the normal alphabetic baseline. Default value.
    - `ideographic` - The text baseline is the ideographic baseline; this is the bottom of the body of the characters, if the main body of characters protrudes beneath the alphabetic baseline.
    - `bottom` - The text baseline is the bottom of the bounding box. This differs from the ideographic baseline in that the ideographic baseline doesn't consider descenders. 
```javascript
ctx.textBaseline = "top" || "hanging" || "middle" || "alphabetic" || "ideographic" || "bottom";
```

-	`direction` (*Experimental*) - specifies the current text direction used to draw text. _(`2`)_
    - `ltr` - The text direction is left-to-right.
    - `rtl` - The text direction is right-to-left.
    - `inherit` - The text direction is inherited from the &lt;canvas&gt; element or the Document as appropriate. Default value. 
```javascript
ctx.direction = "ltr" || "rtl" || "inherit";
```

`measureText` – Returns a TextMetrics object containing the width, in pixels, that the specified text will be when drawn in the current text style. (read only) _(`2`)_
```javascript
function draw() {
  var ctx = document.getElementById('canvas').getContext('2d');
  var text = ctx.measureText('foo'); // TextMetrics object
  text.width; // 16;
}
```

## Source
[Beginning Graphic Design: Typography](https://edu.gcfglobal.org/en/beginning-graphic-design/typography/1/ ), GCF LearnFree.org _(`1`)_

[Canvas Tutorial](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial), MDN Web Docs _(`2`)_

[SVG Tutorial](https://developer.mozilla.org/en-US/docs/Web/SVG/Tutorial), MDN Web Docs _(`3`)_

[Typography Essentials, 100 Design Principles for Working with Type](https://www.goodreads.com/book/show/6832833-typography-essentials), Ina Saltz _(`4`)_

[Typography Tutorial for Beginner: Everything You Need to Learn Typography Basics](https://blog.hubspot.com/marketing/typography-terms-introduction), Britany Leaning @bleaning _(`5`)_

[Web Typography](http://smad.jmu.edu/shen/webtype/baseline.html), Yvette Shen 2012 _(`6`)_