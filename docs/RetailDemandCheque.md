# RetailDemandCheque

Фискальные данные продажи

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**fn_number** | **str** | Номер фискального накопителя | [optional] [readonly] 
**fiscal_doc_sign** | **str** | Фискальный признак документа | [optional] [readonly] 
**fiscal_doc_number** | **str** | Номер фискального документа | [optional] [readonly] 
**kkt_reg_number** | **str** | Регистрационный номер | [optional] [readonly] 
**time** | **str** | Время фискализации | [optional] [readonly] 
**receipt** | **str** | Электронный чек | [optional] [readonly] 

## Example

```python
from moysklad_remap_12_sdk.models.retail_demand_cheque import RetailDemandCheque

# TODO update the JSON string below
json = "{}"
# create an instance of RetailDemandCheque from a JSON string
retail_demand_cheque_instance = RetailDemandCheque.from_json(json)
# print the JSON string representation of the object
print(RetailDemandCheque.to_json())

# convert the object into a dict
retail_demand_cheque_dict = retail_demand_cheque_instance.to_dict()
# create an instance of RetailDemandCheque from a dict
retail_demand_cheque_from_dict = RetailDemandCheque.from_dict(retail_demand_cheque_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


