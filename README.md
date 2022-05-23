# List of countries and their flags
Json file that contains the list of all countries in the world with their flags and their 2 digit codes (ISO 3166-1) using Emoji CSS.

```
<link href="https://emoji-css.afeld.me/emoji.css" rel="stylesheet">
```


## Installation

To install it in your project, you can use the CDN version of [Emoji CSS library](https://emoji-css.afeld.me/), or you can download the Emoji CSS file and insert it directly in your project (the CSS file is available in this repository).

## Usage

### Usage with Loop

For example, you can browse the Json file with a loop and display all the countries and their flags as follows (in the following example I use VueJs to display the list of all countries):

```
<div v-for='item in CountriesList'>
    <i :class="['em', item.flag]"></i> {{item.Name}} {{item.Code}}
</div>
```

### Usage for a single flag

Or you can insert a single flag as follows: 

```
<i class="em em-flag-dz" aria-role="presentation" aria-label="Algeria Flag"></i>
```