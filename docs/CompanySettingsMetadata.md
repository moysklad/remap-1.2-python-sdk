# CompanySettingsMetadata

Метаданные Настроек компании (companysettings/metadata)

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**custom_entities** | [**List[CustomEntityMetadata]**](CustomEntityMetadata.md) | Список пользовательских справочников | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.company_settings_metadata import CompanySettingsMetadata

# TODO update the JSON string below
json = "{}"
# create an instance of CompanySettingsMetadata from a JSON string
company_settings_metadata_instance = CompanySettingsMetadata.from_json(json)
# print the JSON string representation of the object
print(CompanySettingsMetadata.to_json())

# convert the object into a dict
company_settings_metadata_dict = company_settings_metadata_instance.to_dict()
# create an instance of CompanySettingsMetadata from a dict
company_settings_metadata_from_dict = CompanySettingsMetadata.from_dict(company_settings_metadata_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


