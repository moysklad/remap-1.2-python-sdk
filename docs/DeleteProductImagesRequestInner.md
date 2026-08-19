# DeleteProductImagesRequestInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.delete_product_images_request_inner import DeleteProductImagesRequestInner

# TODO update the JSON string below
json = "{}"
# create an instance of DeleteProductImagesRequestInner from a JSON string
delete_product_images_request_inner_instance = DeleteProductImagesRequestInner.from_json(json)
# print the JSON string representation of the object
print(DeleteProductImagesRequestInner.to_json())

# convert the object into a dict
delete_product_images_request_inner_dict = delete_product_images_request_inner_instance.to_dict()
# create an instance of DeleteProductImagesRequestInner from a dict
delete_product_images_request_inner_from_dict = DeleteProductImagesRequestInner.from_dict(delete_product_images_request_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


