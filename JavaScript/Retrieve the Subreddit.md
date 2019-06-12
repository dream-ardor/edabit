## Retrieve the Subreddit

Create a function to extract the name of the subreddit from its URL.
```js
Examples:
subReddit("https://www.reddit.com/r/funny/") ➞ "funny"

subReddit("https://www.reddit.com/r/relationships/") ➞ "relationships"

subReddit("https://www.reddit.com/r/mildlyinteresting/") ➞ "mildlyinteresting
```

## My Code
```js
const subReddit = link => link.split("/")[4]

```
