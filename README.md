# Ex08 Event Registration Web Application
## Date:21/12/2025

## AIM:
To design, develop and deploy a web application for event registration using Figma UI tool.

## UI DESIGN TOOL:
Figma

## DESIGN STEPS:

### Step 1:
Use frames to represent screens or sections.

### Step 2:
Add column grids for consistent spacing and alignment.

### Step 3:
Insert shapes, text, buttons, and icons.

### Step 4:
Use Auto Layout for flexible, responsive design.

### Step 5:
Define color, text, and effect styles globally for consistency.

### Step 6:
Name layers logically and group related elements.

### Step 6:
Link frames to show navigation or interactions.

### Step 7:
Select the specific frame while generating code using Anima plugin.

## CODE:
```
index.html
<!DOCTYPE html>
<html>
  <head>
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <meta charset="utf-8" />
    <link rel="stylesheet" href="globals.css" />
    <link rel="stylesheet" href="styleguide.css" />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="iphone-pro-max">
      <img class="logo" src="img/logo-1.png" />
      <img class="line" src="img/line-1.svg" />
      <div class="rectangle"></div>
      <div class="text-wrapper">PONGAL CELEBRATION EVENTS</div>
      <img class="text-on-a-path" src="img/text-on-a-path.svg" />
      <div class="div"></div>
      <div class="text-wrapper-2">REGISTER</div>
      <div class="rectangle-2"></div>
      <div class="text-wrapper-3">designed by Raaghavi S</div>
      <div class="rectangle-3"></div>
      <div class="text-wrapper-4">LOGIN</div>
      <img class="pongal" src="img/pongal-1.png" />
    </div>
  </body>
</html>

globals.css
@import url("https://cdnjs.cloudflare.com/ajax/libs/meyer-reset/2.0/reset.min.css");
* {
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}
html,
body {
  margin: 0px;
  height: 100%;
}
/* a blue color as a generic focus style */
button:focus-visible {
  outline: 2px solid #4a90e2 !important;
  outline: -webkit-focus-ring-color auto 5px !important;
}
a {
  text-decoration: none;
}

style.css
.iphone-pro-max {
  overflow: hidden;
  background: linear-gradient(
    180deg,
    rgba(205, 236, 236, 1) 0%,
    rgba(165, 115, 156, 1) 100%
  );
  width: 100%;
  min-width: 563px;
  min-height: 984px;
  position: relative;
}

.iphone-pro-max .logo {
  position: absolute;
  top: 12px;
  left: 11px;
  width: 552px;
  height: 83px;
  aspect-ratio: 6.67;
  object-fit: cover;
}

.iphone-pro-max .line {
  position: absolute;
  top: 110px;
  left: 21px;
  width: 521px;
  height: 2px;
  object-fit: cover;
}

.iphone-pro-max .rectangle {
  position: absolute;
  top: 152px;
  left: 71px;
  width: 427px;
  height: 58px;
  background-color: #927ff4;
  box-shadow: 0px 4px 4px #00000040;
}

.iphone-pro-max .text-wrapper {
  position: absolute;
  top: 167px;
  left: 100px;
  text-shadow: 0px 4px 4px #00000040;
  font-family: "Inter-SemiBold Italic", Helvetica;
  font-weight: 600;
  font-style: italic;
  color: #000000;
  font-size: 24px;
  letter-spacing: 0;
  line-height: normal;
}

.iphone-pro-max .text-on-a-path {
  position: absolute;
  top: 865px;
  left: 1978px;
  width: 148px;
  height: 44px;
}

.iphone-pro-max .div {
  position: absolute;
  top: 424px;
  left: 179px;
  width: 206px;
  height: 44px;
  background-color: #ed67df;
  box-shadow: var(--drop-shadow-600);
}

.iphone-pro-max .text-wrapper-2 {
  position: absolute;
  top: 431px;
  left: 231px;
  text-shadow: 0px 4px 4px #00000040;
  font-family: "Inter-MediumItalic", Helvetica;
  font-weight: 500;
  font-style: italic;
  color: #000000;
  font-size: 24px;
  letter-spacing: 0;
  line-height: normal;
}

.iphone-pro-max .rectangle-2 {
  position: absolute;
  top: 945px;
  left: -1px;
  width: 563px;
  height: 41px;
  background-color: #3d3c76;
}

.iphone-pro-max .text-wrapper-3 {
  position: absolute;
  top: 945px;
  left: 152px;
  font-family: "Merienda-Regular", Helvetica;
  font-weight: 400;
  color: #fefcfc;
  font-size: 22px;
  letter-spacing: 0;
  line-height: normal;
}

.iphone-pro-max .rectangle-3 {
  position: absolute;
  top: 304px;
  left: 197px;
  width: 170px;
  height: 50px;
  background-color: #f46be7;
  box-shadow: 0px 4px 4px #00000040;
}

.iphone-pro-max .text-wrapper-4 {
  position: absolute;
  top: 315px;
  left: 243px;
  text-shadow: 0px 4px 4px #00000040;
  font-family: "Inter-MediumItalic", Helvetica;
  font-weight: 500;
  font-style: italic;
  color: #000000;
  font-size: 24px;
  letter-spacing: 0;
  line-height: normal;
}

.iphone-pro-max .pongal {
  position: absolute;
  top: 501px;
  left: 82px;
  width: 413px;
  height: 413px;
  aspect-ratio: 1;
  object-fit: cover;
}

index.html
<!DOCTYPE html>
<html>
  <head>
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <meta charset="utf-8" />
    <link rel="stylesheet" href="globals.css" />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="iphone-pro-max">
      <div class="ellipse"></div>
      <div class="text-wrapper">EVENTS</div>
      <div class="rectangle"></div>
      <p class="div">Musical chairs with a twist</p>
      <div class="text-wrapper-2">Pinata</div>
      <div class="text-wrapper-3">Silambam</div>
      <div class="text-wrapper-4">Sing</div>
      <div class="text-wrapper-5">Rangoli Competition</div>
      <img class="star" src="img/star-1.svg" />
      <img class="img" src="img/star-2.svg" />
      <img class="star-2" src="img/star-3.svg" />
      <img class="star-3" src="img/star-4.svg" />
      <img class="star-4" src="img/star-5.svg" />
      <img class="star-5" src="img/star-6.svg" />
      <div class="text-wrapper-6">Dance</div>
      <img class="pongal" src="img/pongal2-1.png" />
    </div>
  </body>
</html>

globals.css
@import url("https://cdnjs.cloudflare.com/ajax/libs/meyer-reset/2.0/reset.min.css");
* {
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}
html,
body {
  margin: 0px;
  height: 100%;
}
/* a blue color as a generic focus style */
button:focus-visible {
  outline: 2px solid #4a90e2 !important;
  outline: -webkit-focus-ring-color auto 5px !important;
}
a {
  text-decoration: none;
}

style.css
.iphone-pro-max {
  background: linear-gradient(
    180deg,
    rgba(209, 233, 241, 1) 0%,
    rgba(127, 86, 138, 1) 100%
  );
  width: 100%;
  min-width: 564px;
  min-height: 980px;
  position: relative;
}

.iphone-pro-max .ellipse {
  position: absolute;
  top: 52px;
  left: 136px;
  width: 289px;
  height: 73px;
  background-color: #ad92cd;
  border-radius: 144.5px / 36.5px;
  box-shadow: 0px 4px 4px #00000040;
}

.iphone-pro-max .text-wrapper {
  position: absolute;
  top: 72px;
  left: 218px;
  text-shadow: 0px 4px 4px #00000040;
  font-family: "Inter-SemiBold Italic", Helvetica;
  font-weight: 600;
  font-style: italic;
  color: #000000;
  font-size: 27px;
  letter-spacing: 0;
  line-height: normal;
}

.iphone-pro-max .rectangle {
  position: absolute;
  top: 162px;
  left: 55px;
  width: 455px;
  height: 766px;
  background-color: #fff8f8;
  box-shadow: 0px 4px 4px #00000040;
}

.iphone-pro-max .div {
  position: absolute;
  top: 561px;
  left: 134px;
  font-family: "Inter-MediumItalic", Helvetica;
  font-weight: 500;
  font-style: italic;
  color: #000000;
  font-size: 26px;
  letter-spacing: 0;
  line-height: normal;
  white-space: nowrap;
}

.iphone-pro-max .text-wrapper-2 {
  position: absolute;
  top: 496px;
  left: 134px;
  font-family: "Inter-MediumItalic", Helvetica;
  font-weight: 500;
  font-style: italic;
  color: #000000;
  font-size: 26px;
  letter-spacing: 0;
  line-height: normal;
  white-space: nowrap;
}

.iphone-pro-max .text-wrapper-3 {
  position: absolute;
  top: 435px;
  left: 138px;
  font-family: "Inter-MediumItalic", Helvetica;
  font-weight: 500;
  font-style: italic;
  color: #000000;
  font-size: 26px;
  letter-spacing: 0;
  line-height: normal;
  white-space: nowrap;
}

.iphone-pro-max .text-wrapper-4 {
  position: absolute;
  top: 365px;
  left: 138px;
  font-family: "Inter-MediumItalic", Helvetica;
  font-weight: 500;
  font-style: italic;
  color: #000000;
  font-size: 26px;
  letter-spacing: 0;
  line-height: normal;
  white-space: nowrap;
}

.iphone-pro-max .text-wrapper-5 {
  position: absolute;
  top: 288px;
  left: 134px;
  font-family: "Inter-MediumItalic", Helvetica;
  font-weight: 500;
  font-style: italic;
  color: #000000;
  font-size: 26px;
  letter-spacing: 0;
  line-height: normal;
  white-space: nowrap;
}

.iphone-pro-max .star {
  position: absolute;
  top: 212px;
  left: 87px;
  width: 27px;
  height: 30px;
}

.iphone-pro-max .img {
  position: absolute;
  top: 285px;
  left: 88px;
  width: 26px;
  height: 33px;
}

.iphone-pro-max .star-2 {
  position: absolute;
  top: 362px;
  left: 91px;
  width: 25px;
  height: 33px;
}

.iphone-pro-max .star-3 {
  position: absolute;
  top: 429px;
  left: 91px;
  width: 25px;
  height: 33px;
}

.iphone-pro-max .star-4 {
  position: absolute;
  top: 496px;
  left: 91px;
  width: 26px;
  height: 28px;
}

.iphone-pro-max .star-5 {
  position: absolute;
  top: 561px;
  left: 89px;
  width: 29px;
  height: 30px;
}

.iphone-pro-max .text-wrapper-6 {
  position: absolute;
  top: 214px;
  left: 138px;
  font-family: "Inter-MediumItalic", Helvetica;
  font-weight: 500;
  font-style: italic;
  color: #000000;
  font-size: 26px;
  letter-spacing: 0;
  line-height: normal;
  white-space: nowrap;
}

.iphone-pro-max .pongal {
  position: absolute;
  top: 600px;
  left: 120px;
  width: 320px;
  height: 320px;
  aspect-ratio: 1;
  object-fit: cover;
}

index.html
<!DOCTYPE html>
<html>
  <head>
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <meta charset="utf-8" />
    <link rel="stylesheet" href="globals.css" />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="iphone-pro-max">
      <div class="rectangle"></div>
      <div class="text-wrapper">EVENT REGISTRATION FORM</div>
      <div class="div"></div>
      <div class="rectangle-2"></div>
      <div class="text-wrapper-2">Email ID</div>
      <div class="rectangle-3"></div>
      <div class="text-wrapper-3">Full name</div>
      <div class="rectangle-4"></div>
      <div class="text-wrapper-4">Gender</div>
      <div class="rectangle-5"></div>
      <div class="text-wrapper-5">Age</div>
      <div class="rectangle-6"></div>
      <div class="text-wrapper-6">Register No.</div>
      <div class="rectangle-7"></div>
      <div class="text-wrapper-7">Department</div>
      <div class="rectangle-8"></div>
      <div class="text-wrapper-8">Mobile No.</div>
      <div class="rectangle-9"></div>
      <div class="text-wrapper-9">Events registered</div>
      <div class="rectangle-10"></div>
      <div class="text-wrapper-10">Submit</div>
      <img class="pongal" src="img/pongal3-1.png" />
    </div>
  </body>
</html>

globals.css
@import url("https://cdnjs.cloudflare.com/ajax/libs/meyer-reset/2.0/reset.min.css");
* {
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}
html,
body {
  margin: 0px;
  height: 100%;
}
/* a blue color as a generic focus style */
button:focus-visible {
  outline: 2px solid #4a90e2 !important;
  outline: -webkit-focus-ring-color auto 5px !important;
}
a {
  text-decoration: none;
}

style.css
.iphone-pro-max {
  background: linear-gradient(
    180deg,
    rgba(184, 224, 232, 1) 0%,
    rgba(157, 123, 180, 1) 100%
  );
  width: 100%;
  min-width: 551px;
  min-height: 980px;
  position: relative;
}

.iphone-pro-max .rectangle {
  position: absolute;
  top: 40px;
  left: 70px;
  width: 399px;
  height: 74px;
  background-color: #919deb;
  box-shadow: 0px 4px 4px #00000040;
}

.iphone-pro-max .text-wrapper {
  position: absolute;
  top: 62px;
  left: 88px;
  text-shadow: 0px 4px 4px #00000040;
  font-family: "Inter-SemiBold Italic", Helvetica;
  font-weight: 600;
  font-style: italic;
  color: #000000;
  font-size: 26px;
  letter-spacing: 0;
  line-height: normal;
  white-space: nowrap;
}

.iphone-pro-max .div {
  position: absolute;
  top: 151px;
  left: 32px;
  width: 487px;
  height: 780px;
  background-color: #fffafa;
  border: 1px solid;
  border-color: #000000;
}

.iphone-pro-max .rectangle-2 {
  position: absolute;
  top: 651px;
  left: 88px;
  width: 244px;
  height: 42px;
  background-color: #b8e0e8;
  box-shadow: 0px 4px 4px #00000040;
}

.iphone-pro-max .text-wrapper-2 {
  position: absolute;
  top: 657px;
  left: 161px;
  font-family: "Inter-MediumItalic", Helvetica;
  font-weight: 500;
  font-style: italic;
  color: #000000;
  font-size: 26px;
  letter-spacing: 0;
  line-height: normal;
  white-space: nowrap;
}

.iphone-pro-max .rectangle-3 {
  position: absolute;
  top: 177px;
  left: 88px;
  width: 244px;
  height: 49px;
  background-color: #b8e0e8;
  box-shadow: 0px 4px 4px #00000040;
}

.iphone-pro-max .text-wrapper-3 {
  position: absolute;
  top: 186px;
  left: 152px;
  font-family: "Inter-MediumItalic", Helvetica;
  font-weight: 500;
  font-style: italic;
  color: #000000;
  font-size: 26px;
  letter-spacing: 0;
  line-height: normal;
  white-space: nowrap;
}

.iphone-pro-max .rectangle-4 {
  position: absolute;
  top: 260px;
  left: 88px;
  width: 244px;
  height: 43px;
  background-color: #b8e0e8;
  box-shadow: 0px 4px 4px #00000040;
}

.iphone-pro-max .text-wrapper-4 {
  position: absolute;
  top: 266px;
  left: 165px;
  font-family: "Inter-MediumItalic", Helvetica;
  font-weight: 500;
  font-style: italic;
  color: #000000;
  font-size: 26px;
  letter-spacing: 0;
  line-height: normal;
  white-space: nowrap;
}

.iphone-pro-max .rectangle-5 {
  position: absolute;
  top: 347px;
  left: 88px;
  width: 244px;
  height: 40px;
  background-color: #b8e0e8;
  box-shadow: 0px 4px 4px #00000040;
}

.iphone-pro-max .text-wrapper-5 {
  position: absolute;
  top: 347px;
  left: 186px;
  font-family: "Inter-MediumItalic", Helvetica;
  font-weight: 500;
  font-style: italic;
  color: #000000;
  font-size: 26px;
  letter-spacing: 0;
  line-height: normal;
  white-space: nowrap;
}

.iphone-pro-max .rectangle-6 {
  position: absolute;
  top: 427px;
  left: 88px;
  width: 244px;
  height: 38px;
  background-color: #b8e0e8;
  box-shadow: 0px 4px 4px #00000040;
}

.iphone-pro-max .text-wrapper-6 {
  position: absolute;
  top: 430px;
  left: 138px;
  font-family: "Inter-MediumItalic", Helvetica;
  font-weight: 500;
  font-style: italic;
  color: #000000;
  font-size: 26px;
  letter-spacing: 0;
  line-height: normal;
  white-space: nowrap;
}

.iphone-pro-max .rectangle-7 {
  position: absolute;
  top: 499px;
  left: 88px;
  width: 244px;
  height: 42px;
  background-color: #b8e0e8;
  box-shadow: 0px 4px 4px #00000040;
}

.iphone-pro-max .text-wrapper-7 {
  position: absolute;
  top: 504px;
  left: 137px;
  font-family: "Inter-MediumItalic", Helvetica;
  font-weight: 500;
  font-style: italic;
  color: #000000;
  font-size: 26px;
  letter-spacing: 0;
  line-height: normal;
  white-space: nowrap;
}

.iphone-pro-max .rectangle-8 {
  position: absolute;
  top: 575px;
  left: 88px;
  width: 244px;
  height: 42px;
  background-color: #b8e0e8;
  box-shadow: 0px 4px 4px #00000040;
}

.iphone-pro-max .text-wrapper-8 {
  position: absolute;
  top: 579px;
  left: 144px;
  font-family: "Inter-MediumItalic", Helvetica;
  font-weight: 500;
  font-style: italic;
  color: #000000;
  font-size: 26px;
  letter-spacing: 0;
  line-height: normal;
  white-space: nowrap;
}

.iphone-pro-max .rectangle-9 {
  position: absolute;
  top: 727px;
  left: 88px;
  width: 244px;
  height: 42px;
  background-color: #b8e0e8;
  box-shadow: 0px 4px 4px #00000040;
}

.iphone-pro-max .text-wrapper-9 {
  position: absolute;
  top: 731px;
  left: 99px;
  font-family: "Inter-MediumItalic", Helvetica;
  font-weight: 500;
  font-style: italic;
  color: #000000;
  font-size: 26px;
  letter-spacing: 0;
  line-height: normal;
  white-space: nowrap;
}

.iphone-pro-max .rectangle-10 {
  position: absolute;
  top: 841px;
  left: 156px;
  width: 216px;
  height: 42px;
  background-color: #f5106f;
  box-shadow: 0px 4px 4px #00000040;
}

.iphone-pro-max .text-wrapper-10 {
  position: absolute;
  top: 846px;
  left: 225px;
  text-shadow: 0px 4px 4px #00000040;
  font-family: "Inter-SemiBold Italic", Helvetica;
  font-weight: 600;
  font-style: italic;
  color: #000000;
  font-size: 26px;
  letter-spacing: 0;
  line-height: normal;
  white-space: nowrap;
}

.iphone-pro-max .pongal {
  position: absolute;
  top: 671px;
  left: 348px;
  width: 154px;
  height: 159px;
  aspect-ratio: 0.97;
  object-fit: cover;
}

```

## OUTPUT:
![alt text](<Screenshot (55).png>)

## RESULT:
The program to design, develop and deploy a web application for event registration using Figma UI tool is completed successfully.
