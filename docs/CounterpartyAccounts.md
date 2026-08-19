# CounterpartyAccounts

Массив счетов контрагента

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[Account]**](Account.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.counterparty_accounts import CounterpartyAccounts

# TODO update the JSON string below
json = "{}"
# create an instance of CounterpartyAccounts from a JSON string
counterparty_accounts_instance = CounterpartyAccounts.from_json(json)
# print the JSON string representation of the object
print(CounterpartyAccounts.to_json())

# convert the object into a dict
counterparty_accounts_dict = counterparty_accounts_instance.to_dict()
# create an instance of CounterpartyAccounts from a dict
counterparty_accounts_from_dict = CounterpartyAccounts.from_dict(counterparty_accounts_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


