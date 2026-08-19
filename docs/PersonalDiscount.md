# PersonalDiscount


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | ID дополнительного поля | [optional] [readonly] 
**meta** | [**Meta**](Meta.md) |  | [optional] 
**product_folders** | [**List[ProductFolder]**](ProductFolder.md) | Группы товаров со скидкой | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.personal_discount import PersonalDiscount

# TODO update the JSON string below
json = "{}"
# create an instance of PersonalDiscount from a JSON string
personal_discount_instance = PersonalDiscount.from_json(json)
# print the JSON string representation of the object
print(PersonalDiscount.to_json())

# convert the object into a dict
personal_discount_dict = personal_discount_instance.to_dict()
# create an instance of PersonalDiscount from a dict
personal_discount_from_dict = PersonalDiscount.from_dict(personal_discount_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


