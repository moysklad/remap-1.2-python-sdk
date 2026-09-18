# AuditFilters

Доступные значения фильтров аудита

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**source** | [**List[AuditSourceType]**](AuditSourceType.md) | Источники изменений, доступные для фильтрации | [optional] 
**entitytype** | **List[str]** | Типы сущностей, доступные для фильтрации | [optional] 
**eventtype** | [**List[AuditEventType]**](AuditEventType.md) | Типы событий, доступные для фильтрации | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.audit_filters import AuditFilters

# TODO update the JSON string below
json = "{}"
# create an instance of AuditFilters from a JSON string
audit_filters_instance = AuditFilters.from_json(json)
# print the JSON string representation of the object
print(AuditFilters.to_json())

# convert the object into a dict
audit_filters_dict = audit_filters_instance.to_dict()
# create an instance of AuditFilters from a dict
audit_filters_from_dict = AuditFilters.from_dict(audit_filters_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


