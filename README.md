## Measuring web performance

Multiple tools with their own metrics.

**Metrics**

Almost every metric is made up, they are not standardized and could be ambiguous.

- The page has displayed useful content, which is measured with First Contentful Paint (FCP).
- First Meaningful Paint (FMP) measures when the primary content of a page is visible to the user.
- The Time to Interactive (TTI) metric measures how long it takes a page to become interactive.
- More: https://web.dev/lighthouse-performance/

**Tools**

WebpageTest 
https://webpagetest.org/
and Lighthouse

**Lighthouse**

3 ways to use it: 
- Pagespeed insights - https://developers.google.com/speed/pagespeed/insights/
- Chrome devtools
- CLI - https://www.npmjs.com/package/lighthouse

They are using different versions of Lighthouse, could give you different results

It can report 5 different categories: Performance, PWA, Best practices, Accessibility, SEO

- The results are just suggestions, take them with a grain of salt, not always gives you better results
- Depends on a lots of things (computer, location, network) -> giving a different result every time
- Performance scoring: https://web.dev/performance-scoring/

***Tips how to use:***
- It depends on your user/ your chrome extensions -> best to use them in incognito mode
- If you are looking for improvements in our sites, best to use the `no3rdparty` feature switch to eliminate 3rd party resources and measure only our code
- You can download your report as HTML/JSON to share it

**JS Performance**

- Gives you a flame chart
- Look for long tasks that are holding the main thread and lower fps, indicated with a red corner mark
- You can also save and load these charts as JSON

**Code coverage**

- Almost every article about performance starts with a tip to delete unused code to improve your website performance
- Lists every resource with a percentage
- You can even see not used lines if you open one file
