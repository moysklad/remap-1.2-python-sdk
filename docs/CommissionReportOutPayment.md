# CommissionReportOutPayment

Элемент массива `payments` документа commissionReportOut. Ссылка или раскрытый платеж; `linkedSum` может отсутствовать. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | 
**linked_sum** | **float** | Сумма, оплаченная по данному документу; может отсутствовать у ссылки | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.commission_report_out_payment import CommissionReportOutPayment

# TODO update the JSON string below
json = "{}"
# create an instance of CommissionReportOutPayment from a JSON string
commission_report_out_payment_instance = CommissionReportOutPayment.from_json(json)
# print the JSON string representation of the object
print(CommissionReportOutPayment.to_json())

# convert the object into a dict
commission_report_out_payment_dict = commission_report_out_payment_instance.to_dict()
# create an instance of CommissionReportOutPayment from a dict
commission_report_out_payment_from_dict = CommissionReportOutPayment.from_dict(commission_report_out_payment_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


