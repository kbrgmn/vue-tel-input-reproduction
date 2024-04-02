# vue-tel-input issue #452

Error message:
```
Uncaught (in promise) Maximum recursive updates exceeded in component <app>.
This means you have a reactive effect that is mutating its own dependencies and thus recursively triggering itself.
Possible sources include component template, render function, updated hook or watcher source function.
```


- Running in dev mode `bun dev`: Cancels any input after auto format has run
- Running in prod mode `bun run build && node .output/server/index.mjs`: Slows down page until it crashes
