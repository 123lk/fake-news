# Fake News Mission Statement

Our mission, now that we've chosen to accept it, is as follows:

We want to design and build the hub for a community of dilligent fact checkers. It will be used to expose falsitities, address bias and show ownership models of newspapers and websites. In order to succeed in this mission, the information that our community contributes must be accessible not just on the site, but anywhere in the browser, exposing links and tweets with contentious or downright false origins, and drawing attention to trustworthy sources. 

In order to achieve this, there is a need for three main components: 

- The website. This is a wikipedia style site with pages (initially) for newspapers and sites, which accumulate scores (positive or negative) over time. Although contributers will be able to directly comment, cross-reference and fact check articles, these articles will not have scores of their own due to the speed of the news-cycle. The article scores will feed into the overall score for the website. As well as community of contributers, there will also be trusted contributers, who effectively serve as moderators. This will be built primarily in react, redux and bulma. 

- The database. This will primarily be built in SQL, and eventually hosted on AWS. It will need to use password authentication in order to allow moderators and contributers to log in. Only users with accounts will be able to contribute. This will also store the algorithm for assessing the reliability of news sources, and will serve up all of the stored information to the website on request, and some to the chrome app.

- The Chrome app. Any user will be able to install the chrome app from the chrome web store. This will need to trawl the DOM, find links to news sites and stories and, if it recognises any of the domains, will render a css flag (red, amber or green) next to the link. 

