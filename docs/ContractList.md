# ContractList

Список договоров

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[Contract]**](Contract.md) | Массив договоров | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.contract_list import ContractList

# TODO update the JSON string below
json = "{}"
# create an instance of ContractList from a JSON string
contract_list_instance = ContractList.from_json(json)
# print the JSON string representation of the object
print(ContractList.to_json())

# convert the object into a dict
contract_list_dict = contract_list_instance.to_dict()
# create an instance of ContractList from a dict
contract_list_from_dict = ContractList.from_dict(contract_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


