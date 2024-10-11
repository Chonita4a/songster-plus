# songster-plus
Script for any browser for songsterr.com

This script is to avoid the annoying popup that the page emits, allowing you to enjoy the tabs without problems.

The script is simple, first look for a class with name "rq1ph" and execute a click on the "a" tag inside it, all this in an interval of 200 milliseconds and that's it.

1.- Open https://www.songsterr.com/

2.- Open devTools of your browser, "F12"

3.- Write "allow pasting" or something like that to give permissions.

4.- Paste this script and press "enter":

```markdown
setInterval(function() {
                const link = document.querySelector('.rq1ph a');
                if (link) {
                    link.click();
                }
            }, 200); //in milliseconds.
```
5.- Enjoy.

NOTE: The timer defaults to 200, but you can change it if you wish.
