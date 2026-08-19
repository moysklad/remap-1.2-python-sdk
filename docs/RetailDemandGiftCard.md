# RetailDemandGiftCard

Подарочный сертификат, используемый при оплате розничной продажи

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** | Номер сертификата | [optional] 
**payment_sum** | **float** | Сумма сертификата | [optional] [readonly] 

## Example

```python
from moysklad_remap_12_sdk.models.retail_demand_gift_card import RetailDemandGiftCard

# TODO update the JSON string below
json = "{}"
# create an instance of RetailDemandGiftCard from a JSON string
retail_demand_gift_card_instance = RetailDemandGiftCard.from_json(json)
# print the JSON string representation of the object
print(RetailDemandGiftCard.to_json())

# convert the object into a dict
retail_demand_gift_card_dict = retail_demand_gift_card_instance.to_dict()
# create an instance of RetailDemandGiftCard from a dict
retail_demand_gift_card_from_dict = RetailDemandGiftCard.from_dict(retail_demand_gift_card_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


