---
layout: post
title: "Lab 10: The Final One!"
author: Fin Lockert
categories: misc
---

Today my group and I were able to finish the final lab for this year! That means we only have to focus on the final project and we're done. In this lab, we made a remotely hosted database website, although all it has on there for now are the incompleted issues on our group GitHub repository. The tutorial, when we were able to get past the hurdles from the very beginning, was very easy and took almost no time to complete.

What were those early issues, you ask? Well, I should start by saying that the tutorial lacking crucial information was not the main problem this time. Instead, it was actually using the Azure portal (also that DotNet was recently updated to 8.0 but we'll get to that later). In the original repository we set up, which has since been deleted since The Great Reset, I had made it with the sample application before using the forked stuff from GitHub that the tutorial said to. That wasn't an actual problem, but it wasn't something that benefitted us either. 

The main problem with the Azure portal is when we were creating the Web App + Database, because as a default it set it to "PostgreSQL" rather than "AzureSQL," which the tutorial didn't mention in the first place since that was likely a default previously. When this was discovered, we also found out that the student subscription we were using did not even allow us to use AzureSQL in the first place, though this was an easy fix (literally just a checkbox) when we found it. After figuring this out, the troubleshooting to fix what we had was taking much longer than it would to just restart, which is what we did.

Otherwise, the DotNet becoming 8.0 was a relatively simple fix, where we were told to write "dotnet tool install -g dotnet-ef" on the workflows we instead hat to write "dotnet tool install -g --version 7.0 dotnet-ef" which is almost no change at all.

While it looks like all the work on the GitHub came from me, and it did actually all come from my account, this was just the easiest way for us to do it. Note: I did **NOT** do all of the work myself, we just used my computer while we were at the library together, both last night and earlier this evening at the time of writing this (on November 21st, 2023).

To see our beautiful, plain and not stylized lab, please click [here](https://msdocs-core-sql-ayz.azurewebsites.net/). Thanks!