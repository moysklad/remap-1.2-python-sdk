# GetVariantCharacteristics200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**rows** | [**List[VariantCharacteristic]**](VariantCharacteristic.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.get_variant_characteristics200_response import GetVariantCharacteristics200Response

# TODO update the JSON string below
json = "{}"
# create an instance of GetVariantCharacteristics200Response from a JSON string
get_variant_characteristics200_response_instance = GetVariantCharacteristics200Response.from_json(json)
# print the JSON string representation of the object
print(GetVariantCharacteristics200Response.to_json())

# convert the object into a dict
get_variant_characteristics200_response_dict = get_variant_characteristics200_response_instance.to_dict()
# create an instance of GetVariantCharacteristics200Response from a dict
get_variant_characteristics200_response_from_dict = GetVariantCharacteristics200Response.from_dict(get_variant_characteristics200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


