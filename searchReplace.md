# Hints for Search and Replace

* ```:s/patternToReplace/replaceWith/options``` 
    * option flags:
        * ```c``` : asks for a *y* or *n* before replacing
        * ```g``` : replaces all the occurances on the line rather than just
          the first
    * More on ```:s```
        * ```:s``` does just for  the current line
        * ```:%s``` for whole file
        * in visual mode select a region before ```:s``` to replace in that
          region
        * can give a line range
            * static numbers ```:start,ends/```
                * start is the line to start on
                * end is the last line 
            * relative numbers ```:-num1,+num2s/```
                * relative lines to the current line
                * $-num$ is how many lines before current line
                * $+num$ is how many lines after current line
                * *any* combination seems to work... 
    * The ```\``` is used to escape characters in the patterns
        * example: ```\/``` to escape / or ```\*``` for *
* ```*``` : searches for the currently highlighted word
* ```cgn``` : 
    * cuts the current highlight or word
    * replaces the word
    * goes to the next occurrence
    * ```.``` : repeats ```cgn``` process

[Home](README.md)
