# NotificationInvoice

Краткое представление счета покупателю в уведомлении

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID объекта | [optional] 
**name** | **str** | Наименование объекта | [optional] 
**payment_planned_moment** | **str** | Запланированная дата оплаты | [optional] 
**sum** | **int** | Сумма счета | [optional] 
**customer_name** | **str** | Имя покупателя | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.notification_invoice import NotificationInvoice

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationInvoice from a JSON string
notification_invoice_instance = NotificationInvoice.from_json(json)
# print the JSON string representation of the object
print(NotificationInvoice.to_json())

# convert the object into a dict
notification_invoice_dict = notification_invoice_instance.to_dict()
# create an instance of NotificationInvoice from a dict
notification_invoice_from_dict = NotificationInvoice.from_dict(notification_invoice_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


