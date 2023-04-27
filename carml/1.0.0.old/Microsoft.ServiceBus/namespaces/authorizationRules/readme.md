# ServiceBus Namespace Authorization Rules `[Microsoft.ServiceBus/namespaces/authorizationRules]`

This module deploys authorization rules for a service bus namespace

## Resource Types

| Resource Type | API Version |
| :-- | :-- |
| `Microsoft.ServiceBus/namespaces/AuthorizationRules` | 2017-04-01 |

## Parameters

| Parameter Name | Type | Default Value | Possible Values | Description |
| :-- | :-- | :-- | :-- | :-- |
| `cuaId` | string |  |  | Optional. Customer Usage Attribution ID (GUID). This GUID must be previously registered |
| `name` | string |  |  | Required. The name of the authorization rule |
| `namespaceName` | string |  |  | Required. Name of the parent Service Bus Namespace for the Service Bus Queue. |
| `rights` | array | `[]` | `[Listen, Manage, Send]` | Optional. The rights associated with the rule. |

## Outputs

| Output Name | Type | Description |
| :-- | :-- | :-- |
| `name` | string | The name of the authorization rule. |
| `resourceGroupName` | string | The name of the Resource Group the authorization rule was created in. |
| `resourceId` | string | The resource ID of the authorization rule. |

## Template references

- [Namespaces/Authorizationrules](https://docs.microsoft.com/en-us/azure/templates/Microsoft.ServiceBus/2017-04-01/namespaces/AuthorizationRules)