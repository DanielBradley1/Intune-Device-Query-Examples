# Intune Device Query Examples

## Find local users
```
LocalUserAccount
| where WindowsSid contains 'S-1-5'
```
