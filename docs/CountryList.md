# CountryList

Список стран

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[Country]**](Country.md) | Массив стран | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.country_list import CountryList

# TODO update the JSON string below
json = "{}"
# create an instance of CountryList from a JSON string
country_list_instance = CountryList.from_json(json)
# print the JSON string representation of the object
print(CountryList.to_json())

# convert the object into a dict
country_list_dict = country_list_instance.to_dict()
# create an instance of CountryList from a dict
country_list_from_dict = CountryList.from_dict(country_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


