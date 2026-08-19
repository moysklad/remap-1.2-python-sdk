# ProductAlcoholic

Объект, содержащий поля алкогольной продукции

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**excise** | **bool** | Содержит акцизную марку | [optional] 
**type** | **int** | Код вида продукции | [optional] 
**strength** | **float** | Крепость | [optional] 
**volume** | **float** | Объём тары | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.product_alcoholic import ProductAlcoholic

# TODO update the JSON string below
json = "{}"
# create an instance of ProductAlcoholic from a JSON string
product_alcoholic_instance = ProductAlcoholic.from_json(json)
# print the JSON string representation of the object
print(ProductAlcoholic.to_json())

# convert the object into a dict
product_alcoholic_dict = product_alcoholic_instance.to_dict()
# create an instance of ProductAlcoholic from a dict
product_alcoholic_from_dict = ProductAlcoholic.from_dict(product_alcoholic_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


