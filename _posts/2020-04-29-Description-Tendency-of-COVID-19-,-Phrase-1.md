---
layout: post
title: Description Tendency of COVID-19, Phrase 1
lang: en
categories:
    - Python
tags:
    - Env
 date: 2020-04-29-Description-Tendency-of-COVID-19-,-Phrase-1
---


# Description Tendency of COVID-19, Phrase 1
“ The purpose of this python project based on COVID-19 dataset is to presenting my business intelligence skills through implementing programming language, programming design architecture,  data analysis and visualisation, data manipulation. ”

This project, phrase 1, is merely establishing a fundamental programming framework and extension ability for further development. Therefore, a part of functionalities are not  completed. In term of visualisation, there is only presenting the historical tendency of  the confirmed patients number, which is wrapped up in a method, and it can be easily extended via adding methods due to the ideal of modular design and MVC architecture.

## Technical Features
* JSON API 
* MVC design architecture 
* Data visual - Matplotlib
* Modular design

## Findings
* Object instantiation and invocation in nesting classes should be initialised in the interior of  the class with `__init__` method,  but not using the import implementation.
* `Class Person(Object)` is an inheritance, which refers to more functionalities of objects of class that can be used. 
* The initialisation method `__init__` inside class does not necessary if it is not need, and not affects the initialisation of class object.
* Loading data of JSON can be treated as string, and should be converted to a correct data type, such as integer, to presenting the visual.

## Issues
* Labels of x coordination can be overlay due to a large of amount of accumulated data, such as date. To solve the issue, I want those labels to display in space and not very labels. In this case,  `plt.xticks(range(0, xlen, 7))`can partly solve this issue.  The last parameter, 7, is the distance between lables. However, I notice that the latest dates can be missed display if it happened no equal to 7. So that the issue will be leaved to the next  phrase development. 
* The line graph has not been properly presented with showing statistical numbers based on its timeline. It will be handled in the next phrase.

## Summary
The framework of this project has been properly developed for further development based on MVC design architecture. It is also a well practice for programming pattern design and module design.  In term of data visualisation based on Matplotlib, the preliminary functions have been properly implemented in order to understand the basic idea of the python library. More functionalities and fining code will be carried on in the next phrase. 






