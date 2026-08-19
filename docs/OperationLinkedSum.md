# OperationLinkedSum

Поле суммы по связанной операции. Комбинируется через `allOf` с телом документа в элементах `operations[]`. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**linked_sum** | **float** | Сумма, оплаченная по данному документу | 

## Example

```python
from moysklad_remap_12_sdk.models.operation_linked_sum import OperationLinkedSum

# TODO update the JSON string below
json = "{}"
# create an instance of OperationLinkedSum from a JSON string
operation_linked_sum_instance = OperationLinkedSum.from_json(json)
# print the JSON string representation of the object
print(OperationLinkedSum.to_json())

# convert the object into a dict
operation_linked_sum_dict = operation_linked_sum_instance.to_dict()
# create an instance of OperationLinkedSum from a dict
operation_linked_sum_from_dict = OperationLinkedSum.from_dict(operation_linked_sum_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


