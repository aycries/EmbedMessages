# Config options
This plugin was written with customizability in mind, thus there are a lot of config options.
Below you can find the default options:
```ini
    em.staffReplyDmEnabled = on
    em.staffReplyDmColor = "#2F3136"

    em.staffReplyThreadEnabled = on
    em.staffReplyThreadColor = "#2F3136"
    em.staffReplyDmTimestampEnabled = on

    em.userReplyThreadEnabled = on
    em.userReplyThreadColor = "#2F3136"

    em.systemReplyDmEnabled = on
    em.systemReplyDmColor = "#2F3136"

    em.systemReplyThreadEnabled = on
    em.systemReplyThreadColor = "#2F3136"

    em.systemStaffEnabled = on
    em.systemStaffColor = "#2F3136"

    # Miscellaneous Settings
    em.systemName = "System"
```
If you want to change an option, simply copy and paste the corresponding line into your config and change the value.

# Valid values
## Toggles
Any setting that ends in `Enabled` is a toggle.  
Like regular on/off settings, these take any truthy or falsy values.  
Truthy: `on`, `1`, `true`  
Falsy: `off`, `0`, `false`, `null`

## Colors
Any option that ends in `Color` takes a color value.  
Valid color formats are:
- HEX (e.g. "#7289DA") | These must start with a `#` and be in quotes
- RGB (e.g. 114, 137, 218) | Any three numbers delimited with any non-number  
  
## Miscellaneous Settings
These all accept different values. All misc. settings and their types are listed here:
### systemName
This accepts any string. Said string will then be used in the embed instead of `System` when a system message is sent.  
Setting this to `$botname` will automatically use the Bots username (as it was when the plugin was loaded - later changes are not reflected until the bot restarts).
