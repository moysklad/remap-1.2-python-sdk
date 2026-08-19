# RetailStoreReceiptTemplate

Шаблон чека

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**header** | **str** |  | [optional] 
**footer** | **str** |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.retail_store_receipt_template import RetailStoreReceiptTemplate

# TODO update the JSON string below
json = "{}"
# create an instance of RetailStoreReceiptTemplate from a JSON string
retail_store_receipt_template_instance = RetailStoreReceiptTemplate.from_json(json)
# print the JSON string representation of the object
print(RetailStoreReceiptTemplate.to_json())

# convert the object into a dict
retail_store_receipt_template_dict = retail_store_receipt_template_instance.to_dict()
# create an instance of RetailStoreReceiptTemplate from a dict
retail_store_receipt_template_from_dict = RetailStoreReceiptTemplate.from_dict(retail_store_receipt_template_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


