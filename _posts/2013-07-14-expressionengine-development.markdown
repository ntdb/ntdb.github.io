---
layout: post
title:  "ExpressionEngine Development"
date:   2013-07-14
original: "inthepin.es"
originalurl: "http://inthepines.co/posts/expressionengine_development"
---

Confessi... er... humble brag. We don't typically use prebuilt content management systems. We like to keep our hands dirty in many different frameworks and we really enjoy building our own CMS when the time comes. Not only is it good experience for us but it allows us to build a solution that fits the application extremely well. In some cases, however, a client may already be familiar with a certain CMS or otherwise have experience that lends itself towards an existing solution.

One of the frameworks we've grown fond of is Codeigniter: it has everything we want and little that we don't need when building a client/server app. The creators of Codeigniter have done us the favor of building a CMS with it: ExpressionEngine. Their documentation is fantastic and it's easy to find overviews of how the system works. Instead of getting into basics, I want to share two mistakes we made on our first go-around with ExpressionEngine this year and the solutions that saved us loads of time and frustration later.

First, we made the ignorant mistake of using the CMS to build our templates. EE2 stores templates in the database by default and allows developers to modify them via the php-built backend. This means no syntax coloring, no linting, terrible in-page search, and no kind of auto-complete whatsoever. That's bad enough. If your server is at all unreliable or slow (cough cough lithium cough) then you're going to lose time, work, and patience very quickly. Fortunately, EE2 loves devs and is capable of saving templates as files. For our second ExpressionEngine site of the year (check out our projects section soon) we have been using our text editor of choice (Sublime Text 2) to write templates and have been enjoying all of the features above (including syntax coloring via a Sublime plugin made just for EE2).

Second, our deployment process was extremely painful. Expression Engine stores site URLs and file paths in many different places all over the database and they can not natively be batch-updated. Every time we deployed Sidewalk Radio to the staging server we had to go through the backend and find every URL and path and update it to match the current environment. We'd typically discover that we forgot a parameter when an upload didn't work or php errors littered a page. The first solution involved a plugin found on devot-ee which served well. The final and best solution, however, is the poorly-documented ability to have the EE2 database config defer to a config.php file in the site root. We were able to build config files with paths and database credentials specific to each environment, throw them into .gitignore, and just forget about the pains of deployment altogether.

It's not custom and it doesn't always make sense but ExpressionEngine is a solid solution for a project in need of a pre-built CMS. Check it out and don't make our development mistakes.