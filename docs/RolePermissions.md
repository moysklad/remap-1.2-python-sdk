# RolePermissions

Права роли. В JSON передаются объектом, где ключи — названия пермиссий, значения — Boolean или объекты прав сущностей. Для currency, country, taxrate и uom право view неизменяемо и равно ALL; попытка изменить его приводит к ошибке. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api_request** | **bool** | Доступ по АПИ | [optional] 
**account_delete** | **bool** | Удалять аккаунт | [optional] 
**delete_from_recycle_bin** | **bool** | Очищать корзину | [optional] 
**edit_currency_rate_of_document** | **bool** | Редактировать курс валюты документа | [optional] 
**edit_document_templates** | **bool** | Редактировать шаблоны документов и отчетов | [optional] 
**edit_documents_of_restricted_period** | **bool** | Редактировать документы закрытого периода | [optional] 
**export_data** | **bool** | Экспортировать данные | [optional] 
**import_data** | **bool** | Импортировать данные | [optional] 
**listen_calls** | **bool** | Прослушивание звонков | [optional] 
**online_shops** | **bool** | Интернет магазины | [optional] 
**owner_assign** | **bool** | Передавать владение аккаунтом | [optional] 
**owner_data_update** | **bool** | Редактировать данные владельца | [optional] 
**purchase_control** | **bool** | Управление закупками | [optional] 
**restore_from_recycle_bin** | **bool** | Восстанавливать документы из корзины | [optional] 
**send_email** | **bool** | Отправлять почту | [optional] 
**subscription_control** | **bool** | Управление подпиской | [optional] 
**view_audit** | **bool** | Просматривать аудит | [optional] 
**view_cash_flow** | **bool** | Просматривать движение денежных средств | [optional] 
**view_commission_goods** | **bool** | Просматривать товары на реализации | [optional] 
**view_company_crm** | **bool** | Просматривать показатели | [optional] 
**view_customer_balance_list** | **bool** | Просматривать взаиморасчеты | [optional] 
**view_dashboard** | **bool** | Просматривать показатели | [optional] 
**view_money_dashboard** | **bool** | Видеть остатки денег | [optional] 
**view_product_cost_and_profit** | **bool** | Видеть себестоимость, цену закупки и прибыль товаров | [optional] 
**view_profit_and_loss** | **bool** | Просматривать прибыль и убытки | [optional] 
**view_purchase_funnel** | **bool** | Просматривать воронку продаж | [optional] 
**view_recycle_bin** | **bool** | Просматривать корзину | [optional] 
**view_sale_profit** | **bool** | Просматривать прибыльность | [optional] 
**view_serial_numbers** | **bool** | Просматривать серийные номера | [optional] 
**view_stock_report** | **bool** | Просматривать остатки по товарам | [optional] 
**view_turnover** | **bool** | Просматривать обороты | [optional] 
**gtin_list** | [**Permissions**](Permissions.md) |  | [optional] 
**account_adjustment** | [**Permissions**](Permissions.md) |  | [optional] 
**bonus_transaction** | [**Permissions**](Permissions.md) |  | [optional] 
**cash_in** | [**Permissions**](Permissions.md) |  | [optional] 
**cash_out** | [**Permissions**](Permissions.md) |  | [optional] 
**cashbox_adjustment** | [**Permissions**](Permissions.md) |  | [optional] 
**commission_report_in** | [**Permissions**](Permissions.md) |  | [optional] 
**commission_report_out** | [**Permissions**](Permissions.md) |  | [optional] 
**company** | [**Permissions**](Permissions.md) |  | [optional] 
**contract** | [**Permissions**](Permissions.md) |  | [optional] 
**counterparty_adjustment** | [**Permissions**](Permissions.md) |  | [optional] 
**country** | [**Permissions**](Permissions.md) |  | [optional] 
**crpt_cancellation** | [**Permissions**](Permissions.md) |  | [optional] 
**crpt_package_creation** | [**Permissions**](Permissions.md) |  | [optional] 
**crpt_package_disaggregation** | [**Permissions**](Permissions.md) |  | [optional] 
**crpt_package_item_removal** | [**Permissions**](Permissions.md) |  | [optional] 
**currency** | [**Permissions**](Permissions.md) |  | [optional] 
**custom_entity** | [**Permissions**](Permissions.md) |  | [optional] 
**customer_order** | [**Permissions**](Permissions.md) |  | [optional] 
**demand** | [**Permissions**](Permissions.md) |  | [optional] 
**emission_order** | [**Permissions**](Permissions.md) |  | [optional] 
**utilization_report** | [**Permissions**](Permissions.md) |  | [optional] 
**atk_aggregation** | [**Permissions**](Permissions.md) |  | [optional] 
**retire_order_osu** | [**Permissions**](Permissions.md) |  | [optional] 
**employee** | [**Permissions**](Permissions.md) |  | [optional] 
**enroll_order** | [**Permissions**](Permissions.md) |  | [optional] 
**enroll_return** | [**Permissions**](Permissions.md) |  | [optional] 
**enter** | [**Permissions**](Permissions.md) |  | [optional] 
**expenseitem** | [**Permissions**](Permissions.md) |  | [optional] 
**facture_in** | [**Permissions**](Permissions.md) |  | [optional] 
**facture_out** | [**Permissions**](Permissions.md) |  | [optional] 
**good** | [**Permissions**](Permissions.md) |  | [optional] 
**internal_order** | [**Permissions**](Permissions.md) |  | [optional] 
**inventory** | [**Permissions**](Permissions.md) |  | [optional] 
**invoice_in** | [**Permissions**](Permissions.md) |  | [optional] 
**invoice_out** | [**Permissions**](Permissions.md) |  | [optional] 
**loss** | [**Permissions**](Permissions.md) |  | [optional] 
**move** | [**Permissions**](Permissions.md) |  | [optional] 
**my_company** | [**Permissions**](Permissions.md) |  | [optional] 
**payment_in** | [**Permissions**](Permissions.md) |  | [optional] 
**payment_out** | [**Permissions**](Permissions.md) |  | [optional] 
**prepayment** | [**Permissions**](Permissions.md) |  | [optional] 
**prepayment_return** | [**Permissions**](Permissions.md) |  | [optional] 
**price_list** | [**Permissions**](Permissions.md) |  | [optional] 
**processing** | [**Permissions**](Permissions.md) |  | [optional] 
**processing_order** | [**Permissions**](Permissions.md) |  | [optional] 
**processing_plan** | [**Permissions**](Permissions.md) |  | [optional] 
**processing_stage** | [**Permissions**](Permissions.md) |  | [optional] 
**processing_process** | [**Permissions**](Permissions.md) |  | [optional] 
**production_task** | [**Permissions**](Permissions.md) |  | [optional] 
**production_stage_completion** | [**Permissions**](Permissions.md) |  | [optional] 
**project** | [**Permissions**](Permissions.md) |  | [optional] 
**purchase_order** | [**Permissions**](Permissions.md) |  | [optional] 
**purchase_return** | [**Permissions**](Permissions.md) |  | [optional] 
**remains_order** | [**Permissions**](Permissions.md) |  | [optional] 
**remarking_order** | [**Permissions**](Permissions.md) |  | [optional] 
**retail_demand** | [**Permissions**](Permissions.md) |  | [optional] 
**retail_drawer_cash_in** | [**Permissions**](Permissions.md) |  | [optional] 
**retail_drawer_cash_out** | [**Permissions**](Permissions.md) |  | [optional] 
**retail_sales_return** | [**Permissions**](Permissions.md) |  | [optional] 
**retail_shift** | [**Permissions**](Permissions.md) |  | [optional] 
**retail_store** | [**Permissions**](Permissions.md) |  | [optional] 
**retire_order** | [**Permissions**](Permissions.md) |  | [optional] 
**sales_return** | [**Permissions**](Permissions.md) |  | [optional] 
**sales_channel** | [**Permissions**](Permissions.md) |  | [optional] 
**script** | [**ScriptPermissions**](ScriptPermissions.md) |  | [optional] 
**script_template** | [**ScriptTemplatePermissions**](ScriptTemplatePermissions.md) |  | [optional] 
**supply** | [**Permissions**](Permissions.md) |  | [optional] 
**taxrate** | [**Permissions**](Permissions.md) |  | [optional] 
**tracking_code_list** | [**Permissions**](Permissions.md) |  | [optional] 
**uom** | [**Permissions**](Permissions.md) |  | [optional] 
**warehouse** | [**Permissions**](Permissions.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.role_permissions import RolePermissions

# TODO update the JSON string below
json = "{}"
# create an instance of RolePermissions from a JSON string
role_permissions_instance = RolePermissions.from_json(json)
# print the JSON string representation of the object
print(RolePermissions.to_json())

# convert the object into a dict
role_permissions_dict = role_permissions_instance.to_dict()
# create an instance of RolePermissions from a dict
role_permissions_from_dict = RolePermissions.from_dict(role_permissions_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


