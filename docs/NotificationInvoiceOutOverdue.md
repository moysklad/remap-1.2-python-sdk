# NotificationInvoiceOutOverdue

Уведомление о просроченном счете покупателя

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**agent_name** | **str** | Имя контрагента | [optional] 
**invoice** | [**NotificationInvoice**](NotificationInvoice.md) |  | [optional] 
**payment_planned_moment** | **str** | Запланированная дата оплаты | [optional] 
**sum** | **int** | Сумма счета | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.notification_invoice_out_overdue import NotificationInvoiceOutOverdue

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationInvoiceOutOverdue from a JSON string
notification_invoice_out_overdue_instance = NotificationInvoiceOutOverdue.from_json(json)
# print the JSON string representation of the object
print(NotificationInvoiceOutOverdue.to_json())

# convert the object into a dict
notification_invoice_out_overdue_dict = notification_invoice_out_overdue_instance.to_dict()
# create an instance of NotificationInvoiceOutOverdue from a dict
notification_invoice_out_overdue_from_dict = NotificationInvoiceOutOverdue.from_dict(notification_invoice_out_overdue_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


