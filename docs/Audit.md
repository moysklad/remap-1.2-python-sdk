# Audit

Контекст аудита

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID контекста аудита | [optional] [readonly] 
**uid** | **str** | Логин сотрудника | [optional] [readonly] 
**source** | **str** | Источник изменения. Известные значения описаны в AuditSourceType | [optional] [readonly] 
**moment** | **str** | Момент изменения | [optional] [readonly] 
**info** | **Dict[str, object]** | Краткое описание контекста | [optional] [readonly] 
**object_count** | **int** | Количество измененных объектов | [optional] [readonly] 
**event_type** | **str** | Тип события. Известные значения описаны в AuditEventType | [optional] [readonly] 
**entity_type** | **str** | Тип сущности | [optional] [readonly] 
**object_type** | **str** | Тип сущностей для специальных настроечных контекстов | [optional] [readonly] 
**support_access** | **bool** | Признак доступа поддержки от имени пользователя | [optional] [readonly] 
**events** | [**AuditEvents**](AuditEvents.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.audit import Audit

# TODO update the JSON string below
json = "{}"
# create an instance of Audit from a JSON string
audit_instance = Audit.from_json(json)
# print the JSON string representation of the object
print(Audit.to_json())

# convert the object into a dict
audit_dict = audit_instance.to_dict()
# create an instance of Audit from a dict
audit_from_dict = Audit.from_dict(audit_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


