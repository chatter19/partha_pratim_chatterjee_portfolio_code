---
date: 2017-04-10T11:00:59-04:00
description: "A ball classifier to identify balls from different sports."
featured_image: "/images/matrix_results.png"
title: "Project 2: EDI Parser"
---

For this example project I built a ball classifier to identify balls from different sports. This could be useful for someone who is new to sports from a certain country. They could take a picture of a ball and an app could serve them some information about the history and rules of the game. This is the underlying model for building something with those capabilities.

I was able to get the model to predict the sport of the ball with 94% accuracy after minimal tuning. For most of the cases this would meet the need of an end user of the app. To get these results I used transfer learning on a CNN trained on rsnet34. This created time efficiencies and solid results.

{{< figure src="/images/matrix_results.png" >}}

[Link to GitHub Repository](https://github.com/PlayingNumbers/ds_salary_proj)
