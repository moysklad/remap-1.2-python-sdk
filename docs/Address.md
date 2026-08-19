# Address

Адрес

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**add_info** | **str** | Другое | [optional] 
**apartment** | **str** | Квартира | [optional] 
**city** | **str** | Город | [optional] 
**comment** | **str** | Комментарий | [optional] 
**country** | [**Country**](Country.md) |  | [optional] 
**house** | **str** | Дом | [optional] 
**postal_code** | **str** | Почтовый индекс | [optional] 
**region** | [**Region**](Region.md) |  | [optional] 
**street** | **str** | Улица | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.address import Address

# TODO update the JSON string below
json = "{}"
# create an instance of Address from a JSON string
address_instance = Address.from_json(json)
# print the JSON string representation of the object
print(Address.to_json())

# convert the object into a dict
address_dict = address_instance.to_dict()
# create an instance of Address from a dict
address_from_dict = Address.from_dict(address_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


