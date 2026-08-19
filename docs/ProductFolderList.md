# ProductFolderList

Список группы товаров

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[ProductFolder]**](ProductFolder.md) | Массив группы товаров | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.product_folder_list import ProductFolderList

# TODO update the JSON string below
json = "{}"
# create an instance of ProductFolderList from a JSON string
product_folder_list_instance = ProductFolderList.from_json(json)
# print the JSON string representation of the object
print(ProductFolderList.to_json())

# convert the object into a dict
product_folder_list_dict = product_folder_list_instance.to_dict()
# create an instance of ProductFolderList from a dict
product_folder_list_from_dict = ProductFolderList.from_dict(product_folder_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


