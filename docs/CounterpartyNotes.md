# CounterpartyNotes

Массив контактных лиц

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[Note]**](Note.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.counterparty_notes import CounterpartyNotes

# TODO update the JSON string below
json = "{}"
# create an instance of CounterpartyNotes from a JSON string
counterparty_notes_instance = CounterpartyNotes.from_json(json)
# print the JSON string representation of the object
print(CounterpartyNotes.to_json())

# convert the object into a dict
counterparty_notes_dict = counterparty_notes_instance.to_dict()
# create an instance of CounterpartyNotes from a dict
counterparty_notes_from_dict = CounterpartyNotes.from_dict(counterparty_notes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


