---
title: "Introduction to R"
date: 2026-10-01T10:48+04:00
categories:
  - blog
tags:
  - extra-credit
---

Wanna learn about R in a single evening? Then an event "Introduction to R" held by NYU Libraries was just for you. It was held last Friday, at 10 PM GMT +4, and covered surprisingly a lot in just 2 hours.


## Summary of the Event

Workshop has started pretty chill, with navigation of RStudio IDE. I have worked on [posit.cloud][posit.cloud], since it is comfortable to use, allows portability and does not require installation of any software.

After they glazed RStudio for a bit (deservedly), namely they mentioned *automatic working directory*, *state restoration*, *cursor placement*, *isolated environments*, *ultimate portability*.

After that we have ran some commands, through console, line selection, and running the whole chunk using `cmd+shift+enter`.

Then there was an introduction to variables, functions and some data structures, vector and data frame. 

One takeaway was probably that object determines what actions we do with it. If we're looking to design a solution for a problem, we should always base off from the problem definition first. We should work on the architecture of our data more carefully. For example, if we want to store numbers but choose to define them as strings, we will not be able to perform `sqrt()` operation on it. Our decisions in the beginning stage will stay with us until the very end.

After that, we did a bunch of operations with `na` values. `is.na()`, `count(is.na)`, `drop_na` were the functions we worked with. This I find very useful, because in sparse datasets, that is in datasets with a lot of empty entries, we will be able to apply some functions very easily. One example I could see of me using this in my life is when calculating the average out of those who entered values, because some datasets put 0 instead of no entry, which brings down the average drastically.

Next we moved to using packages. We have learned how to install datasets. How install.packages("package") is different than library(package). We have primarily worked with NHANES, and within NHANES we were advised to use tidyverse dataset, because it's usually neat, and philosophy behind all the tidyverse datasets is same.

After that we did some work with importing/exporting data in csv, xlsx formats. 

Another feature that I find would be very useful, especially when connecting two different datasets, or just working with datasets in general, was the functions with altering the dataset. `rename(), mutate(), filter(), select(), arrange(), count()` for example. 

Next part of workshop focused on continuous and categorical variables. Continuous variables is where variables are in some sort of consistent order between each other. For example age, hex color, weight. Anything that has to do with numbers more or less. Categorical variables on the other end are type of variables which can be divided into kinds, into distinct kinds. For example, colors, age categories (child, adult, elderly,etc.). We have learned how to turn continuous variables into categorical ones, and how to turn categorical variables into some other categorical ones. An example of continuous to categorical variable transformation would be converting the age of the person to a whether they're an adult or a child.


Lastly, we have looked at building plots with ggplot2. It was quite useful, and I liked the level of customizability ggplot2 provides: how you can change colors, labels. Or choose a preset theme. Histograms and boxplots will be extremely useful to show the difference between the zones more qualitatively. For example, I want to work with Germany - analyze the differences between East and West - and I think histograms will be of immense use there to show the difference in development and its effects on the modern-day Germany.

![ggplot]({{ '/assets/images/ggplot_explanation.png' | relative_url }})

I think outside of class the stuff I learned in class will be useful in my capstone as well, where I am building a dataset of Quranic variants and collecting them into a single database. I will be able to perform analysis on text more naturally, find the differences better and get better insights from the data, because I am better versed in graphs now. ggplot2 is quite fun.

## Useful resources

### PDF 

It was provided as a supplemental material before the session began, on this [page][https://nyu.libcal.com/event/17490476?c=0.13652513867939664]. Provides a good overview of the event, and includes all the exercises we have done. Can serve as sort of a cheatsheet.

[View PDF]({{ '/assets/introduction-to-r/introduction_to_R.pdf' | relative_url }})

### R project file

Downloaded from the same page as a PDF, and instructor has run through this file during the session. Was useful because we could follow the instructor and gain hands-on experience.

[Download R project file]({{ '/assets/introduction-to-r/introduction_to_R (1).qmd' | relative_url }})


## Comment on usage of AI

- Only used ChatGPT Codex, but not as an agent. Questions were structured as "how to do _task_? Don't write into the file, show me how to do it. I take full responsibility over the code.

- to learn how to insert links to PDF and qmd files to the .md file.