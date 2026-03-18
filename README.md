# Ex08 Event Registration Web Application
## Date: 18/3/2026

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

Page 1
```
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
    <div class="android-compact">
      <img class="mobile-bg" src="img/mobile-bg-1.png" />
      <div class="a-hour-hackathon">
        a 24-hour hackathon<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;only solo
      </div>
      <img class="logo" src="img/logo-1.png" />
      <img class="rectangle" src="img/rectangle-1.svg" />
      <div class="text-wrapper">REGISTER</div>
      <div class="hack-vision">Hack-Vision<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2026</div>
      <img class="hackathon" src="img/ex9-hackathon-1.png" />
      <p class="date-april">Date : 1 April 2026<br />Venue : SEC 4th floor</p>
    </div>
  </body>
</html>

global.css

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
/* @FONTWARNING[{"type": "restricted", "family": "Inter-BlackItalic", "weight": "900", "style": "italic", "allowsCrossOrigin": false}] */

@font-face {
  font-family: "Inter-BlackItalic";
  src: local("Inter-BlackItalic");
}
/* @FONTWARNING[{"type": "restricted", "family": "Inter-SemiBold Italic", "weight": "600", "style": "italic", "allowsCrossOrigin": false}] */

@font-face {
  font-family: "Inter-SemiBold Italic";
  src: local("Inter-SemiBold Italic");
}

style.css

.android-compact {
  background-color: #ffffff;
  width: 100%;
  min-width: 405px;
  min-height: 775px;
  position: relative;
}

.android-compact .mobile-bg {
  position: absolute;
  top: 79px;
  left: 0;
  width: 405px;
  height: 724px;
  aspect-ratio: 0.56;
  object-fit: cover;
}

.android-compact .a-hour-hackathon {
  position: absolute;
  top: 515px;
  left: 85px;
  font-family: "Inter-BlackItalic", Helvetica;
  font-weight: 900;
  font-style: italic;
  color: #000000;
  font-size: 20px;
  letter-spacing: 0;
  line-height: normal;
}

.android-compact .logo {
  position: absolute;
  top: -1px;
  left: 0;
  width: 405px;
  height: 80px;
  aspect-ratio: 5.01;
  object-fit: cover;
}

.android-compact .rectangle {
  position: absolute;
  top: 693px;
  left: 51px;
  width: 280px;
  height: 83px;
}

.android-compact .text-wrapper {
  position: absolute;
  top: 716px;
  left: 105px;
  width: 203px;
  font-family: "Inter-BlackItalic", Helvetica;
  font-weight: 900;
  font-style: italic;
  color: #ffffff;
  font-size: 36px;
  letter-spacing: 0;
  line-height: normal;
}

.android-compact .hack-vision {
  position: absolute;
  top: 116px;
  left: 53px;
  width: 308px;
  font-family: "Inter-BlackItalic", Helvetica;
  font-weight: 900;
  font-style: italic;
  color: #fe1414;
  font-size: 48px;
  letter-spacing: 0;
  line-height: normal;
}

.android-compact .hackathon {
  position: absolute;
  top: 261px;
  left: 36px;
  width: 339px;
  height: 226px;
  aspect-ratio: 1.5;
  object-fit: cover;
}

.android-compact .date-april {
  position: absolute;
  top: 599px;
  left: 61px;
  font-family: "Inter-SemiBold Italic", Helvetica;
  font-weight: 600;
  font-style: italic;
  color: #000000;
  font-size: 24px;
  letter-spacing: 0;
  line-height: normal;
}

```

