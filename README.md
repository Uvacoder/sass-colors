<p align="center">
  <a href="https://github.com/yonicb/sass-colors" target="blank"><img src="https://i.ibb.co/b596wMs/sass-colors.png" width="120" alt="Sass-colors Logo" /></a>
</p>

<p align="center">
🎨 Sass-colors 🌐 is a scss library, which adds modern colors.
</p>
<p align="center" style="max-width: 450px; margin: auto;">
<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
   <a href="https://github.com/yonicb/sass-colors" title="All Contributors"><img src="https://img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square" /></a>
<!-- ALL-CONTRIBUTORS-BADGE:END -->
   <a href="https://github.com/yonicb/sass-colors"><img src="https://img.shields.io/spiget/stars/1000?color=brightgreen&label=Star&logo=github" /></a>
   <a href="https://www.npmjs.com/sass-colors" target="_blank">
   <img src="https://img.shields.io/npm/v/sass-colors" alt="NPM Version" /></a>
   <a href="https://www.npmjs.com/sass-colors" target="_blank">
   <img src="https://img.shields.io/npm/l/sass-colors" alt="Package License" /></a>
   <a href="https://www.npmjs.com/sass-colors" target="_blank">
   <img src="https://img.shields.io/npm/dm/sass-colors" alt="NPM Downloads" /></a>
   <a href="https://github.com/yonicb/sass-colors" target="_blank">
   <img src="https://s3.amazonaws.com/assets.coveralls.io/badges/coveralls_95.svg" alt="Coverage" /></a>
   <a href="https://github.com/yonicb/sass-colors"><img src="https://img.shields.io/badge/Github%20Page-sass.colors-yellow?style=flat-square&logo=github" /></a>
   <a href="https://github.com/yonicb"><img src="https://img.shields.io/badge/Author-Yoni%20Calsin-blueviolet?style=flat-square&logo=appveyor" /></a>
   <a href="https://twitter.com/yonicalsin" target="_blank">
   <img src="https://img.shields.io/twitter/follow/yonicalsin.svg?style=social&label=Follow"></a>
</p>

