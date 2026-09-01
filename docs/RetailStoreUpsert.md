# RetailStoreUpsert

Точка продаж

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | ID Точки продаж | [optional] 
**account_id** | **str** | ID учетной записи владельца Точки продаж | [optional] [readonly] 
**name** | **str** | Наименование Точки продаж | [optional] 
**description** | **str** | Комментарий к Точке продаж | [optional] 
**active** | **bool** | Признак активности Точки продаж | [optional] 
**archived** | **bool** | Признак архивности Точки продаж | [optional] 
**shared** | **bool** | Общий доступ к Точке продаж | [optional] 
**address** | **str** | Адрес Точки продаж одной строкой | [optional] 
**address_full** | [**Address**](Address.md) |  | [optional] 
**external_code** | **str** | Внешний код Точки продаж | [optional] [readonly] 
**updated** | **str** | Момент последнего обновления Точки продаж | [optional] [readonly] 
**meta** | [**Meta**](Meta.md) |  | [optional] 
**organization** | [**Organization**](Organization.md) |  | [optional] 
**store** | [**Store**](Store.md) |  | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**owner** | [**Employee**](Employee.md) | Метаданные владельца (сотрудника) | [optional] 
**price_type** | [**PriceType**](PriceType.md) |  | [optional] 
**environment** | [**RetailStoreEnvironment**](RetailStoreEnvironment.md) |  | [optional] 
**state** | [**RetailStoreState**](RetailStoreState.md) |  | [optional] 
**fiscal_type** | **str** | Фискальный режим работы Точки продаж. Известные значения описаны в FiscalType | [optional] 
**default_tax_system** | **str** | Система налогообложения по умолчанию. Известные значения описаны в TaxSystem | [optional] 
**order_tax_system** | **str** | Система налогообложения заказов. Известные значения описаны в TaxSystem | [optional] 
**minion_to_master_type** | **str** | Ограничение связи касс-слуг с кассами-мастерами. Известные значения описаны в MinionToMasterType | [optional] 
**tobacco_mrc_control_type** | **str** | Режим контроля минимальных розничных цен на табак. Известные значения описаны в TobaccoMrcControlType | [optional] 
**marking_selling_mode** | **str** | Режим продажи маркированных товаров. Известные значения описаны в MarkingSellingMode | [optional] 
**marks_check_mode** | **str** | Режим проверки кодов маркировки. Известные значения описаны в MarksCheckMode | [optional] 
**priority_ofd_send** | **str** | Приоритетный способ отправки чека покупателю. Известные значения описаны в PriorityOfdSend | [optional] 
**allow_create_products** | **bool** | Признак разрешения создания новых товаров при продаже | [optional] 
**allow_custom_price** | **bool** | Признак разрешения устанавливать произвольные цены | [optional] 
**allow_delete_receipt_positions** | **bool** | Признак разрешения удалять позиции из чека | [optional] 
**allow_sell_tobacco_without_mrc** | **bool** | Признак разрешения продажи табачной продукции без проверки МРЦ | [optional] 
**auth_token_attached** | **bool** | Признак подключения авторизационного токена | [optional] [readonly] 
**control_cashier_choice** | **bool** | Признак контроля выбора кассира | [optional] 
**control_shipping_stock** | **bool** | Признак контроля отгрузки только из наличия | [optional] 
**create_cash_in_on_retail_shift_closing** | **bool** | Признак создания операции внесения при закрытии смены | [optional] 
**create_payment_in_on_retail_shift_closing** | **bool** | Признак создания операции прихода денег при закрытии смены | [optional] 
**create_agents_tags** | **List[str]** | Теги, создаваемые у агентов | [optional] 
**filter_agents_tags** | **List[str]** | Группы, по которым фильтруются агенты | [optional] 
**create_order_with_state** | [**State**](State.md) | Статус, в котором создаются заказы покупателей | [optional] 
**customer_order_states** | [**List[State]**](State.md) | Возможные состояния заказов покупателей | [optional] 
**discount_enable** | **bool** | Признак включения скидок | [optional] 
**discount_max_percent** | **int** | Максимально допустимый процент скидки | [optional] 
**enable_returns_with_no_reason** | **bool** | Признак разрешения возвратов без причины | [optional] 
**issue_orders** | **bool** | Признак оформления заказов покупателей | [optional] 
**last_operation_names** | [**List[RetailStoreLastOperationNamesInner]**](RetailStoreLastOperationNamesInner.md) | Последние операции | [optional] 
**master_retail_stores** | [**RetailStoreList**](RetailStoreList.md) | Список касс-мастеров | [optional] 
**ofd_enabled** | **bool** | Признак использования ОФД | [optional] [readonly] 
**only_in_stock** | **bool** | Признак продажи только из наличия | [optional] 
**order_to_state** | [**State**](State.md) | Метаданные статуса заказа покупателя | [optional] 
**print_always** | **bool** | Признак обязательной печати чеков | [optional] 
**product_folders** | [**ProductFolderList**](ProductFolderList.md) | Список групп товаров | [optional] 
**receipt_template** | [**RetailStoreReceiptTemplate**](RetailStoreReceiptTemplate.md) |  | [optional] 
**required_fio** | **bool** | Признак обязательности ФИО покупателя | [optional] 
**required_phone** | **bool** | Признак обязательности телефона покупателя | [optional] 
**required_email** | **bool** | Признак обязательности email покупателя | [optional] 
**required_birthdate** | **bool** | Признак обязательности даты рождения покупателя | [optional] 
**required_sex** | **bool** | Признак обязательности пола покупателя | [optional] 
**required_discount_card_number** | **bool** | Признак обязательности номера дисконтной карты покупателя | [optional] 
**reserve_prepaid_goods** | **bool** | Признак резервирования предоплаченных товаров | [optional] 
**return_from_closed_shift_enabled** | **bool** | Признак разрешения возвратов из закрытой смены | [optional] 
**sell_reserves** | **bool** | Признак разрешения продажи резервов | [optional] 
**send_marks_for_check** | **bool** | Признак отправки кодов маркировки на проверку | [optional] 
**send_marks_to_chestny_znak_on_cloud** | **bool** | Признак отправки кодов маркировки в Честный ЗНАК в облаке | [optional] 
**sync_agents** | **bool** | Признак синхронизации агентов | [optional] 
**show_beer_on_tap** | **bool** | Признак отображения разливного пива | [optional] 
**qr_pay_enabled** | **bool** | Признак включения оплаты через QR | [optional] 
**bank_percent** | **float** | Банковский процент | [optional] 
**qr_bank_percent** | **float** | Банковский процент при оплате по QR | [optional] 
**demand_prefix** | **str** | Префикс номера заказа | [optional] 
**qr_terminal_id** | **str** | Идентификатор QR-терминала | [optional] 
**id_qr** | **str** | Идентификатор QR | [optional] 
**acquire** | [**Agent**](Agent.md) | Эквайер | [optional] 
**cashiers** | [**List[Employee]**](Employee.md) | Кассиры, работающие на точке продаж | [optional] 
**qr_acquire** | [**Agent**](Agent.md) | Эквайер для QR-платежей | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.retail_store_upsert import RetailStoreUpsert

# TODO update the JSON string below
json = "{}"
# create an instance of RetailStoreUpsert from a JSON string
retail_store_upsert_instance = RetailStoreUpsert.from_json(json)
# print the JSON string representation of the object
print(RetailStoreUpsert.to_json())

# convert the object into a dict
retail_store_upsert_dict = retail_store_upsert_instance.to_dict()
# create an instance of RetailStoreUpsert from a dict
retail_store_upsert_from_dict = RetailStoreUpsert.from_dict(retail_store_upsert_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


