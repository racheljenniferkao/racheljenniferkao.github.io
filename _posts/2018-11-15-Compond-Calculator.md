---
layout: post
title: Compound Calculator
---

Recently I have joined a private equity company, Asia Value Capital, as an intern. In a future post, I will share my experiences in AVC, along with the investment knowledge and tips I have learned from them. My intern tasks include taking notes on how to start investing as a beginner, translating Chinese files and brochures into English, and coding/creating a compound calculator for WeChat Mini Program's platform. 

Our main topic today is how I created the Compound Calculator for WeChat's Mini Program.

What is a WeChat's mini program?
A mini program is an app used in WeChat's platform. So think of an app inside of WeChat. It requires zero downloading, thus you do not need to go to the app/play store to download a mini program. It is already included in the WeChat Application. Pretty neat huh? 

Let's start off with getting a mini program up and running. 

I found this wonderful [easy tutorial](https://developers.weixin.qq.com/miniprogram/en/dev/) made by WeChat to get a basic mini program to run. It comes in English and Chinese.


![tutorial]({{ site.baseurl }}/images/tutorialWechat.png)


In the tutorial above, it requires you to apply for a Mini Program account. Sadly, the application is only available in Chinese. There is another catch, if you are not a Chinese citizen, you can only apply a business/company account. That means if you are a foreigner, you can't have an account for your own personal projects. 


But Rachel, what is the meaning of this post if I can't even apply for an account? 


Don't fret, my fellow readers. 
The alternative or loophole is to create a [test account](https://developers.weixin.qq.com/miniprogram/en/dev/devtools/sandbox.html?t=18111421)!

![Test Account]({{ site.baseurl }}/images/testWechat.png)


After you get your test accoount, simply follow the rest of the [easy tutorial](https://developers.weixin.qq.com/miniprogram/en/dev/). That consist of downloading WeChat's devtools application, along with a quickstart demo to start your mini program. 
After you're done, you will have an application similar as below.

![weChatDev]({{ site.baseurl }}/images/weChatDev.png)

Now you might be wondering out of all things, why make a compound calculator? 
AVC values long term investments. Because long term investments along with compound interest rates can lead to an enormous amount of profit over time. Time in this case would be 5 years and more. So I was off and learning about the coding languages of WeChat.

The first thing I noticed is that Mini Program's language is basically html, css, and javascript. They made their own similar versions, wxml, wxss. I find this as a theme in China, their own version of Facebook, Uber, and Venmo/Square Cash. The cool thing about this is that even though mini programs are similar to apps, the langauges behind it aren't your common application languages, ex: java, swift. Mini programs are essentially websites disguise as apps.

One of the the most helpful pages was the [Components Page](https://developers.weixin.qq.com/miniprogram/en/dev/component/). Since mini program's langauge is not exactly like html, so there are certion exceptions or new tags to look out for. The components page is available in English and Chinese. I really like how for each unique tag name, it nicely list out all its attributes and provides an demo example of how everything works. WeChat also mimics React's lifecycle, they have predefined functions that deals with certain states when a page is loading. 

Below is a picture of all the predefined lifecycle functions:

![lifecycle]({{ site.baseurl }}/images/reactCycle.png)

Now back to the calculator. I found a nice compound interest formula along with a good descriptive explanation [on this website](https://www.thecalculatorsite.com/articles/finance/compound-interest-formula.php?page=2). The website provides your basic compound formula, compound formula with additional deposits at the beginning of the month, and compound formula with additional deposits at the end of the month. For simplicity purposes, I only focused on the formula that dealt with deposits made at the end of the month.
Below is the compound formula I used, along with the definitions of variables.

![formula]({{ site.baseurl }}/images/formula.png)
![formula1]({{ site.baseurl }}/images/formula1.png)

With the formula and some basic knowledge of how weChat Mini Program operates, I'm off to create this money making calculator!
Here is my github repo for my [Compound Calculator Mini Program](https://github.com/racheljenniferkao/Compound-Calculator/tree/master/Compound%20Calculator).

What's next?

There is much more to explore. WeChat has lots of data on their large user base, thus their APIs are super useful and easily accessible. Another thing you can tackle is how to manipulate and play with media on their platform. That's what I will be trying out next. I think a good next experiment would be to make a small animated game.

Future improvements/next steps on the calculator?
I would like to create a switch that allows the users to choose which compound interest formula to use. 
I want to have more compounding options and deposit options.
I would also like to make the results look more presentable. 
Overall, have a better UI. 

Also any recommendations and advices are welcome! Please email me. 

Resourceful/Useful Mini Program Websites: 

[https://github.com/apelegri/wechat-mini-program-wiki](https://github.com/apelegri/wechat-mini-program-wiki)

[https://walkthechat.com/wechat-mini-programs-simple-introduction/](https://walkthechat.com/wechat-mini-programs-simple-introduction/)

[https://developers.weixin.qq.com/miniprogram/en/dev/](https://developers.weixin.qq.com/miniprogram/en/dev/)






