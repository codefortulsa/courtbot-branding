# CourtBot Branding and Style Guidelines

This repository contains the files for CourtBot branding. I don't want to get all corporate command-and-control, so I'm going for a minimalist approach to allow for design freedom.

Most of the files are InkScape/Scribus, due to issues with exporting CYMK color spaces from InkScape. (See http://libregraphicsworld.org/blog/entry/getting-cmyk-colors-from-inkscape-to-scribus for more details.)

References to Code for America style guidelines can be resolved at https://style.codeforamerica.org/

## Print (CMYK)

### Reminders

Please remember to include links to CfA and Techlahoma (and logos if space permits).

### Sizing

The flyer is 9" x 11.5" overall w/ 0.25" bleeds.

The business card is double-sided 3.75" x 2.25" overall w/ 0.125" bleeds.

### Logo

* CourtBot Logo Text: C5 M5 Y5 K95
* CourtBot Outline: C5 M5 Y5 K95
* CourtBot Background Color: C4 M2 Y16 K0
* CourtBot Lighter Background Color: C2 M1 Y8 K0
* CourtBot Body Gold: C0 M11 Y73 K0
* CourtBot Body Shadow: C0 M70 Y61 K25

### Fonts

* Baseline Grid: 9.375pt (125% of 15pt, then halved for additional vertical rhythm control)
* Default Paragraph: 15pt Gotham Book w/ 18.75pt after-paragraph spacing. CfA Gray.
* Default Paragraph Italic/Emphasis: 15pt Gotham Book. CfA Blue.
* Default Paragraph Strong/Bold: 18pt Gotham Bold, small caps. CfA Dark Blue.   
* Header: 22pt Gotham Bold w/ 18.75pt after-paragraph spacing, small caps. CfA Blue.
* Header Strong/Bold: 22pt Gotham Bold, small caps. CfA Dark Blue.

## Web (RGB)

### Reminders

Please remember to include links to CfA and Techlahoma (and logos if space permits).

### Logo

* CourtBot Logo Text: #000 (black)
* CourtBot Outline: #000 (black)
* CourtBot Background Color: #fcfbe3
* CourtBot Body Gold: #ffdf53
* CourtBot Body Shadow: #b5571f

### Fonts (In Progress)

    html {
    font-size: 100%; /* 16px */
	    line-height: 1.25em; /* calculated baseline grid is half this, set to 0.625rem */
	    font-family: 'Gotham Book', Helvetica, sans-serif;
    }

    p {
	    margin-top: 1.25rem;
	    color: $color-gray; /* #6D6E71 */
    }

    em, i {
	    color: $color-blue; /* #399fd3 */
    }

    strong, b {
	    font-weight: bold;
	    font-size: 1.2rem;
	    font-variant: small-caps;
	    color: $color-dark-blue; /* #004b6a */
    }

    h1 {
	    font-size: 1.5rem;
	    font-weight: bold;
	    margin-top: 1rem ; /* margin-top and margin-bottom collapse into each other, so making up baseline grid proportions here: 3 * .625rem = 1.875rem - 1.5rem(text height) = 0.375rem + .625rem = 1 rem */
	    font-variant: small-caps;
	    color: $color-blue; /* #399fd3 */
    }

    h1 strong, h1 b {
	    color: $color-dark-blue; /* #004b6a */
    }

## Todo

- [ ] Create CMYK colorspace SVGs for remainder of CourtBot assets (Currently they're embedded in the Scribus files)
- [ ] Test SCSS styles for CourtBot branded websites
