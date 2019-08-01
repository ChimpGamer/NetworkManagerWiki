# Add PlaceholderHook

Through the API you can add PlaceholderHooks in NetworkManager. You'll have to expand your class with the PlaceholderHook class and it should look like this:

```java
public PlaceholderHookExample expands PlaceholderHook {
    
    @Override
    public String onPlaceholderRequest(String identifier) {
        if (identifier.equalsIgnorecases("test")) {
            return "ExampleValue"; //So if the placeholder %example_test% get's requested it will return this.
        }
    }
    
    @Override
    public String getIdentifier() {
        return "example";
    }
}
```

Then you'll have to register it by using NetworkManager\#getPlaceholderManager\#registerPlaceholder which returns a boolean value. If it return's true the Placeholder got successully registered. If false, you should check the server console to find out what's wrong.

