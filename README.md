# Intune Device Query Examples

##Find local user
```
LocalUserAccount
| where WindowsSid contains 'S-1-5'
```
