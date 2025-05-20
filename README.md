# GRN-member-slides
Create slides for each GRN member based on a google form

This guide assumes you have an up-to-date version of `R`, `RStudio` and `Quarto` installed.


To create the slides, go through the following steps:

- Open `create_slides.qmd` in RStudio.
- Install the required packages.
```r
install.packages(c("rmarkdown", "quarto", "googlesheets4"))
```
- Test if running the code chunks works. 
The command `gs4_auth()` should open a browser window and ask you for access to your google account.
You have to choose a google account that has access to the file we call `sheet_url`.
- Click the button `Render` or use the commands
```r
library("quarto")
quarto_render("create_slides.qmd")
```