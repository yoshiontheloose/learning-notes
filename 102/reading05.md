# Understanding CSS
> _WHAT'S IN THE BOX!?!_ 

## Chapter 10
CSS allows you to create rules about each box and how it's contents are presented

HTML elements have rules that contain two parts

* **Selector**  -indicates which element the rule applies to
* **Declaration** - indicates how the elements in the selector should be styled
    - inside curly brackets
    - Made with a _property_ and a _value_ 
        * **Property** - part of the element to be changed
        * **Value** - a setting for the property
        * {property: value}  EX: {color: yellow;}

External  \<link>
    - href
    - type
    - rel

Internal \<style>
    - inside of the \<head> element

# Chapter 11 _Color_

RGB values range from 0-255 

Hex codes - values for red, green, and blue in hexadcimal code 

Color names - only 147 colors supported by browsers. Not commonly used.

Hue | Saturation | Lightness/luminosity
--- | --- | ---
color circle or slider values from 0-360 | Percentage | Percentage 0-black 100-white

RGBA - A stands for alpha
    * ability to change opacity

hsl, hsla - newer way to specify colors
* hsl - Hue Saturation Lightness 
    - EX: hsl(0,100%,100%)
* hsla - Hue Saturation Lightness Transparency
    - a number between 0 and 1.0
    - EX: hsla(0,100%,100%,0.5)   

-------
**Block level element takes up as much space as it can**

**Inline element only takes up necessary space**

[Types of both](https://www.w3schools.com/html/html_blocks.asp)

[<<<Back](README.md)