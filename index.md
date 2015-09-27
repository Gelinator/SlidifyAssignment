---
logo        : 4719eb8d7229ccc240deb9b16ebd02b2.jpg
title       : Exploration and Predictions of the Iris Dataset
subtitle    : Because We Can
author      : Developing Data Products
job         : Data Science Specialization
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : default      # 
widgets     : [mathjax]            # {mathjax, quiz, bootstrap}
mode        : standalone # {standalone, draft}
knit        : slidify::knit2slides

---

## What It Does


For you investigative human being who always wished to be able to predict the species of iris flowers by measuring its petals' width and length, search no more!

It can be found following this link:
[Exploration and Predictions of the Iris Dataset](https://gelinator.shinyapps.io/MyShinyApp "Iris Prediction App")

---




## Exploration

The exploration segment consists of using the sliders to position the desired petal measurements. The input from the sliders is fed to the vertical and horizontal lines from the **ggplot2** graph to form a crosshair, indicating where this specimen would be located compared to the observations in the iris dataset.

---

## Prediction

Using a random forest algorithm on the entire dataset, the resulting predictive model is with the two values provided by the slider inputs, and returning the predicted iris species. The reason for choosing these two measurements is two folds. First, the interpretation and presentation of a two-dimensional model is relatively simple. As the next slide will show, it also provides considerable predictive accuracy.

---

## Explaining the Rationale



Using all the variables gave an accuracy of 0.944, with the following results as variable importance is concerned.


|             | Overall|
|:------------|-------:|
|Sepal.Length |    18.2|
|Sepal.Width  |     0.0|
|Petal.Length |    95.6|
|Petal.Width  |   100.0|


Petal width and length really stand out as the main distinctive variables and a model built solely on those two variables gave similar accuracy at 0.951, hence their selection for the app.
