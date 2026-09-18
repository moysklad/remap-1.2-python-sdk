# AuditEventList

Список событий аудита

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[AuditEvent]**](AuditEvent.md) | Массив событий аудита | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.audit_event_list import AuditEventList

# TODO update the JSON string below
json = "{}"
# create an instance of AuditEventList from a JSON string
audit_event_list_instance = AuditEventList.from_json(json)
# print the JSON string representation of the object
print(AuditEventList.to_json())

# convert the object into a dict
audit_event_list_dict = audit_event_list_instance.to_dict()
# create an instance of AuditEventList from a dict
audit_event_list_from_dict = AuditEventList.from_dict(audit_event_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


