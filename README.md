##Chapter 4
# using R as a calculator, declaring 'x' as an object
x <- 3 * 4
# object_name <- gets value ; verbal reminder for setup. Object names must start with a letter, and can only contain letters, numbers, _ and " .""
birthday_cake <- 1
birthdaycake.frosting <- 2
#inspect an object by typing its name
birthday_cake

#functions
#look like: function_name(argument)

#practice:
#1 does not work because the object was misspelled when calling it.

#2
library(tidyverse)

ggplot(data = mpg) + 
  geom_point(mapping = aes(x = displ, y = hwy))

fliter(mpg, cyl = 8)
filter(diamond, carat > 3)
#this works fine for me, with the exception of some possible misspellings?

#3 alt + shift + k displays keyboard shortcuts / quick references. You can also achieve this by help > cheatsheets > keyboard shortcuts help in the toolbar.

##Chapter 6
#when using the script editior, make sure all parts of the code are highlighted in order for the progam to run correctly, or ctrl + shift + s.

#practice
#1 (if functions were being used) clicking on "(top level)" next to the line number at the bottom of the script will show you what functions are available throughout the script text. via the comments in: https://twitter.com/edwin_thoen/status/1146739118908628992

#2 RStudio Diagnostics will report lack of arguments OR validity of arguments to function calls, warn you if there are no variable declarations in the scope of the code you are attempting to run, alert certain style and aesthetic mistakes, such as whitespace, and provide diagnostics for other languages such as Python, C/C++ and JavaScript.

##Chapter 8
#There is a great pair of keyboard shortcuts that will work together to make sure you’ve captured the important parts of your code in the editor:

Press Cmd/Ctrl + Shift + F10 to restart RStudio.
Press Cmd/Ctrl + Shift + S to rerun the current script.

#working directory: where R looks for files that you ask it to load, and where it will put any files that you ask it to save. Located at the top of the console.
 you can print this by running: getwd()
 
library(tidyverse)

ggplot(diamonds, aes(carat, price)) + 
  geom_hex()
ggsave("diamonds.pdf")

write_csv(diamonds, "diamonds.csv")

getwd()



