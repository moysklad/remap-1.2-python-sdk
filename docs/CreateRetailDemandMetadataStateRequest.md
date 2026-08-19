# CreateRetailDemandMetadataStateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID статуса | [optional] [readonly] 
**name** | **str** | Наименование статуса | [optional] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**color** | **int** | Цвет Статуса | [optional] 
**entity_type** | **str** | Тип сущности, к которой относится Статус (ключевое слово в рамках JSON API) | [optional] [readonly] 
**state_type** | **str** | Тип Статуса. Известные значения описаны в StateType | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.create_retail_demand_metadata_state_request import CreateRetailDemandMetadataStateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateRetailDemandMetadataStateRequest from a JSON string
create_retail_demand_metadata_state_request_instance = CreateRetailDemandMetadataStateRequest.from_json(json)
# print the JSON string representation of the object
print(CreateRetailDemandMetadataStateRequest.to_json())

# convert the object into a dict
create_retail_demand_metadata_state_request_dict = create_retail_demand_metadata_state_request_instance.to_dict()
# create an instance of CreateRetailDemandMetadataStateRequest from a dict
create_retail_demand_metadata_state_request_from_dict = CreateRetailDemandMetadataStateRequest.from_dict(create_retail_demand_metadata_state_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