- 🔨 [Demo](#-demo)
- 📘 [Documentation](#-documentation)
- 💬 [Description](#-description)
- 🐦 [Installation](#-installation)
- ▶️ [Getting started](#%EF%B8%8F-getting-started)
- 🎨 [Colors](#-colors)
  - 🏮 [Deep Red](#-deep-red-colors)
  - 🔴 [Red](#-red-colors)
  - 🎀 [Pink](#-pink-colors)
  - 💜 [Purple](#-purple-colors)
  - ☂️ [Deep Purple](#-deep-purple-colors)
  - 🎨 [Indigo](#-indigo-colors)
  - 📘 [Blue](#-blue-colors)
  - 🔵 [Light Blue](#-light-blue-colors)
  - 🎨 [Cyan](#-cyan-colors)
  - 🎨 [Teal](#-teal-colors)
  - 💚 [Green](#-green-colors)
  - 🍏 [Light Green](#-light-green-colors)
  - 🍈 [Lime](#-lime-colors)
  - 💛 [Yellow](#-yellow-colors)
  - 🎨 [Amber](#-amber-colors)
  - 📙 [Orange](#-orange-colors)
  - 🧡 [Deep Orange](#-deep-orange-colors)
  - 🤝🏾 [Brown](#-brown-colors)
  - 🎨 [Blue Grey](#-blue-grey-colors)
  - 🎨 [Grey](#-grey-colors)
  - ⚫ [Black](#-shades-colors)
  - ⚪ [White](#-shades-colors)
  - 🎨 [Transparent](#-shades-colors)
  
## 🎉 Demo
<p>
Preview live <a href="https://yonicb.github.io/sass-colors/" target="_blank">Click Here</a>
</p>

### 📚 Documentation
<p>
Go to documentation <a href="https://yonicb.github.io/sass-colors/" target="_blank">Click Here</a>
</p>

## 🌐 Description

<p>
Under the hood, sass-colors uses scss/sass, but also provides compatibility with a wide range of other libraries, such as Eg ReactJs, Vuejs, Angular, which allows easy use of the countless third-party add-ons that are available!
</p>


## 📦 Installation
<p>
To start using Sass-colors you need to install it with the package manager npm or yarn, as shown in the next section or download it directly!
</p>

``` ts
// To install using npm
npm install sass-colors -S

// To install using yarn
yarn add sass-colors
```

## ▶️ Getting started
<p>
To use the beautiful colors of sass-colors is very simple, first we will import the colors.scss file that contains the colors. Example:
</p>

```scss
// If you use nodejs, reactjs, vuejs or angular
@import "node_modules/sass-colors/src/colors.scss";

// You can also download it directly and import the file colors.scss, as follows
@import "src/colors.scss";

// usage: color("name_of_color", "type_of_color")
// to avoid to repeating map-get($colors, ...)
```
<p>
As you can see we already import correctly!
Sass-Colors includes a function that adds selection a color and its secondary color, for example:
</p>

```scss
@import "src/colors.scss";

body {
  // First parameter receives the name of the main color, and as a second parameter requires the name of the secondary color

  // usage: color("name_of_color", "type_of_color")
  // to avoid to repeating map-get($colors, ...)
  background: color("red", "base");
}
.button {
  background: color("blue", "accent-1");
  color: white;
  border: 1px solid color("blue", "darken-1");
}
```

```scss
// I will explain more clearly!
// First we import this color map for this example.

/**
| Main Color | Color value |
**/
$deep-red: (
  "base":       #e51c23,
  "lighten-5":  #fdeaeb,
  "lighten-4":  #f8c1c3,
  "lighten-3":  #f3989b,
  "lighten-2":  #ee6e73,
  "lighten-1":  #ea454b,
  "darken-1":   #d0181e,
  "darken-2":   #b9151b,
  "darken-3":   #a21318,
  "darken-4":   #8b1014,
);
// When you execute the function that requires two parameters
/**
color($primary-color, $secondary-color)
**/

```

## 🎨 Colors

| N° | Name        | Lighten | Darken | Accent |
|----|-------------|---------|--------|--------|
| 1  | deep-red    | ✔️       | ✔️      | ❌      |
| 2  | red         | ✔️       | ✔️      | ✔️      |
| 3  | pink        | ✔️       | ✔️      | ✔️      |
| 4  | purple      | ✔️       | ✔️      | ✔️      |
| 5  | deep-purple | ✔️       | ✔️      | ✔️      |
| 6  | indigo      | ✔️       | ✔️      | ✔️      |
| 7  | blue        | ✔️       | ✔️      | ✔️      |
| 8  | light-blue  | ✔️       | ✔️      | ✔️      |
| 9  | cyan        | ✔️       | ✔️      | ✔️      |
| 10 | teal        | ✔️       | ✔️      | ✔️      |
| 11 | green       | ✔️       | ✔️      | ✔️      |
| 12 | light-green | ✔️       | ✔️      | ✔️      |
| 13 | lime        | ✔️       | ✔️      | ✔️      |
| 15 | yellow      | ✔️       | ✔️      | ✔️      |
| 16 | amber       | ✔️       | ✔️      | ✔️      |
| 17 | orange      | ✔️       | ✔️      | ✔️      |
| 18 | deep-orange | ✔️       | ✔️      | ✔️      |
| 19 | brown       | ✔️       | ✔️      | ❌      |
| 20 | blue-grey   | ✔️       | ✔️      | ❌      |
| 21 | grey        | ✔️       | ✔️      | ❌      |

## 🎨 Shades

| N° | Name        | Ligthen | Darken | Accent |
|----|-------------|---------|--------|--------|
| 22 | black       | ❌       | ❌      | ❌      |
| 23 | white       | ❌       | ❌      | ❌      |
| 24 | transparent | ❌       | ❌      | ❌      |



### 🏮 Deep Red Colors
<details>
  <summary>Show Deep Red Colors </summary>

  ```scss
  /**
  *  Deep Red Colors
  **/
  $deep-red: (
    "base":       #e51c23,
    "lighten-5":  #fdeaeb,
    "lighten-4":  #f8c1c3,
    "lighten-3":  #f3989b,
    "lighten-2":  #ee6e73,
    "lighten-1":  #ea454b,
    "darken-1":   #d0181e,
    "darken-2":   #b9151b,
    "darken-3":   #a21318,
    "darken-4":   #8b1014,
  );
  ```
</details>

### 🔴 Red Colors
<details>
  <summary>Show Red Colors</summary>
  

```scss
/**
*  Red Colors
**/
$red: (
  "base":       #F44336,
  "lighten-5":  #FFEBEE,
  "lighten-4":  #FFCDD2,
  "lighten-3":  #EF9A9A,
  "lighten-2":  #E57373,
  "lighten-1":  #EF5350,
  "darken-1":   #E53935,
  "darken-2":   #D32F2F,
  "darken-3":   #C62828,
  "darken-4":   #B71C1C,
  "accent-1":    #FF8A80,
  "accent-2":    #FF5252,
  "accent-3":    #FF1744,
  "accent-4":    #D50000
);
```
</details>


### 🎀 Pink Colors
<details>
  <summary>Show Pink Colors</summary>

Example:
```scss
/**
*  Pink Colors
**/
$pink: (
  "base":       #e91e63,
  "lighten-5":  #fce4ec,
  "lighten-4":  #f8bbd0,
  "lighten-3":  #f48fb1,
  "lighten-2":  #f06292,
  "lighten-1":  #ec407a,
  "darken-1":   #d81b60,
  "darken-2":   #c2185b,
  "darken-3":   #ad1457,
  "darken-4":   #880e4f,
  "accent-1":    #ff80ab,
  "accent-2":    #ff4081,
  "accent-3":    #f50057,
  "accent-4":    #c51162
);
```
  
</details>




### 💜 Purple Colors
<details>
  <summary>Show Purple Colors</summary>

Example:
```scss
/**
*  Purple Colors
**/
$purple: (
  "base":       #9c27b0,
  "lighten-5":  #f3e5f5,
  "lighten-4":  #e1bee7,
  "lighten-3":  #ce93d8,
  "lighten-2":  #ba68c8,
  "lighten-1":  #ab47bc,
  "darken-1":   #8e24aa,
  "darken-2":   #7b1fa2,
  "darken-3":   #6a1b9a,
  "darken-4":   #4a148c,
  "accent-1":    #ea80fc,
  "accent-2":    #e040fb,
  "accent-3":    #d500f9,
  "accent-4":    #aa00ff
);
```
  
</details>

### 🎨 Deep Purple Colors
<details>
  <summary>Show Deep Purple Colors</summary>

Example:
```scss
/**
*  Deep Purple Colors
**/
$deep-purple: (
  "base":       #673ab7,
  "lighten-5":  #ede7f6,
  "lighten-4":  #d1c4e9,
  "lighten-3":  #b39ddb,
  "lighten-2":  #9575cd,
  "lighten-1":  #7e57c2,
  "darken-1":   #5e35b1,
  "darken-2":   #512da8,
  "darken-3":   #4527a0,
  "darken-4":   #311b92,
  "accent-1":    #b388ff,
  "accent-2":    #7c4dff,
  "accent-3":    #651fff,
  "accent-4":    #6200ea
);
```
  
</details>


### 🎨 Indigo Colors
<details>
  <summary>Show Indigo Colors</summary>

Example:
```scss
/**
*  Indigo Colors
**/
$indigo: (
  "base":       #3f51b5,
  "lighten-5":  #e8eaf6,
  "lighten-4":  #c5cae9,
  "lighten-3":  #9fa8da,
  "lighten-2":  #7986cb,
  "lighten-1":  #5c6bc0,
  "darken-1":   #3949ab,
  "darken-2":   #303f9f,
  "darken-3":   #283593,
  "darken-4":   #1a237e,
  "accent-1":    #8c9eff,
  "accent-2":    #536dfe,
  "accent-3":    #3d5afe,
  "accent-4":    #304ffe
);
```
  
</details>

### 📘 Blue Colors
<details>
  <summary>Show Blue Colors</summary>


Example:
```scss
/**
*  Blue Colors
**/
$blue: (
  "base":       #2196F3,
  "lighten-5":  #E3F2FD,
  "lighten-4":  #BBDEFB,
  "lighten-3":  #90CAF9,
  "lighten-2":  #64B5F6,
  "lighten-1":  #42A5F5,
  "darken-1":   #1E88E5,
  "darken-2":   #1976D2,
  "darken-3":   #1565C0,
  "darken-4":   #0D47A1,
  "accent-1":    #82B1FF,
  "accent-2":    #448AFF,
  "accent-3":    #2979FF,
  "accent-4":    #2962FF
);
```
</details>


### 🔵 Light Blue Colors
<details>
  <summary>Show Light Blue Colors</summary>

Example:
```scss
/**
*  Light Blue Colors
**/
$light-blue: (
  "base":       #03a9f4,
  "lighten-5":  #e1f5fe,
  "lighten-4":  #b3e5fc,
  "lighten-3":  #81d4fa,
  "lighten-2":  #4fc3f7,
  "lighten-1":  #29b6f6,
  "darken-1":   #039be5,
  "darken-2":   #0288d1,
  "darken-3":   #0277bd,
  "darken-4":   #01579b,
  "accent-1":    #80d8ff,
  "accent-2":    #40c4ff,
  "accent-3":    #00b0ff,
  "accent-4":    #0091ea
);
```
  
</details>

### 🎨 Cyan Colors
<details>
  <summary>Show Cyan Colors</summary>

Example:
```scss
/**
*  Cyan Colors
**/
$cyan: (
  "base":       #00bcd4,
  "lighten-5":  #e0f7fa,
  "lighten-4":  #b2ebf2,
  "lighten-3":  #80deea,
  "lighten-2":  #4dd0e1,
  "lighten-1":  #26c6da,
  "darken-1":   #00acc1,
  "darken-2":   #0097a7,
  "darken-3":   #00838f,
  "darken-4":   #006064,
  "accent-1":    #84ffff,
  "accent-2":    #18ffff,
  "accent-3":    #00e5ff,
  "accent-4":    #00b8d4
);
```
  
</details>




### 🎨 Teal Colors
<details>
  <summary>Show Teal Colors</summary>

Example:
```scss
/**
*  Teal Colors
**/
$teal: (
  "base":       #009688,
  "lighten-5":  #e0f2f1,
  "lighten-4":  #b2dfdb,
  "lighten-3":  #80cbc4,
  "lighten-2":  #4db6ac,
  "lighten-1":  #26a69a,
  "darken-1":   #00897b,
  "darken-2":   #00796b,
  "darken-3":   #00695c,
  "darken-4":   #004d40,
  "accent-1":    #a7ffeb,
  "accent-2":    #64ffda,
  "accent-3":    #1de9b6,
  "accent-4":    #00bfa5
);
```
</details>

### 💚 Green Colors
<details>
  <summary>Show Green Colors</summary>

Example:
```scss
/**
*  Green Colors
**/
$green: (
  "base":       #4CAF50,
  "lighten-5":  #E8F5E9,
  "lighten-4":  #C8E6C9,
  "lighten-3":  #A5D6A7,
  "lighten-2":  #81C784,
  "lighten-1":  #66BB6A,
  "darken-1":   #43A047,
  "darken-2":   #388E3C,
  "darken-3":   #2E7D32,
  "darken-4":   #1B5E20,
  "accent-1":    #B9F6CA,
  "accent-2":    #69F0AE,
  "accent-3":    #00E676,
  "accent-4":    #00C853
);
```
</details>

### 🍏 Light Green Colors
<details>
  <summary>Show Light Green Colors</summary>

Example:
```scss
/**
*  Light Green Colors
**/
$light-green: (
  "base":       #8bc34a,
  "lighten-5":  #f1f8e9,
  "lighten-4":  #dcedc8,
  "lighten-3":  #c5e1a5,
  "lighten-2":  #aed581,
  "lighten-1":  #9ccc65,
  "darken-1":   #7cb342,
  "darken-2":   #689f38,
  "darken-3":   #558b2f,
  "darken-4":   #33691e,
  "accent-1":    #ccff90,
  "accent-2":    #b2ff59,
  "accent-3":    #76ff03,
  "accent-4":    #64dd17
);
```
  
</details>

### 🍈 Lime Colors
<details>
  <summary>Show Lime Colors</summary>

Example:
```scss
/**
*  Lime Colors
**/
$lime: (
  "base":       #cddc39,
  "lighten-5":  #f9fbe7,
  "lighten-4":  #f0f4c3,
  "lighten-3":  #e6ee9c,
  "lighten-2":  #dce775,
  "lighten-1":  #d4e157,
  "darken-1":   #c0ca33,
  "darken-2":   #afb42b,
  "darken-3":   #9e9d24,
  "darken-4":   #827717,
  "accent-1":    #f4ff81,
  "accent-2":    #eeff41,
  "accent-3":    #c6ff00,
  "accent-4":    #aeea00
);
```
  
</details>


### 💛 Yellow Colors
<details>
  <summary>Show Yellow Colors</summary>

Example:
```scss
/**
*  Yellow Colors
**/
$yellow: (
  "base":       #ffeb3b,
  "lighten-5":  #fffde7,
  "lighten-4":  #fff9c4,
  "lighten-3":  #fff59d,
  "lighten-2":  #fff176,
  "lighten-1":  #ffee58,
  "darken-1":   #fdd835,
  "darken-2":   #fbc02d,
  "darken-3":   #f9a825,
  "darken-4":   #f57f17,
  "accent-1":    #ffff8d,
  "accent-2":    #ffff00,
  "accent-3":    #ffea00,
  "accent-4":    #ffd600
);
```

  
</details>

### 🎨 Amber Colors
<details>
  <summary>Show Amber Colors</summary>

Example:
```scss
/**
*  Amber Colors
**/
$amber: (
  "base":       #ffc107,
  "lighten-5":  #fff8e1,
  "lighten-4":  #ffecb3,
  "lighten-3":  #ffe082,
  "lighten-2":  #ffd54f,
  "lighten-1":  #ffca28,
  "darken-1":   #ffb300,
  "darken-2":   #ffa000,
  "darken-3":   #ff8f00,
  "darken-4":   #ff6f00,
  "accent-1":    #ffe57f,
  "accent-2":    #ffd740,
  "accent-3":    #ffc400,
  "accent-4":    #ffab00
);
```
  
</details>


### 📙 Orange Colors
<details>
  <summary>Show Orange Colors</summary>
  
Example:
```scss
/**
*  Orange Colors
**/
$orange: (
  "base":       #ff9800,
  "lighten-5":  #fff3e0,
  "lighten-4":  #ffe0b2,
  "lighten-3":  #ffcc80,
  "lighten-2":  #ffb74d,
  "lighten-1":  #ffa726,
  "darken-1":   #fb8c00,
  "darken-2":   #f57c00,
  "darken-3":   #ef6c00,
  "darken-4":   #e65100,
  "accent-1":    #ffd180,
  "accent-2":    #ffab40,
  "accent-3":    #ff9100,
  "accent-4":    #ff6d00
);
```
</details>


### 🧡 Deep Orange Colors
<details>
  <summary>Show Deep Orange Colors</summary>

Example:
```scss
/**
*  Deep Orange Colors
**/
$deep-orange: (
  "base":       #ff5722,
  "lighten-5":  #fbe9e7,
  "lighten-4":  #ffccbc,
  "lighten-3":  #ffab91,
  "lighten-2":  #ff8a65,
  "lighten-1":  #ff7043,
  "darken-1":   #f4511e,
  "darken-2":   #e64a19,
  "darken-3":   #d84315,
  "darken-4":   #bf360c,
  "accent-1":    #ff9e80,
  "accent-2":    #ff6e40,
  "accent-3":    #ff3d00,
  "accent-4":    #dd2c00
);
```
</details>


### 🤝🏾 Brown Colors
<details>
  <summary>Show Brown Colors</summary>

Example:
```scss
/**
*  Brown Colors
**/
$brown: (
  "base":       #795548,
  "lighten-5":  #efebe9,
  "lighten-4":  #d7ccc8,
  "lighten-3":  #bcaaa4,
  "lighten-2":  #a1887f,
  "lighten-1":  #8d6e63,
  "darken-1":   #6d4c41,
  "darken-2":   #5d4037,
  "darken-3":   #4e342e,
  "darken-4":   #3e2723
);
```
</details>

### 🎨 Blue Grey Colors
<details>
  <summary>Show Blue Grey Colors</summary>

Example:
```scss
/**
*  Blue Grey Colors
**/
$blue-grey: (
  "base":       #607d8b,
  "lighten-5":  #eceff1,
  "lighten-4":  #cfd8dc,
  "lighten-3":  #b0bec5,
  "lighten-2":  #90a4ae,
  "lighten-1":  #78909c,
  "darken-1":   #546e7a,
  "darken-2":   #455a64,
  "darken-3":   #37474f,
  "darken-4":   #263238
);
```
</details>


### 🎨 Grey Colors
<details>
  <summary>Show Grey Colors</summary>

Example:
```scss
/**
*  Grey Colors
**/
$grey: (
  "base":       #9e9e9e,
  "lighten-5":  #fafafa,
  "lighten-4":  #f5f5f5,
  "lighten-3":  #eeeeee,
  "lighten-2":  #e0e0e0,
  "lighten-1":  #bdbdbd,
  "darken-1":   #757575,
  "darken-2":   #616161,
  "darken-3":   #424242,
  "darken-4":   #212121
);
```
</details>


### 🎨 Shades Colors
<details>
  <summary>Show Shades Colors</summary>

Example:
```scss
/**
*  Shades Colors
**/
$shades: (
  "black":        #000000,
  "white":        #FFFFFF,
  "transparent":  transparent
);
```
</details>



## ⭐ Support for

Sass-colors is an open source project licensed by [MIT](LICENSE). You can grow thanks to the sponsors and the support of the amazing sponsors. If you want to join them, [contact me here](mailto:helloyonicb@gmail.com).


## 🎩 Stay in touch

* Author [Yoni Calsin](https://github.com/yonicb)
* Twitter [Yoni Calsin](https://twitter.com/yonicalsin)

## Contributors ✨

Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tr>
    <td align="center"><a href="https://twitter.com/yonicalsin"><img src="https://avatars0.githubusercontent.com/u/58490737?v=4" width="70px;" alt=""/><br /><sub><b>Yoni Calsin</b></sub></a><br /><a href="https://github.com/sass-colors/sass-colors/commits?author=yonicb" title="Code">💻</a> <a href="https://github.com/sass-colors/sass-colors/issues?q=author%3Ayonicb" title="Bug reports">🐛</a> <a href="https://github.com/sass-colors/sass-colors/commits?author=yonicb" title="Documentation">📖</a> <a href="#blog-yonicb" title="Blogposts">📝</a></td>
  </tr>
</table>

<!-- markdownlint-enable -->
<!-- prettier-ignore-end -->
<!-- ALL-CONTRIBUTORS-LIST:END -->

This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!

## 📜 License

Sass-colors is [MIT licensed](LICENSE).