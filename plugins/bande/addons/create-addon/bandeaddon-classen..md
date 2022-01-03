# BandeAddon classen.

{% code title="BandeAddon.java" %}
```java
public abstract class BandeAddon {
    
    // Bliver callet når et addon bliver disabled.
    public void onDisable(){};

    // Bliver callet når et addon bliver enabled.
    public void onEnable(){};

    // Bliver callet når et addon bliver reloaded.
    public void onReload(){};
    

    // Disable / Enable et addon
    public void setEnabled(boolean enabled){};
    
    // Returner om addonet er enabled.
    public boolean isEnabled(){};
    
    // Returner en addon.yml som class.
    public AddonDescriptionFile getDescription(){};

    // Returner instancen af Bande pluginet.
    public JavaPlugin getMainPlugin(){}

    // Returner Bande pluginets logget.
    public Logger getLogger();
    
    // Returner Addons Data Folder.
    // plugins/Bande/addons/ExampleAddon/
    public File getAddonFolder();

    // Gemmer en fil der ligger i Addons Resource Mappe.
    public void saveResource(String resourcePath, boolean replace) {}
    
}

```
{% endcode %}
