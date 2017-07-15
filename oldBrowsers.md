# Why your site has to be compatible with older browsers

I can hear you saying, *“what do I have to do with people who think it’s okay to use IE9”*. And I see where you’re coming from. If people want to see your site, they should just update their browser. And telling you as a developer. I thought the exact same thing. Why should it?

## Not everyone on a computer, is a developer
What I’m trying to say with this, is that not all the users on the web, are familiar with computers, or technology. There are a lot of people who don’t even know how to update their computer or browser. And why should we take away their access to sites. Just because they don’t have the knowledge that you have?

Okay, it also depends on who your target audience is. But there are a few billion sites out there, who’s target audience aren’t teenagers. Or even an audience that uses the computer for everything. There are still people out there, who don’t live with their phones and computers stuck to their body. Think about it, sites about how to use medicine, recipes, information on their town hall, etc.
These people also need their information. Why take that away from them?

## Let’s talk about very large companies
If you’re creating a site for a very big company, there’s a good chance the company itself still works with IE9 or even IE8. As a developer, you can’t tell them to just update their browsers, because otherwise they won’t be able to watch their own website in the office.
When you’re working for a company that already exists for a long time, the chances are big that the computers even will be outdated. And because of the outdated computers, they can’t update their browser, because the computer can’t cope with it. You’re basically telling the company to buy some new computers. When they ask you why, your answer can’t be: *“I just don’t want to make a site work on IE9”*. But that really is the reason why, and you’re telling them you are kind of lazy. This can’t be how the web is going to work.

And I know why you’re thinking these things. Because I’ve been there. And then a teacher gave us a good reason to change our minds a bit. He told us, that if the older browsers like Internet Explorer are going to be deleted, what is the fun about being a front-end developer? What would be the challenge, because if we are going to create sites that only work on the newest browsers. It wouldn’t be difficult, computers can do that. Fancy themes can do that.
The reason that you want to be a front-end developer, should be that you’d like to explore the web, to deliver a great site, that works cross-device, and of course, cross-browser.

## Don’t be that person:
Don’t think *“But 95% of the target audience can see the site”*, those other 5% deserve to see the site just as much as the rest. And don’t get me wrong, I’m not saying that your site should work as perfect on the oldest browser as the newest browser. I’m saying that your site should work.

What I mean with that is, the basis of the site should work. Don’t let CSS or JavaScript screw up your content. HTML only should be the perfect basis. Start making your site with only HTML, once that works (check it on older browsers to) start giving it a basic design with CSS. Try to progressive enhance your website per browser. So, if a browser does support `display: flex; `, enhance your site with display flex. But make sure, that when it doesn’t support that, the site will still work on a different way.

Do the same thing with JavaScript. Use it only on the browsers where the particular function is supported. Write a check and only run the code if it is supported.

![M&M representation](/images/menm.jpg)<br/>
<sup>3: alistapart.com</sup>

The reason why I’m telling you to enhance, and not to downgrade it, is because, it has a better outcome. When you’re downgrading, you’re taking away functions from the site, which might have been needed on all the browsers. When you’re enhancing, you’re sure that your site works on the crappiest browser that you want. And you can start making it more beautiful for the better browsers.
This actually saves you time. When downgrading, you have to choose what you want to lose, and that could be extremely difficult. Adding stuff to a site is much easier, which is what you do with enhancing.

And of course, your site doesn’t have to work in IE5, or a browser that literally supports nothing. You can be reasonable with that. But browsers like IE9 are browsers that are actually used by lots of people. Think about your target audience and use that to draw the line.

I hope this article makes you think about these points. Make the web greater by making it available for a greater audience.

Sources
1.	https://levinsonblock.com/2-steps-make-old-browsers-work-new-websites/
2.	https://www.smashingmagazine.com/2012/07/old-browsers-are-holding-back-the-web/
3.	https://alistapart.com/d/understandingprogressiveenhancement/m-m.jpg
4.	https://ux.stackexchange.com/questions/64250/do-websites-still-have-to-support-internet-explorer-8-and-below/
