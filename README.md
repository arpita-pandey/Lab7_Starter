1) Where would you fit your automated tests in your Recipe project development pipeline?

Within a GitHub Action that runs whenever code is pushed. This is the best place because the tests run automatically and consistently for every change, which helps catch bugs early and prevents broken code from piling up. It is more reliable than depending on developers to remember to run tests manually, and it is much safer than waiting until all development is finished.

2) Would you use an end to end test to check if a function is returning the correct output? (yes/no)

No. End to end tests are meant to verify full user workflows through the interface, not to check the correctness of one small function in isolation. A unit test would be the better choice for testing whether a function returns the correct output.

3) What is the difference between navigation and snapshot mode?

Navigation mode analyzes a page as it loads from the beginning and measures overall load performance, accessibility, best practices, and SEO during that page load process. Snapshot mode analyzes the page only in its current state at a single moment, which makes it useful for checking things like accessibility issues but not for measuring page load behavior or JavaScript execution over time. 
4) Name three things we could do to improve the CSE 110 shop site based on the Lighthouse results.

Based on the Lighthouse report, one improvement would be to minify the JavaScript, since Lighthouse estimated about 58 KiB of savings there. Another would be to reduce unused JavaScript, which was the biggest issue and showed an estimated savings of about 3,151 KiB. A third improvement would be to reduce render blocking requests and heavy main thread work, since the report showed a Total Blocking Time of 540 ms and a Max Potential First Input Delay of 350 ms.
