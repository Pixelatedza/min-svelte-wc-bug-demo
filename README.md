Minimal reproduction of svelte custom components not being cleaned up fully.

Run svelte normally (vite-project directory) `yarn dev`. Then, open the index.html in the root directory in your browser.

#### To replicate the bug:
- click "toggle content" repeatedly. If the content has shown up a second time, this is enough. This can be repeated indefinitely though.
- click "change store value", the store will update and print it's value. The value will be printed **n** timse. **n** being the amount of times the content was shown.
