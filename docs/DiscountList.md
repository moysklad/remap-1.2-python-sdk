# DiscountList

Список Скидок

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[DiscountAbstract]**](DiscountAbstract.md) | Массив скидок всех типов для учётной записи (см. &#x60;meta.type&#x60;: discount, personaldiscount, specialpricediscount, accumulationdiscount, bonusprogram).  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.discount_list import DiscountList

# TODO update the JSON string below
json = "{}"
# create an instance of DiscountList from a JSON string
discount_list_instance = DiscountList.from_json(json)
# print the JSON string representation of the object
print(DiscountList.to_json())

# convert the object into a dict
discount_list_dict = discount_list_instance.to_dict()
# create an instance of DiscountList from a dict
discount_list_from_dict = DiscountList.from_dict(discount_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


