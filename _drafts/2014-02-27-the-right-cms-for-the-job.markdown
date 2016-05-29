---
layout: post
title:  "The Right CMS For The Job"
date:   2014-02-27
---

I am not a tools-first developer. I don't describe myself as an "iOS developer", "Rails developer", or a "Node developer" because I really enjoy tackling new and different problems with the right tool for the job.

When I set out to build <a href="http://www.lorimakes.com/" target="_blank">Lori's website</a> last year I really wanted to find a CMS with a small footprint that would also be easy and enjoyable for her to use. Thankfully, I found <a href="http://www.anchorcms.com/">Anchor CMS</a>. It fit all of my requirements and more. Further, it is open source and I was able to make some contributions to the source while working with it.

I got so excited about Anchor that I took it for granted that I would use it when the time came to rebuild my own website. That's how I fell into the tools-first trap that, honestly, bogged me down and delayed the rebuild for weeks. I wanted to use Anchor but I couldn't match its data model and templating conventions with my desire for simplicity in design. Anchor is structured around (blog) posts and pages. For Lori's website I hacked pages into behaving as projects. This turned out well because her work is visual: the entire site is based on images. I wanted to maintain this approach on ntdb.net but did not want an image-based implementation. My stubborn desire to shoehorn Anchor into a design-shoe that it didn't fit led to weeks of frustration.

Enter <a href="http://jekyllrb.com/" target="_blank">Jekyll</a>. While sitting in a coffee shop in Chicago last week I remembered finding multiple plain-text "CMS" implementations while researching for Lori's website. Upon investigation and going much further through the documentation than I'm used to, I realized that Jekyll was the tool I had wanted without knowing it.