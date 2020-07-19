# Day 3
So - I didn't get a lot done on this day - in fact I wrestled with `mdsvex` for a long while, both in new sapper templates using rollup and webpack and having various amounts of defeat. I posted an issue about the new project install/setup docs - it's obvious the problem is on my end with my lack of knowledge of both rollup and webpack, not with `mdsvex` and some kind helpful soul got me a bit closer, but I'm still having errors so I think I'll put that on hold for now.

What I did so was open up the `cypress` stuff and start poking at it. [cypress](https://www.cypress.io/) is really great and pretty easy to pick up - I was able to throw together a quick change in the test spec to have it test my front page (well, not 'test' so much as ensure that the text is showing up and it's got a dialtone)

### cypress\integration\spec.js
```diff
  it('has the correct <h1>', () => {
-    cy.contains('h1', 'Great Success!');
+    cy.contains('h1', 'Paul\'s Blog Site');
  });
```



