# CounterpartyMetadata

Метаданные контрагентов

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**attributes** | [**AttributeMetaInfoList**](AttributeMetaInfoList.md) |  | [optional] 
**states** | [**List[State]**](State.md) | Массив статусов контрагентов | [optional] 
**tags** | **List[str]** | Тэги контрагентов | [optional] 
**create_shared** | **bool** | Создавать новых контрагентов с меткой \&quot;Общий\&quot; | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.counterparty_metadata import CounterpartyMetadata

# TODO update the JSON string below
json = "{}"
# create an instance of CounterpartyMetadata from a JSON string
counterparty_metadata_instance = CounterpartyMetadata.from_json(json)
# print the JSON string representation of the object
print(CounterpartyMetadata.to_json())

# convert the object into a dict
counterparty_metadata_dict = counterparty_metadata_instance.to_dict()
# create an instance of CounterpartyMetadata from a dict
counterparty_metadata_from_dict = CounterpartyMetadata.from_dict(counterparty_metadata_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


