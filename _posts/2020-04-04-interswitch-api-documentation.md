---
layout: post
title: Interswitch API Documentation; New and Improved
tags: [Documentation Interswitch DeveloperExperience]
--- 

April 1st marks the beginning of a new Financial year at Interswitch and I can't help but marvel at what we've been able to achieve in Interswitch Engineering within the last financial year particularly towards improving the experience of developers integrating with our APIs.

When I joined Interswitch in June last year, I was assigned to join the Developer Relations team team. Our goal was to improve the experience of developers integrating with Interswitch APIs. This was a huge feat in itself, to put it lightly, we had received a lot of bad reviews regarding our APIs ranging from the complexity of the APIs which makes integration worrisome, to lack of proper API documentation and sometimes lack of support. However, the topmost issue from the issues listed above was the documentation. I must say, working to improve the documentation platform for Interswitch gave me the opportunity to test so many platforms before arriving at a decision on which best suits our current needs, it has also improved my understanding of API products in Interswitch and also had me working with internal and external developers to ensure that we tackled existing problems to improve the experience of developers integrating with our APIs.

In this article, I will run you through the process of how  Interswitch documentation transformed from [this](https://sandbox.interswitchng.com/docbase/) to [this](https://developer.interswitch.com/docs/), the issues we had with our existing documentation platform, why we chose the new platform and how this new platform addresses the issues in the previous documentation platform.

## The Old Documentation Platform - Docbase

![](https://lh3.googleusercontent.com/Tz2Yf24whR1WWFzmIDFan5U9yAzrUpIJ73vZsb4XgBYYAoFu13Bwa9r1J-nPX51lNX9Jf1ifdRor9diXXoMxquiLoP-N7WqvGXfHoEzkKrgGHlnY1FuJvpSTQiWjr9pkFGdDYeU)

                                                     Docbase homepage

There has been a misconception over the past few years that Interswitch does not have a centralized documentation platform and  PDF documents are given to aid developer's integration with our APIs. While the statement above was true at some point, that scenario changed a long time ago. A few years ago, in a bid to have all API documentation in a single place to improve our external developers experience, we moved our API documentation to [docbase](https://sandbox.interswitchng.com/docbase/) built with [Wordpress](https://wordpress.com/). The move to Docbase was an attempt to solve the issues our users faced when they read our API documentation. While it was able to solve some of those issues, others still persisted.

### Disadvantages of the old documentation platform

1.  Lack of proper awareness among developers during project launch - Developers are the primary users of API documentations and as such should be at the forefront of any awareness campaign done at project launch but this wasn't done when Docbase was launched and that made almost everyone in the developer community unaware of the existence of our documentation platform.

1.  Outdated Content - There was a disconnection between API update and documentation update. Oftentimes, the documentation is not updated when the product API is updated and as such made the documentation become obsolete.

1.  A disconnection between our external and internal developers - Any developer can attest to the fact that whenever they experience issues with integration, getting support from an internal developer gets the issue resolved faster either because the internal developer has more understanding of the API or the fact that they can relate more with your problem from a developer's point of view just as you.

Now don't get me wrong, docbase also has it's advantages such as its provision of a one stop platform for all our APIs and a  community forum page. However, as most of our external developers could attest to the disadvantages outweigh the advantages and with that the need to sort for improvements and create a better platform for our API documentations that addresses the issues of the docbase.

## The New Documentation Platform - Slate

![](https://lh3.googleusercontent.com/raqT1zcPSpT1dqepEs1adOJTzkrzSDUifqh3shbmUx5rcceg6RW5BgQou2pc9rctEjBOOC9QU-d8gtOI-ik5wEAA7G5pCWJkZUHCXSzIpG9JFEPFridZkrK2mmMdL-4Xd5oJTY0)

                                                 Slate product homepage

![](https://lh4.googleusercontent.com/KewrrXNwxmDilSKPDNPEuyNiwT9yWWA9Rr0VwDfh4fE2zwaU2xvGG9XfOSKvzigwHvmfPzfzzvQ9a9QkRqpRVo6N9txAlcUm-p7v2XUIaCiVxedcquX4CL1W9cyej3DeXxBq7AQ)

                                             Slate product sub-category homepage

![](https://lh4.googleusercontent.com/cu7Ktdc0CzFibZaXUtU6VEe11WFCGKHyF2pBSGF4i1WpqPEbINKwx3FWpJgO6dGSrV9oS-gaWqBKs_i8TWC0LXH3BxbRPZEfT2lAdFMWmVer62O7JLahG_Bdw-uPP_SQOj9gYsw)

                                                    Slate API Reference

The new documentation platform was built with [slate](https://github.com/slatedocs/slate), a Ruby-based tool that generates a great-looking, three-panelled API documentation static site from a set of markdown files.

**To improve our documentation, Slate was chosen for the following reasons:**

1.  **Open Source** - In a bid to promote open source movement, Interswitch has been adopting the use of some open source tools and our documentation platform is one of them.

2.  **Flexibility** - Slate's  flexibility gave us the freedom to build what we wanted without starting from scratch. Due to the flexibility of slate, we were able to transform it from its original single page three-panelled API documentation static site to a multi page site with a homepage for all products categories. Each product has its own homepage for product subcategories where necessary, get started guides, and comprehensive API references e.t.c.![](https://lh3.googleusercontent.com/RDfou2O9jK09D5aCdgi89JH7C6n5nTLCz00LVc_ruEpyJr9q4MkJqeJdJ8tcyltEGaoPa3KLNaU68Yjpw4ptrl9EbxnXDJRvrcScTk8JNdtVm8SqTFIg9Xy6qTfIWiG9O0GWERM)

                           ***Slate original single page three-panelled API documentation static site***

1.  When you write docs with Slate, you're just writing Markdown, which makes it simple to edit and understand. 

2.  Slate provides an out-of-the-box syntax highlighting for [over 100 languages](https://github.com/jneen/rouge/wiki/List-of-supported-languages-and-lexers) with no configuration required.

3.  It could be hosted in a public GitHub repository which will make it simple for other developers to make pull requests to the docs if they find typos or want to make suggestions. Interswitch engineering has plans to Open Source it's documentation in the nearest future so that people could have the freedom to report issues and also work on it directly.

Even though Slate offered great features, we knew that we needed to put some internal processes in place to ensure that it doesn't end up like our previous API documentation. To achieve this, the developer relations team assumed the documentation team position and we also ensured that  for every API that is built or modified and pushed to production, a corresponding API Reference must be updated on slate and pushed for review to the documentation team for review.

## Additional Features

The developer relations team seeks to bridge the gap between our external and internal developers to ensure that the integration process of our APIs becomes seamless. Here are some other things we've done to ensure that the aforementioned goals come to reality. 

1.  [Developer Forum](https://discord.gg/ATRq54) - We created a [forum](https://discord.gg/) that will connect our internal and external developers thereby giving them a place to easily interact, make feature requests, report bugs, suggest edits on documentation, carry out beta testing, etc.

2.  [Developer Console](https://developer.interswitchgroup.com/) - The new developer console provides self-service integration, giving you the ability to access Interswitch product APIs, authentication parameters, Sandbox keys, production keys, documentation and seamless project management.

3.  **Admin Dashboard** - A dashboard that will be managed internally and used to manage APIs on the developer console. Requests from the developer console would also be handled seamlessly on the admin dashboard.

## Conclusion

We might not be where we want to be yet but at Interswitch engineering, we believe that we've taken a bold first step in the right direction to give our developers the better and seamless integration experience they deserve. We are excited about how much we've been able to achieve this past financial year. It's the beginning of a new financial year and we intend to top the last so stay tuned.
