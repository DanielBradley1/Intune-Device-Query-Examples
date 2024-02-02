# Intune Device Query Examples

### Find local users
```
LocalUserAccount
| where WindowsSid contains 'S-1-5'
```

### Query local disk TPM and encryption
```
EncryptableVolume
| join Tpm 
| project WindowsDriveLetter, ProtectionStatus, EncryptionMethod, EncryptionPercentage, Activated, Enabled, SpecVersion, Manufacturer
```
