# TaxRate

Ставка НДС

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID налоговой ставки | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**owner** | [**Employee**](Employee.md) | Метаданные владельца (Сотрудника) | [optional] 
**shared** | **bool** | Флаг общего доступа | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**updated** | **str** | Момент последнего обновления сущности | [optional] [readonly] 
**rate** | **float** | Значение налоговой ставки | [optional] 
**archived** | **bool** | Флаг принадлежности ставки к архивным ставкам | [optional] 
**comment** | **str** | Комментарий к налоговой ставке | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.tax_rate import TaxRate

# TODO update the JSON string below
json = "{}"
# create an instance of TaxRate from a JSON string
tax_rate_instance = TaxRate.from_json(json)
# print the JSON string representation of the object
print(TaxRate.to_json())

# convert the object into a dict
tax_rate_dict = tax_rate_instance.to_dict()
# create an instance of TaxRate from a dict
tax_rate_from_dict = TaxRate.from_dict(tax_rate_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


