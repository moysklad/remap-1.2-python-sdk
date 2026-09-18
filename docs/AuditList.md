# AuditList

Список контекстов аудита

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[Audit]**](Audit.md) | Массив контекстов аудита | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.audit_list import AuditList

# TODO update the JSON string below
json = "{}"
# create an instance of AuditList from a JSON string
audit_list_instance = AuditList.from_json(json)
# print the JSON string representation of the object
print(AuditList.to_json())

# convert the object into a dict
audit_list_dict = audit_list_instance.to_dict()
# create an instance of AuditList from a dict
audit_list_from_dict = AuditList.from_dict(audit_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


