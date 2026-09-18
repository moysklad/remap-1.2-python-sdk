# AuditEvent

Событие аудита

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**additional_info** | **str** | Дополнительная информация о событии | [optional] [readonly] 
**audit** | [**AuditEventAudit**](AuditEventAudit.md) |  | [optional] 
**diff** | **Dict[str, object]** | Изменения, произошедшие в событии | [optional] [readonly] 
**entity** | [**AuditEventEntity**](AuditEventEntity.md) |  | [optional] 
**entity_type** | **str** | Тип сущности | [optional] [readonly] 
**event_type** | **str** | Действие события. Известные значения описаны в AuditEventType | [optional] [readonly] 
**moment** | **str** | Время создания события | [optional] [readonly] 
**name** | **str** | Имя сущности | [optional] [readonly] 
**object_count** | **int** | Количество измененных объектов | [optional] [readonly] 
**object_type** | **str** | Тип сущностей для специальных настроечных событий | [optional] [readonly] 
**source** | **str** | Источник изменения. Известные значения описаны в AuditSourceType | [optional] [readonly] 
**support_access** | **bool** | Признак доступа поддержки от имени пользователя | [optional] [readonly] 
**uid** | **str** | Логин сотрудника | [optional] [readonly] 

## Example

```python
from moysklad_remap_12_sdk.models.audit_event import AuditEvent

# TODO update the JSON string below
json = "{}"
# create an instance of AuditEvent from a JSON string
audit_event_instance = AuditEvent.from_json(json)
# print the JSON string representation of the object
print(AuditEvent.to_json())

# convert the object into a dict
audit_event_dict = audit_event_instance.to_dict()
# create an instance of AuditEvent from a dict
audit_event_from_dict = AuditEvent.from_dict(audit_event_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


