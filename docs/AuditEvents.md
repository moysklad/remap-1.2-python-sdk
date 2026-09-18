# AuditEvents

Метаданные списка связанных событий аудита

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**MetaList**](MetaList.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.audit_events import AuditEvents

# TODO update the JSON string below
json = "{}"
# create an instance of AuditEvents from a JSON string
audit_events_instance = AuditEvents.from_json(json)
# print the JSON string representation of the object
print(AuditEvents.to_json())

# convert the object into a dict
audit_events_dict = audit_events_instance.to_dict()
# create an instance of AuditEvents from a dict
audit_events_from_dict = AuditEvents.from_dict(audit_events_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


