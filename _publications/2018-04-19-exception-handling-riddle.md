---
title: "The exception handling riddle: an empirical study on the Android API"
collection: publications
permalink: /publication/2018-04-19-exception-handling-riddle
excerpt: "We examine the use of the Java exception types in the Android platform's Application Programming Interface (API) reference documentation and their impact on the stability of Android applications. We develop a method that automatically assesses an API's quality regarding the exceptions listed in the API's documentation. We statically analyze ten versions of the Android platform's API (14–23) and 3539 Android applications to determine inconsistencies between exceptions that analysis can find in the source code and exceptions that are documented. We cross-check the analysis of the Android platform's API and applications with crash data from 901,274 application execution failures (crashes). We discover that almost 10% of the undocumented exceptions that static analysis can find in the Android platform's API source code manifest themselves in crashes. Additionally, we observe that 38% of the undocumented exceptions that developers use in their client applications to handle API methods also manifest themselves in crashes. These findings argue for documenting known might-thrown exceptions that lead to execution failures. However, a randomized controlled trial we run shows that relevant documentation improvements are ineffective and that making such exceptions checked is a more effective way for improving applications' stability."
date: 2018-04-19
venue: 'Journal of Systems and Software'
paperurl: 'https://doi.org/10.1016/j.jss.2018.04.034'
citation: 'Maria Kechagia, Marios Fragkoulis, Panos Louridas, and Diomidis Spinellis. (2018). &quot;The exception handling riddle: an empirical study on the Android API.&quot; Journal of Systems and Software. volume 142. pages 248-270. doi: 10.1109/TC.2017.2695447.'
---

