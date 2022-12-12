<img src="./img/cv_photo.png" alt="Vladislav Molodid's photo" width="200" height="200"/>

# Vladislav Molodid
* **Phone**: +375 44 748-00-95
* **E-mail**: [molodid.vladislav@gmail.com](mailto:molodid.vladislav@gmail.com)
* **Location**: Mogilev, Belarus
* **Github**: https://github.com/arkey99700

## About me
I am a passionate self-educated front-end developer who is eager to explore new web technologies and new ways of creating web applications and improving user experience!

## Experience
* **Fullstack Developer**<br>
*Sotbit*<br>
Oct 2022 - Present<br>
Mogilev, Belarus
* **Functional Testing Trainee**<br>
*EPAM Systems*<br>
Jan 2020 - May 2020<br>
  Mogilev, Belarus

## Education
* **Mogilev State A.Kuleshov University**<br>
Bachelor's degree, Romano-Germanic Philology<br>
2015 - 2020

## Skills
* **HTML**
* **CSS/SCSS**
* **JavaScript (Node.js, Vue.js)**
* **PHP (Bitrix)**
* **Git**
* **Figma**
* **Adobe Photoshop**

## Code Example
[(4 kyu) Human readable duration format](https://www.codewars.com/kata/52742f58faf5485cae000b9a)

    function formatDuration (seconds) {
      if (seconds === 0) return "now";
      
      const secondsInUnits = {
        year: 31536000,
        day: 86400,
        hour: 3600,
        minute: 60,
        second: 1
      };
      let result = [];
    
      function getUnitsFromSeconds(sec, unit = "second") {
        let int = 0,
        temp = "";
    
        if (seconds > 31535999) {
          unit = "year";
        } else if (seconds > 86399) {
          unit = "day";
        } else if (seconds > 3599) {
          unit = "hour";
        } else if (seconds > 59) {
          unit = "minute";
        }
        
        int = Math.floor(sec / secondsInUnits[unit]);
        seconds = sec -= int * secondsInUnits[unit];
        temp = `${int} ${unit}`;
        if (int > 1) temp += "s";
        
        result.push(temp);
      }
      
      while (seconds > 0) {
        getUnitsFromSeconds(seconds);
      }
    
      return result.length > 1 ? `${result.slice(0, result.length - 1).join(", ")} and ${result[result.length - 1]}` : `${result[result.length - 1]}`
    }

## Languages

* **Russian** - native;
* **English** - C1;
* **French** - A2;