# Prepayment

Предоплата

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Предоплаты | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**name** | **str** | Наименование Предоплаты | [optional] 
**code** | **str** | Код Предоплаты | [optional] 
**external_code** | **str** | Внешний код Предоплаты | [optional] 
**sync_id** | **str** | ID синхронизации | [optional] 
**description** | **str** | Комментарий Предоплаты | [optional] 
**created** | **str** | Дата создания | [optional] [readonly] 
**deleted** | **str** | Момент последнего удаления Предоплаты | [optional] [readonly] 
**updated** | **str** | Момент последнего обновления Предоплаты | [optional] [readonly] 
**moment** | **str** | Дата документа | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.prepayment import Prepayment

# TODO update the JSON string below
json = "{}"
# create an instance of Prepayment from a JSON string
prepayment_instance = Prepayment.from_json(json)
# print the JSON string representation of the object
print(Prepayment.to_json())

# convert the object into a dict
prepayment_dict = prepayment_instance.to_dict()
# create an instance of Prepayment from a dict
prepayment_from_dict = Prepayment.from_dict(prepayment_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


