# Class 07 (22/11/2023)

## Fonts

- import { Font_name, Fontname } from "next/font/google";

- Fonts need to be assigned to a variable to be used.

```
const fontName = fontName({
    weight:["400", "700"],
    subsets:["latin"],
    })

```

- A variable font is made to contain all font weights, so it is not necessary to import the weight we will use.

## Image

- import Image from "next/image"

- By using the Image component instead of the img tag, the website will reserve that space for the actual image and display said image once it's loaded.

- width and height have to match the image ratio, so it can resize images depending on screen size.
