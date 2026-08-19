# AttributeMetaInfoList

Доп.поля

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[AttributeMetaInfo]**](AttributeMetaInfo.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.attribute_meta_info_list import AttributeMetaInfoList

# TODO update the JSON string below
json = "{}"
# create an instance of AttributeMetaInfoList from a JSON string
attribute_meta_info_list_instance = AttributeMetaInfoList.from_json(json)
# print the JSON string representation of the object
print(AttributeMetaInfoList.to_json())

# convert the object into a dict
attribute_meta_info_list_dict = attribute_meta_info_list_instance.to_dict()
# create an instance of AttributeMetaInfoList from a dict
attribute_meta_info_list_from_dict = AttributeMetaInfoList.from_dict(attribute_meta_info_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