page 2
```
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
    <div class="android-compact">
      <img class="logo" src="img/logo-2.png" />
      <div class="text-wrapper">Registration Form</div>
      <p class="NAME-INSTITUTION-AGE">
        NAME :<br /><br />INSTITUTION:<br /><br />AGE :<br /><br />DOMAIN :<br /><br />SKILLS :<br /><br />DEPARTMENT
        :<br /><br />MOBILE :<br /><br />Email ID :
      </p>
      <div class="rectangle"></div>
      <div class="ellipse"></div>
      <div class="div"></div>
      <div class="rectangle-2"></div>
      <div class="rectangle-3"></div>
      <div class="rectangle-4"></div>
      <div class="rectangle-5"></div>
      <div class="rectangle-6"></div>
      <div class="rectangle-7"></div>
      <div class="rectangle-8"></div>
      <div class="text-wrapper-2">SUBMIT</div>
    </div>
  </body>
</html>

globaal.css

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
/* @FONTWARNING[{"type": "restricted", "family": "Jersey 20-Regular", "weight": "400", "style": "normal", "allowsCrossOrigin": false}] */

@font-face {
  font-family: "Jersey 20-Regular";
  src: local("Jersey 20-Regular");
}
/* @FONTWARNING[{"type": "restricted", "family": "K2D-Regular", "weight": "400", "style": "normal", "allowsCrossOrigin": false}] */

@font-face {
  font-family: "K2D-Regular";
  src: local("K2D-Regular");
}
/* @FONTWARNING[{"type": "restricted", "family": "K2D-ExtraBold", "weight": "800", "style": "normal", "allowsCrossOrigin": false}] */

@font-face {
  font-family: "K2D-ExtraBold";
  src: local("K2D-ExtraBold");
}

style.css

.android-compact {
  background-color: #f989ee;
  width: 100%;
  min-width: 407px;
  min-height: 799px;
  position: relative;
}

.android-compact .logo {
  position: absolute;
  top: 0;
  left: 1px;
  width: 406px;
  height: 81px;
  aspect-ratio: 5.01;
  object-fit: cover;
}

.android-compact .text-wrapper {
  position: absolute;
  top: 115px;
  left: 74px;
  width: 249px;
  font-family: "Jersey 20-Regular", Helvetica;
  font-weight: 400;
  color: #000000;
  font-size: 36px;
  letter-spacing: 0;
  line-height: normal;
  white-space: nowrap;
}

.android-compact .NAME-INSTITUTION-AGE {
  position: absolute;
  top: 188px;
  left: 15px;
  font-family: "K2D-Regular", Helvetica;
  font-weight: 400;
  color: #000000;
  font-size: 24px;
  letter-spacing: 0;
  line-height: normal;
}

.android-compact .rectangle {
  position: absolute;
  top: 313px;
  left: 89px;
  width: 230px;
  height: 27px;
  background-color: #d9d9d9;
}

.android-compact .ellipse {
  top: 204px;
  left: 129px;
  width: 7px;
  height: 1px;
  border-radius: 3.5px / 0.5px;
  position: absolute;
  background-color: #d9d9d9;
}

.android-compact .div {
  top: 182px;
  left: 113px;
  width: 233px;
  height: 46px;
  border-radius: 116.5px / 23px;
  position: absolute;
  background-color: #d9d9d9;
}

.android-compact .rectangle-2 {
  position: absolute;
  top: 254px;
  left: 180px;
  width: 215px;
  height: 31px;
  background-color: #d9d9d9;
}

.android-compact .rectangle-3 {
  position: absolute;
  top: 374px;
  left: 129px;
  width: 213px;
  height: 28px;
  background-color: #d9d9d9;
}

.android-compact .rectangle-4 {
  position: absolute;
  top: 436px;
  left: 120px;
  width: 222px;
  height: 28px;
  background-color: #d9d9d9;
}

.android-compact .rectangle-5 {
  position: absolute;
  top: 502px;
  left: 204px;
  width: 170px;
  height: 21px;
  background-color: #d9d9d9;
}

.android-compact .rectangle-6 {
  position: absolute;
  top: 568px;
  left: 129px;
  width: 245px;
  height: 27px;
  background-color: #d9d9d9;
}

.android-compact .rectangle-7 {
  position: absolute;
  top: 627px;
  left: 133px;
  width: 241px;
  height: 20px;
  background-color: #d9d9d9;
}

.android-compact .rectangle-8 {
  position: absolute;
  top: 690px;
  left: 40px;
  width: 319px;
  height: 78px;
  background-color: #2162bf;
  box-shadow: 0px 4px 4px #00000040;
}

.android-compact .text-wrapper-2 {
  position: absolute;
  top: 703px;
  left: 133px;
  font-family: "K2D-ExtraBold", Helvetica;
  font-weight: 800;
  color: #ffffff;
  font-size: 40px;
  letter-spacing: 0;
  line-height: normal;
}

```
page 3

```
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
    <div class="android-compact">
      <img class="logo" src="img/logo-3.png" />
      <div class="text-wrapper">SUCCESS!!!</div>
      <p class="your-registration-is">
        Your Registration is complete<br /><br />Stay tuned to show cse yor skills<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;and
        receive prizes
      </p>
      <div class="rectangle"></div>
      <p class="for-queries-CONTACT">
        For Queries ; CONTACT<br /><br />
        1234-567-890<br />sav@fake.com
      </p>
    </div>
  </body>
</html>


global.css

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
/* @FONTWARNING[{"type": "restricted", "family": "K2D-ExtraBold", "weight": "800", "style": "normal", "allowsCrossOrigin": false}] */

@font-face {
  font-family: "K2D-ExtraBold";
  src: local("K2D-ExtraBold");
}


style.css

.android-compact {
  background-color: #88e8dd;
  overflow: hidden;
  width: 100%;
  min-width: 409px;
  min-height: 799px;
  position: relative;
}

.android-compact .logo {
  position: absolute;
  top: 0;
  left: 0;
  width: 409px;
  height: 84px;
  aspect-ratio: 5.01;
  object-fit: cover;
}

.android-compact .text-wrapper {
  position: absolute;
  top: 218px;
  left: 32px;
  width: 404px;
  font-family: "K2D-ExtraBold", Helvetica;
  font-weight: 800;
  color: #14017f;
  font-size: 64px;
  letter-spacing: 0;
  line-height: normal;
}

.android-compact .your-registration-is {
  position: absolute;
  top: 381px;
  left: 32px;
  width: 402px;
  font-family: "K2D-ExtraBold", Helvetica;
  font-weight: 800;
  color: #000000;
  font-size: 24px;
  letter-spacing: 0;
  line-height: normal;
}

.android-compact .rectangle {
  position: absolute;
  top: 586px;
  left: 16px;
  width: 367px;
  height: 172px;
  background-color: #29a2f3;
  transform: rotate(180deg);
  box-shadow: 0px 4px 4px #00000040;
}

.android-compact .for-queries-CONTACT {
  position: absolute;
  top: 606px;
  left: 42px;
  font-family: "K2D-ExtraBold", Helvetica;
  font-weight: 800;
  color: #ffffff;
  font-size: 24px;
  letter-spacing: 0;
  line-height: normal;
}


```
## OUTPUT:

<img width="1920" height="1080" alt="Screenshot (133)" src="https://github.com/user-attachments/assets/056d4c51-73dc-4c8b-bff4-2ec363140e8d" />


## RESULT:
The program to design, develop and deploy a web application for event registration using Figma UI tool is completed successfully.
