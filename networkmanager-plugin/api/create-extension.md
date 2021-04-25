# Create extension

## Java

```java
public class ExtensionExample extends NMExtension {
    
    @Override
    public void onEnable() {
        
    }
    
    @Override
    public void onDisable() {
    
    }
    
    @Override
    public void onConfigReload() {
    
    }
}
```

{% hint style="info" %}
If you want to check which type of platform the extension is running on you can use: getNetworkManager\(\).getPlatformType\(\). Example: getNetworkManager\(\).getPlatformType\(\) == PlatformType.BUKKIT
{% endhint %}

## Kotlin

```kotlin
class ExtensionExample : NMExtension {

    override fun onEnable() {
    
    }
    
    override fun onDisable() {
    
    }
    
    override fun onConfigReload() {
    
    }
}
```

{% hint style="info" %}
If you want to check which type of platform the extension is running on you can use: networkManager.platformType. Example: networkManager.platformType === PlatformType.BUKKIT
{% endhint %}

