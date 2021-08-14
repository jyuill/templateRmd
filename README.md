README
================
JY
2021-08-14

## R Markdown Templates for Figure 4

R Markdown Templates designed for Figure 4.

### Templates

(names are specified in ‘template.yaml’ for each template - see Creation
section below for more.)

-   **basic template (fig4)**: simple features including
    -   author based on system username
    -   date based on current system date when knit
    -   most common packages loaded
    -   tabbed layout
    -   table of contents
-   **basic - code (fig4)**: as above but with code folding

### Usage

1.  install package from github repo:
    **devtools::install\_github(repo=“jyuill/templateRmd”)**
2.  load for use: library(templateRmd)

### Template Creation

R Markdown templates require a package. A couple extra steps and it’s
easy to setup, share, maintain.

1.  In RStudio: create NEW project &gt; New directory &gt; R package
    using devtools &gt; name of package
    -   this will load a couple of files/directories needed for basic
        package
2.  DESCRIPTION: update info
3.  New directory for markdown template: **inst &gt; rmarkdown &gt;
    templates &gt; folder name for template**
4.  In folder for template:
    -   **template.yaml** file: name: template name as you want to
        appear in template list when creating new R Markdown
        -   works for me with template name in quotes, other examples
            show no quotes.
    -   **skeleton** folder: add markdown file ‘skeleton.Rmd’ with
        template features.
5.  Create Github repo based on the R project:
    -   easy way to do this is to manually create a Github repo with
        same name.
    -   follow instructions for commands to run in Shell to push files
        from computer to repo.

That’s basically it! Good to go with Usage instructions above.

References for template creation:

-   R Markdown Cheat Sheet
-   <https://rstudio.github.io/rstudio-extensions/rmarkdown_templates.html>
-   <https://chester.rbind.io/ecots2k16/template_pkg/>

## Updates

1.  Make changes in RStudio, as with any repo.
2.  Push changes back to Github.
3.  Re-install package for use - see ‘Usage’ above.
4.  Add new templates by creating new folder under ‘templates’ and
    pushing to repo.
