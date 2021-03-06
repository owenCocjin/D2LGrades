# Slate Grades
> Browser extension that shows your grades in D2L!

---

## Usage
> The recommended installation method is through the app stores, but in certain cases you can manually install.

The addon will modify the page (hence the scary warning about using data from the sites) and add the calculated grade beside the "Grade" header.
<div style="text-align:center;margin-bottom:20px">
	<img src="https://github.com/owenCocjin/D2LGrades/raw/master/Pics/ford2lgrades.png"/>
</div>

It will also add a row to the table with information on the calculated marks:
| Grade Item | Points | Weight Achieved | Grade |
| --- | --- | --- | --- |
| Title of row | Existing weights | Your score out of the existing weights | Calculated grade |

<div style="text-align:center;">
	<img src="https://github.com/owenCocjin/D2LGrades/raw/master/Pics/ford2l.png"/>
</div>

__Note:__ If the _Points_ column isn't 100/100, then your missing some marks; The prof might not have posted the marks yet. Better get on that!

<br/>

## Support
> Only certain sites, browsers, etc... are supported

#### Browsers
Currently only the following browsers are supported:
- Firefox (Rejected from store due to a "limited audience")
- [Chrome](https://chrome.google.com/webstore/detail/d2l-grades/ifdhnjknhbaodcekanmodnnlkedklkbm)

#### Sites
Should work with any site using D2L. The addon matches the following:
- `https://\*/d2l/lms/grades/my_grades/main.d2l?ou=\*`

<br/>

## Manual Installation
The packages should be in the app store of your respected browser. If not there are packages in this repo which you can install manually.

#### Firefox
1. Download the latest `d2l_grades-X.X-fx.xpi` file ([Latest](https://github.com/owenCocjin/D2LGrades/raw/master/Distributions/XPI/d2l_grades-1.1-fx.xpi)).
2. In Firefox, go to __Addons__ ([Ctrl+Shft+A])
3. Click the gears in the top right -> __Install Add-on From File__
4. Find the `.xpi` package, select it, click __Add__ on the popup
5. Congrats! Go check your grades in D2L!

#### Chrome
1. Clone this repo _OR_ download `d2lgrades.chrome.zip` file ([Latest](https://github.com/owenCocjin/D2LGrades/raw/master/Distributions/ZIP/d2lgrades.chrome.zip)) and unzip it to a folder. From here we'll assume the unzipped/cloned contents are in `~/D2LGrades/Chrome/`
2. Go to `chrome://extensions` and check __Developer Mode__ in the top right.
3. Click __Load Unpacked__ and select the `~/D2LGrades/Chrome/` folder (There should be a `manifest.json` file in it).
4. Congrats! A new extension "D2L Grades 1.0" should have popped up. Go check out your grades now!

<br/>

## Limitations
- D2L isn't standardized, so the addon might not work for some courses. If the grades table's columns follow the order:
```
"Grade Item", "Points", "Weight Achieved", "Grade"
```
Then it should be fine.
- Firefox has rejected the addon from its store as it has a "limited" audience. Manual installation is required for Firefox.
