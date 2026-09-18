# AuditEventAudit

Метаданные контекста аудита

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.audit_event_audit import AuditEventAudit

# TODO update the JSON string below
json = "{}"
# create an instance of AuditEventAudit from a JSON string
audit_event_audit_instance = AuditEventAudit.from_json(json)
# print the JSON string representation of the object
print(AuditEventAudit.to_json())

# convert the object into a dict
audit_event_audit_dict = audit_event_audit_instance.to_dict()
# create an instance of AuditEventAudit from a dict
audit_event_audit_from_dict = AuditEventAudit.from_dict(audit_event_audit_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


