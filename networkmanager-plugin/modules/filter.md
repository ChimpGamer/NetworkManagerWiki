# Filter

The Filter module uses regex. Even if you don't apply it it will be used internal to find the matching word.

With regex you can make efficient rules to Filter words or sentences. For example:

```
\b(v(\W|\d|_)*a(\W|\d|_)*g(\W|\d|_)*i(\W|\d|_)*n(\W|\d|_)*a(\W|\d|_)*) # This will block vagina is a few ways.
   ^          ^          ^          ^          ^          ^
```

You can test your regex expressions at an online website like: [https://regexr.com/](https://regexr.com/)\
\
**Tip:** You can let the filter change <3 to ❤ by setting "<3/b" as word (without quotes)  and "&4❤\&r" as replacement (without quotes).

Want to share your regex expressions? Send me a messages on spigot or discord and I'll add them to this page with your name and explanation.

### Permissions

**Permission**: networkmanager.filter.bypass\
Allows you to bypass the filter.

**Permission**: networkmanager.antiswear.notify\
With this permission you get notified about swearing players



