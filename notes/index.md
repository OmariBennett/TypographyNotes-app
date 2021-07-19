# Typography Notes
`Typography`
- – style or appearance of text,
- – the art of working with text.

## Terminology
### The Anatomy of a Typeface
`Ascender` - The portion of a letter that extends above the mean line of a font -- i.e., is taller than the font's x-height. (In this case, you will also notice the letter ‘h’ is taller than the x-height.)

`Baseline` - The line where the letters sit.

`Bowl` - The curved part of the character that encloses the circular or curved parts of some letters, like ‘d’, ‘b’, ‘o’, ‘d’, and ‘b’. (In the case, it is that round shape sticking off the letter ‘a’.)

`Cap height` - The distance from the baseline to the top of the capital letter.

`Cross` bar - The bar that goes across the inside of the letter and connects one side to another. (In this case, it is the bar inside the capital letter 'B’.)

`Counter` - The empty space in the middle of letters such as ‘B’, ‘O’, or ‘A’.

`Descender` - The longest point on a letter that falls beyond the baseline.

`Finial` - The tapered end of letters such as ‘e’ or ‘c’.

`Hierarchy` – is used to guide the reader’s eye to whatever is most important. In other words, it shows them where to begin and where to go next using different levels of emphasis.

`Kerning` – is the space between specific characters. *Some fonts have what we call bad kerning, making certain letters look improperly spaced. If a font you are using has bad kerning, it is best to cut your losses and choose something else.

`Leading` – is the space between lines of text, also known as line spacing.

`Ligature` - The stroke that joins adjacent letters.

`Serif` - The slight projection finishing off a stroke of a letter in certain typefaces. (In this case, it is that little foot sticking off the letter ‘l’.)

`Spine` - The curvy body of the letter 's' -- and only the letter ’s’. It gets its own term because the spine can be almost vertical or mostly horizontal, depending on the typeface.

`Stem` - The base of a letter, like the stem of a flower.

`Tracking` – is the overall space between characters, sometimes called character spacing.

`Terminal` - A type of curve that you see at the top of the letter ‘f’ or the end of the letter ‘j’.

`X-height` - Located in between the baseline and the cap height, it is the height of the body of the lowercase letter. (In this case, it is the letters ‘a’, ’u’, and ‘y’.)

### Common Font Classification Types
`Type Families` - “type family” or “typeface family” is used to describe a range of designs that are all variations of one basic typeface.

`Display` – Because of their decorative nature, display fonts are best for small amounts of text; for example, title and herders, and more graphic-heavy designs.
-	Script
-	Blackletter
-	All-caps
-	Plain Fancy
- _*_ When deciding which fonts to use, less is more. It is best to limit yourself to one or two per project. If you need more contrast, try repeating one of your fonts in a different size, weight, or style.

`San serif` – fonts do not have that extra stroke-hence the name, which is French for “without serif”. _*_ This style is considered cleaner and more modern than serif fonts. Also, it tends to be easier to read on computer screens, including smartphones and tablets.

`Serif` – fonts have little strokes called serifs attached to the main part of the letter. _*_ Because of their classic look, they are a good choice for more traditional projects. They are also common in print publications, like magazines and newspapers.

## Typography Essentials
`Using letter as form` – Each letter is a shape unto itself, a shape that may serve as an illustration, as an icon, as a vessel, or as a graphic focal point, apart from its meaning as an alphabetic unit.

`Using counter spaces as form` – The space inside and around the shape of a letter, called counter spaces, are often overlooked as design elements. *Their shapes can be customized using color, pattern, or texture. The beauty of counter spaces, sometimes called “negative” spaces, is that they are the jewels that are already tucked into the letters… using them well is like discovering buried treasure.

`Letterform details` – Specialized detailing can communicate apart from the literal message; whether customized or built in as alternate character within a typeface, even a simple swash or ligature can add an extra level of meaning or make the design more specific to the message.

`Emotional content implied by the text` – Letterforms can amplify the emotional weight of the text. *The delicate tracery of a flowing italic might best convey a poem about nature.

`Historical connotation` – typefaces area product of their era. A good design may be well served with a historically appropriate typeface choice when possible.

`Vertical Rhythm` – Improves readability and helps to make the layout harmonious and organized. Vertical Rhythm on the web is contributed to by font-size, line-height, and margin size.

`Combining fonts` - When deciding which fonts to use, less is more. It's best to limit yourself to one or two per project. If you need more contrast, try repeating one of your fonts in a different size, weight, or style. *You've probably heard that opposites attract.*

## Typography Code Basics Essentials
### CSS
`Kerning` – is the space between specific characters. *Some fonts have what we call bad kerning, making certain letters look improperly spaced. If a font you are using has bad kerning, it is best to cut your losses and choose something else.
```css
CSS rule { letter-spacing: 1rem; }
```

`Leading` – is the space between lines of text, also known as line spacing.
```css
CSS rule { line-height: 1.2; }
```

`Tracking` – is the overall space between characters, sometimes called character spacing.
```css
CSS rule { word-spacing: 1rem; }
```
### SVG
`SVG` - An essential part of a text is the font in which it is displayed. SVG offers a set of attributes, many like their CSS counterparts, to enable font selection.
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

`Text-Anchor` – An attribute is used to align (stat-, middle-, or end-alignment) a string of pre-formatted text or auto-wrapped text where the wrapping area is determined from the inline-size property relative to a given point.
```html
<text text-anchor="start" x="60" y="40">A</text>
```

`Dominant-Baseline` – An attribute specifies the dominant baseline, which is the baseline used to align the box’s text and inline-level contents. (auto | text-bottom | alphabetic | ideographic | middle | central | mathematical | hanging | text-top)
```html
<text dominant-baseline="auto" x="30" y="20">Auto</text>
```

`Tspan` – element has the following custom attributes.
```html
<text>
  This is <tspan font-weight="bold" fill="red">bold and red<tspan>
</text>
```
#### Attributes
- `textPath` - This element fetches via its xlink:href attribute an arbitrary path and aligns the characters, that it encircles, along this path.

- `href` - The URL to the path or basic shape on which to render the text. If the path attribute is set, href has no effect.
    Value type: <URL> ; Default value: none; Animatable: yes

- `lengthAdjust` - Where length adjustment should be applied to the text: the space between glyphs, or both the space and the glyphs themselves.
    Value type: spacing|spacingAndGlyphs; Default value: spacing; Animatable: yes

- `method` - Which method to render individual glyphs along the path.
    Value type: align|stretch ; Default value: align; Animatable: yes

- `path` - The path on which the text should be rendered.
    Value type: <path_data> ; Default value: none; Animatable: yes

- `side` - Which side of the path the text should be rendered.
    Value type: left|right ; Default value: left; Animatable: yes

- `spacing` - How space between glyphs should be handled.
    Value type: auto|exact ; Default value: exact; Animatable: yes

- `startOffset` - How far the beginning of the text should be offset from the beginning of the path.
    Value type: <length>|<percentage>|<number> ; Default value: 0; Animatable: yes

- `textLength` - The width of the space into which the text will render.
    Value type: <length>|<percentage>|<number> ; Default value: auto; Animatable: yes 
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
`CANVAS` – The canvas rendering context provides two methods to render text.

`fillText` – draws a text string at the specified, filling the string’s characters with the current fillStyle.
```javascript
function draw() {
  var ctx = document.getElementById('canvas').getContext('2d');
  ctx.font = '48px serif';
  ctx.fillText('Hello world', 10, 50);
}
```

`strokeText` – Draws the outlines of – the characters of a text string at the specified coordinates.
```javascript
function draw() {
  var ctx = document.getElementById('canvas').getContext('2d');
  ctx.font = '48px serif';
  ctx.strokeText('Hello world', 10, 50);
}
```

  #### Styling Text
-	Font
```javascript
ctx.font = value;
```
-	textAlign
```javascript
ctx.textAlign = "left" || "right" || "center" || "start" || "end";
```
-	textBaseline
```javascript
ctx.textBaseline = "top" || "hanging" || "middle" || "alphabetic" || "ideographic" || "bottom";
```
-	direction (*Experimental*)
```javascript
ctx.direction = "ltr" || "rtl" || "inherit";
```

`measureText` – Returns a TextMetrics object containing the width, in pixels, that the specified text will be when drawn in the current text style. (read only)
```javascript
function draw() {
  var ctx = document.getElementById('canvas').getContext('2d');
  var text = ctx.measureText('foo'); // TextMetrics object
  text.width; // 16;
}

```

## Source
[Beginning Graphic Design: Typography](https://edu.gcfglobal.org/en/beginning-graphic-design/typography/1/ ), GCF LearnFree.org

[Canvas Tutorial](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial), MDN Web Docs

[SVG Tutorial](https://developer.mozilla.org/en-US/docs/Web/SVG/Tutorial), MDN Web Docs

[Typography Essentials, 100 Design Principles for Working with Type](https://www.goodreads.com/book/show/6832833-typography-essentials), Ina Saltz

[Typography Tutorial for Beginner: Everything You Need to Learn Typography Basics](https://blog.hubspot.com/marketing/typography-terms-introduction), Britany Leaning @bleaning 

[Web Typography](http://smad.jmu.edu/shen/webtype/baseline.html), Yvette Shen 2012