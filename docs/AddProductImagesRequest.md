# AddProductImagesRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**filename** | **str** | Имя файла с расширением | 
**content** | **str** | Файл, закодированный в формате Base64 | 

## Example

```python
from moysklad_remap_12_sdk.models.add_product_images_request import AddProductImagesRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AddProductImagesRequest from a JSON string
add_product_images_request_instance = AddProductImagesRequest.from_json(json)
# print the JSON string representation of the object
print(AddProductImagesRequest.to_json())

# convert the object into a dict
add_product_images_request_dict = add_product_images_request_instance.to_dict()
# create an instance of AddProductImagesRequest from a dict
add_product_images_request_from_dict = AddProductImagesRequest.from_dict(add_product_images_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


