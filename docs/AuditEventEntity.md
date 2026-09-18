# AuditEventEntity

Метаданные сущности, в которой произошло изменение

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.audit_event_entity import AuditEventEntity

# TODO update the JSON string below
json = "{}"
# create an instance of AuditEventEntity from a JSON string
audit_event_entity_instance = AuditEventEntity.from_json(json)
# print the JSON string representation of the object
print(AuditEventEntity.to_json())

# convert the object into a dict
audit_event_entity_dict = audit_event_entity_instance.to_dict()
# create an instance of AuditEventEntity from a dict
audit_event_entity_from_dict = AuditEventEntity.from_dict(audit_event_entity_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


