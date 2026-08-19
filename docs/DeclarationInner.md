# DeclarationInner

Запись о прослеживаемости импортных товаров

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**gtd** | **str** | Грузовая таможенная декларация | [optional] [readonly] 
**rnpt** | **str** | Регистрационный номер партии товара (прослеживаемый товар) | [optional] [readonly] 
**country** | [**Country**](Country.md) | Страна происхождения товара | [optional] [readonly] 
**quantity** | **float** | Количество товара с указанными ГТД или РНПТ в позиции документа | [optional] [readonly] 

## Example

```python
from moysklad_remap_12_sdk.models.declaration_inner import DeclarationInner

# TODO update the JSON string below
json = "{}"
# create an instance of DeclarationInner from a JSON string
declaration_inner_instance = DeclarationInner.from_json(json)
# print the JSON string representation of the object
print(DeclarationInner.to_json())

# convert the object into a dict
declaration_inner_dict = declaration_inner_instance.to_dict()
# create an instance of DeclarationInner from a dict
declaration_inner_from_dict = DeclarationInner.from_dict(declaration_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


