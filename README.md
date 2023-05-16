# How to reproduce

```
npm install
npm start
```

Then in second terminal

```
npx playwright codegen http://localhost:3040/
```

In playwright browser turn on developer tools and click console.

Then click the cross.

It will result in this error in the console:

```
t (in promise) TypeError: Cannot read properties of undefined (reading 'includes')
    at parseSelectorString (<anonymous>:1422:17)
    at parseSelector (<anonymous>:1322:18)
    at InjectedScript.parseSelector (<anonymous>:4440:20)
    at makeStrict (eval at extend (localhost/:4673:40), <anonymous>:1017:43)
    at cssFallback (eval at extend (localhost/:4673:40), <anonymous>:1061:10)
    at generateSelector (eval at extend (localhost/:4673:40), <anonymous>:826:40)
    at Recorder._updateModelForHoveredElement (eval at extend (localhost/:4673:40), <anonymous>:3404:36)
    at Recorder._onFocus (eval at extend (localhost/:4673:40), <anonymous>:3395:10)
    at Recorder._performAction (eval at extend (localhost/:4673:40), <anonymous>:3531:10)
parseSelectorSt
```
