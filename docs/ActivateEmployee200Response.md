# ActivateEmployee200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**mail_activation_required** | **bool** | Признак того, что на почту сотрудника выслано письмо для активации | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.activate_employee200_response import ActivateEmployee200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ActivateEmployee200Response from a JSON string
activate_employee200_response_instance = ActivateEmployee200Response.from_json(json)
# print the JSON string representation of the object
print(ActivateEmployee200Response.to_json())

# convert the object into a dict
activate_employee200_response_dict = activate_employee200_response_instance.to_dict()
# create an instance of ActivateEmployee200Response from a dict
activate_employee200_response_from_dict = ActivateEmployee200Response.from_dict(activate_employee200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


