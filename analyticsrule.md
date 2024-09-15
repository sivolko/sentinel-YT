# AnalyticsRule

To find successful sign in&#x20;

```
// KQL code

SecurityEvent
| where Activity contains "success" and Account !contains "system" 
| project Account , Activity, Computer, TimeGenerated, EventID, IpAddress
```

MITRE ATT\&CK InitialAccess Initial Access



