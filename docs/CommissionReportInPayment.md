# CommissionReportInPayment

Элемент массива `payments` документа commissionReportIn. Ссылка или раскрытый платеж; `linkedSum` может отсутствовать. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | 
**linked_sum** | **float** | Сумма, оплаченная по данному документу; может отсутствовать у ссылки | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.commission_report_in_payment import CommissionReportInPayment

# TODO update the JSON string below
json = "{}"
# create an instance of CommissionReportInPayment from a JSON string
commission_report_in_payment_instance = CommissionReportInPayment.from_json(json)
# print the JSON string representation of the object
print(CommissionReportInPayment.to_json())

# convert the object into a dict
commission_report_in_payment_dict = commission_report_in_payment_instance.to_dict()
# create an instance of CommissionReportInPayment from a dict
commission_report_in_payment_from_dict = CommissionReportInPayment.from_dict(commission_report_in_payment_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


