# Account

Счета контрагентов/юрлиц

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID счета | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**updated** | **str** | Время последнего изменения | [optional] [readonly] 
**is_default** | **bool** | Основной счет | [optional] 
**account_number** | **str** | Номер счета | [optional] 
**bank_name** | **str** | Наименование банка | [optional] 
**bank_location** | **str** | Адрес банка | [optional] 
**correspondent_account** | **str** | Корр. счет | [optional] 
**bic** | **str** | БИК | [optional] 
**currency** | [**Currency**](Currency.md) | Метаданные валюты расчетного счета юрлица | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.account import Account

# TODO update the JSON string below
json = "{}"
# create an instance of Account from a JSON string
account_instance = Account.from_json(json)
# print the JSON string representation of the object
print(Account.to_json())

# convert the object into a dict
account_dict = account_instance.to_dict()
# create an instance of Account from a dict
account_from_dict = Account.from_dict(account_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


