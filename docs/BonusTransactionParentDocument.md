# BonusTransactionParentDocument

Метаданные связанного документа бонусной операции

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.bonus_transaction_parent_document import BonusTransactionParentDocument

# TODO update the JSON string below
json = "{}"
# create an instance of BonusTransactionParentDocument from a JSON string
bonus_transaction_parent_document_instance = BonusTransactionParentDocument.from_json(json)
# print the JSON string representation of the object
print(BonusTransactionParentDocument.to_json())

# convert the object into a dict
bonus_transaction_parent_document_dict = bonus_transaction_parent_document_instance.to_dict()
# create an instance of BonusTransactionParentDocument from a dict
bonus_transaction_parent_document_from_dict = BonusTransactionParentDocument.from_dict(bonus_transaction_parent_document_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


