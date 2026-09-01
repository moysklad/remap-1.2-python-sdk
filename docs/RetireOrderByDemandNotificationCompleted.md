# RetireOrderByDemandNotificationCompleted

Уведомление о завершении создания выводов из оборота по отгрузкам

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**created_docs_count** | **int** | Количество созданных документов | [optional] 
**error_message** | **str** | Сообщение об ошибке | [optional] 
**message** | **str** | Сообщение о завершении операции | [optional] 
**task_state** | **str** | Статус завершения. Известные значения описаны в NotificationTaskState | [optional] 
**start_moment** | **str** | Дата и время начала создания документов | [optional] 
**end_moment** | **str** | Дата и время окончания создания документов | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.retire_order_by_demand_notification_completed import RetireOrderByDemandNotificationCompleted

# TODO update the JSON string below
json = "{}"
# create an instance of RetireOrderByDemandNotificationCompleted from a JSON string
retire_order_by_demand_notification_completed_instance = RetireOrderByDemandNotificationCompleted.from_json(json)
# print the JSON string representation of the object
print(RetireOrderByDemandNotificationCompleted.to_json())

# convert the object into a dict
retire_order_by_demand_notification_completed_dict = retire_order_by_demand_notification_completed_instance.to_dict()
# create an instance of RetireOrderByDemandNotificationCompleted from a dict
retire_order_by_demand_notification_completed_from_dict = RetireOrderByDemandNotificationCompleted.from_dict(retire_order_by_demand_notification_completed_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


