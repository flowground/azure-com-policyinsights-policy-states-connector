# ![LOGO](logo.png) PolicyStatesClient **flow**ground Connector

## Description

A generated **flow**ground connector for the PolicyStatesClient API (version 2018-07-01-preview).

Generated from: https://api.apis.guru/v2/specs/azure.com/policyinsights-policyStates/2018-07-01-preview/swagger.json<br/>
Generated at: 2019-05-07T17:38:36+03:00

## API Description



## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Lists available operations.

#### Input Parameters
* `api-version` - _required_ - Client Api Version.

### Queries policy states for the resources under the management group.

#### Input Parameters
* `policyStatesResource` - _required_ - The virtual resource under PolicyStates resource type. In a given time range, 'latest' represents the latest policy state(s), whereas 'default' represents all policy state(s).
    Possible values: default, latest.
* `managementGroupsNamespace` - _required_ - The namespace for Microsoft Management RP; only "Microsoft.Management" is allowed.
    Possible values: Microsoft.Management.
* `managementGroupName` - _required_ - Management group name.
* `api-version` - _required_ - Client Api Version.
* `$top` - _optional_ - Maximum number of records to return.
* `$orderby` - _optional_ - Ordering expression using OData notation. One or more comma-separated column names with an optional "desc" (the default) or "asc", e.g. "$orderby=PolicyAssignmentId, ResourceId asc".
* `$select` - _optional_ - Select expression using OData notation. Limits the columns on each record to just those requested, e.g. "$select=PolicyAssignmentId, ResourceId".
* `$from` - _optional_ - ISO 8601 formatted timestamp specifying the start time of the interval to query. When not specified, the service uses ($to - 1-day).
* `$to` - _optional_ - ISO 8601 formatted timestamp specifying the end time of the interval to query. When not specified, the service uses request time.
* `$filter` - _optional_ - OData filter expression.
* `$apply` - _optional_ - OData apply expression for aggregations.

### Summarizes policy states for the resources under the management group.

#### Input Parameters
* `policyStatesSummaryResource` - _required_ - The virtual resource under PolicyStates resource type for summarize action. In a given time range, 'latest' represents the latest policy state(s) and is the only allowed value.
    Possible values: latest.
* `managementGroupsNamespace` - _required_ - The namespace for Microsoft Management RP; only "Microsoft.Management" is allowed.
    Possible values: Microsoft.Management.
* `managementGroupName` - _required_ - Management group name.
* `api-version` - _required_ - Client Api Version.
* `$top` - _optional_ - Maximum number of records to return.
* `$from` - _optional_ - ISO 8601 formatted timestamp specifying the start time of the interval to query. When not specified, the service uses ($to - 1-day).
* `$to` - _optional_ - ISO 8601 formatted timestamp specifying the end time of the interval to query. When not specified, the service uses request time.
* `$filter` - _optional_ - OData filter expression.

### Queries policy states for the resources under the subscription.

#### Input Parameters
* `policyStatesResource` - _required_ - The virtual resource under PolicyStates resource type. In a given time range, 'latest' represents the latest policy state(s), whereas 'default' represents all policy state(s).
    Possible values: default, latest.
* `subscriptionId` - _required_ - Microsoft Azure subscription ID.
* `api-version` - _required_ - Client Api Version.
* `$top` - _optional_ - Maximum number of records to return.
* `$orderby` - _optional_ - Ordering expression using OData notation. One or more comma-separated column names with an optional "desc" (the default) or "asc", e.g. "$orderby=PolicyAssignmentId, ResourceId asc".
* `$select` - _optional_ - Select expression using OData notation. Limits the columns on each record to just those requested, e.g. "$select=PolicyAssignmentId, ResourceId".
* `$from` - _optional_ - ISO 8601 formatted timestamp specifying the start time of the interval to query. When not specified, the service uses ($to - 1-day).
* `$to` - _optional_ - ISO 8601 formatted timestamp specifying the end time of the interval to query. When not specified, the service uses request time.
* `$filter` - _optional_ - OData filter expression.
* `$apply` - _optional_ - OData apply expression for aggregations.

### Summarizes policy states for the resources under the subscription.

#### Input Parameters
* `policyStatesSummaryResource` - _required_ - The virtual resource under PolicyStates resource type for summarize action. In a given time range, 'latest' represents the latest policy state(s) and is the only allowed value.
    Possible values: latest.
* `subscriptionId` - _required_ - Microsoft Azure subscription ID.
* `api-version` - _required_ - Client Api Version.
* `$top` - _optional_ - Maximum number of records to return.
* `$from` - _optional_ - ISO 8601 formatted timestamp specifying the start time of the interval to query. When not specified, the service uses ($to - 1-day).
* `$to` - _optional_ - ISO 8601 formatted timestamp specifying the end time of the interval to query. When not specified, the service uses request time.
* `$filter` - _optional_ - OData filter expression.

### Queries policy states for the subscription level policy assignment.

#### Input Parameters
* `policyStatesResource` - _required_ - The virtual resource under PolicyStates resource type. In a given time range, 'latest' represents the latest policy state(s), whereas 'default' represents all policy state(s).
    Possible values: default, latest.
* `subscriptionId` - _required_ - Microsoft Azure subscription ID.
* `authorizationNamespace` - _required_ - The namespace for Microsoft Authorization resource provider; only "Microsoft.Authorization" is allowed.
    Possible values: Microsoft.Authorization.
* `policyAssignmentName` - _required_ - Policy assignment name.
* `api-version` - _required_ - Client Api Version.
* `$top` - _optional_ - Maximum number of records to return.
* `$orderby` - _optional_ - Ordering expression using OData notation. One or more comma-separated column names with an optional "desc" (the default) or "asc", e.g. "$orderby=PolicyAssignmentId, ResourceId asc".
* `$select` - _optional_ - Select expression using OData notation. Limits the columns on each record to just those requested, e.g. "$select=PolicyAssignmentId, ResourceId".
* `$from` - _optional_ - ISO 8601 formatted timestamp specifying the start time of the interval to query. When not specified, the service uses ($to - 1-day).
* `$to` - _optional_ - ISO 8601 formatted timestamp specifying the end time of the interval to query. When not specified, the service uses request time.
* `$filter` - _optional_ - OData filter expression.
* `$apply` - _optional_ - OData apply expression for aggregations.

### Summarizes policy states for the subscription level policy assignment.

#### Input Parameters
* `policyStatesSummaryResource` - _required_ - The virtual resource under PolicyStates resource type for summarize action. In a given time range, 'latest' represents the latest policy state(s) and is the only allowed value.
    Possible values: latest.
* `subscriptionId` - _required_ - Microsoft Azure subscription ID.
* `authorizationNamespace` - _required_ - The namespace for Microsoft Authorization resource provider; only "Microsoft.Authorization" is allowed.
    Possible values: Microsoft.Authorization.
* `policyAssignmentName` - _required_ - Policy assignment name.
* `api-version` - _required_ - Client Api Version.
* `$top` - _optional_ - Maximum number of records to return.
* `$from` - _optional_ - ISO 8601 formatted timestamp specifying the start time of the interval to query. When not specified, the service uses ($to - 1-day).
* `$to` - _optional_ - ISO 8601 formatted timestamp specifying the end time of the interval to query. When not specified, the service uses request time.
* `$filter` - _optional_ - OData filter expression.

### Queries policy states for the subscription level policy definition.

#### Input Parameters
* `policyStatesResource` - _required_ - The virtual resource under PolicyStates resource type. In a given time range, 'latest' represents the latest policy state(s), whereas 'default' represents all policy state(s).
    Possible values: default, latest.
* `subscriptionId` - _required_ - Microsoft Azure subscription ID.
* `authorizationNamespace` - _required_ - The namespace for Microsoft Authorization resource provider; only "Microsoft.Authorization" is allowed.
    Possible values: Microsoft.Authorization.
* `policyDefinitionName` - _required_ - Policy definition name.
* `api-version` - _required_ - Client Api Version.
* `$top` - _optional_ - Maximum number of records to return.
* `$orderby` - _optional_ - Ordering expression using OData notation. One or more comma-separated column names with an optional "desc" (the default) or "asc", e.g. "$orderby=PolicyAssignmentId, ResourceId asc".
* `$select` - _optional_ - Select expression using OData notation. Limits the columns on each record to just those requested, e.g. "$select=PolicyAssignmentId, ResourceId".
* `$from` - _optional_ - ISO 8601 formatted timestamp specifying the start time of the interval to query. When not specified, the service uses ($to - 1-day).
* `$to` - _optional_ - ISO 8601 formatted timestamp specifying the end time of the interval to query. When not specified, the service uses request time.
* `$filter` - _optional_ - OData filter expression.
* `$apply` - _optional_ - OData apply expression for aggregations.

### Summarizes policy states for the subscription level policy definition.

#### Input Parameters
* `policyStatesSummaryResource` - _required_ - The virtual resource under PolicyStates resource type for summarize action. In a given time range, 'latest' represents the latest policy state(s) and is the only allowed value.
    Possible values: latest.
* `subscriptionId` - _required_ - Microsoft Azure subscription ID.
* `authorizationNamespace` - _required_ - The namespace for Microsoft Authorization resource provider; only "Microsoft.Authorization" is allowed.
    Possible values: Microsoft.Authorization.
* `policyDefinitionName` - _required_ - Policy definition name.
* `api-version` - _required_ - Client Api Version.
* `$top` - _optional_ - Maximum number of records to return.
* `$from` - _optional_ - ISO 8601 formatted timestamp specifying the start time of the interval to query. When not specified, the service uses ($to - 1-day).
* `$to` - _optional_ - ISO 8601 formatted timestamp specifying the end time of the interval to query. When not specified, the service uses request time.
* `$filter` - _optional_ - OData filter expression.

### Queries policy states for the subscription level policy set definition.

#### Input Parameters
* `policyStatesResource` - _required_ - The virtual resource under PolicyStates resource type. In a given time range, 'latest' represents the latest policy state(s), whereas 'default' represents all policy state(s).
    Possible values: default, latest.
* `subscriptionId` - _required_ - Microsoft Azure subscription ID.
* `authorizationNamespace` - _required_ - The namespace for Microsoft Authorization resource provider; only "Microsoft.Authorization" is allowed.
    Possible values: Microsoft.Authorization.
* `policySetDefinitionName` - _required_ - Policy set definition name.
* `api-version` - _required_ - Client Api Version.
* `$top` - _optional_ - Maximum number of records to return.
* `$orderby` - _optional_ - Ordering expression using OData notation. One or more comma-separated column names with an optional "desc" (the default) or "asc", e.g. "$orderby=PolicyAssignmentId, ResourceId asc".
* `$select` - _optional_ - Select expression using OData notation. Limits the columns on each record to just those requested, e.g. "$select=PolicyAssignmentId, ResourceId".
* `$from` - _optional_ - ISO 8601 formatted timestamp specifying the start time of the interval to query. When not specified, the service uses ($to - 1-day).
* `$to` - _optional_ - ISO 8601 formatted timestamp specifying the end time of the interval to query. When not specified, the service uses request time.
* `$filter` - _optional_ - OData filter expression.
* `$apply` - _optional_ - OData apply expression for aggregations.

### Summarizes policy states for the subscription level policy set definition.

#### Input Parameters
* `policyStatesSummaryResource` - _required_ - The virtual resource under PolicyStates resource type for summarize action. In a given time range, 'latest' represents the latest policy state(s) and is the only allowed value.
    Possible values: latest.
* `subscriptionId` - _required_ - Microsoft Azure subscription ID.
* `authorizationNamespace` - _required_ - The namespace for Microsoft Authorization resource provider; only "Microsoft.Authorization" is allowed.
    Possible values: Microsoft.Authorization.
* `policySetDefinitionName` - _required_ - Policy set definition name.
* `api-version` - _required_ - Client Api Version.
* `$top` - _optional_ - Maximum number of records to return.
* `$from` - _optional_ - ISO 8601 formatted timestamp specifying the start time of the interval to query. When not specified, the service uses ($to - 1-day).
* `$to` - _optional_ - ISO 8601 formatted timestamp specifying the end time of the interval to query. When not specified, the service uses request time.
* `$filter` - _optional_ - OData filter expression.

### Queries policy states for the resources under the resource group.

#### Input Parameters
* `policyStatesResource` - _required_ - The virtual resource under PolicyStates resource type. In a given time range, 'latest' represents the latest policy state(s), whereas 'default' represents all policy state(s).
    Possible values: default, latest.
* `subscriptionId` - _required_ - Microsoft Azure subscription ID.
* `resourceGroupName` - _required_ - Resource group name.
* `api-version` - _required_ - Client Api Version.
* `$top` - _optional_ - Maximum number of records to return.
* `$orderby` - _optional_ - Ordering expression using OData notation. One or more comma-separated column names with an optional "desc" (the default) or "asc", e.g. "$orderby=PolicyAssignmentId, ResourceId asc".
* `$select` - _optional_ - Select expression using OData notation. Limits the columns on each record to just those requested, e.g. "$select=PolicyAssignmentId, ResourceId".
* `$from` - _optional_ - ISO 8601 formatted timestamp specifying the start time of the interval to query. When not specified, the service uses ($to - 1-day).
* `$to` - _optional_ - ISO 8601 formatted timestamp specifying the end time of the interval to query. When not specified, the service uses request time.
* `$filter` - _optional_ - OData filter expression.
* `$apply` - _optional_ - OData apply expression for aggregations.

### Summarizes policy states for the resources under the resource group.

#### Input Parameters
* `policyStatesSummaryResource` - _required_ - The virtual resource under PolicyStates resource type for summarize action. In a given time range, 'latest' represents the latest policy state(s) and is the only allowed value.
    Possible values: latest.
* `subscriptionId` - _required_ - Microsoft Azure subscription ID.
* `resourceGroupName` - _required_ - Resource group name.
* `api-version` - _required_ - Client Api Version.
* `$top` - _optional_ - Maximum number of records to return.
* `$from` - _optional_ - ISO 8601 formatted timestamp specifying the start time of the interval to query. When not specified, the service uses ($to - 1-day).
* `$to` - _optional_ - ISO 8601 formatted timestamp specifying the end time of the interval to query. When not specified, the service uses request time.
* `$filter` - _optional_ - OData filter expression.

### Queries policy states for the resource group level policy assignment.

#### Input Parameters
* `policyStatesResource` - _required_ - The virtual resource under PolicyStates resource type. In a given time range, 'latest' represents the latest policy state(s), whereas 'default' represents all policy state(s).
    Possible values: default, latest.
* `subscriptionId` - _required_ - Microsoft Azure subscription ID.
* `resourceGroupName` - _required_ - Resource group name.
* `authorizationNamespace` - _required_ - The namespace for Microsoft Authorization resource provider; only "Microsoft.Authorization" is allowed.
    Possible values: Microsoft.Authorization.
* `policyAssignmentName` - _required_ - Policy assignment name.
* `api-version` - _required_ - Client Api Version.
* `$top` - _optional_ - Maximum number of records to return.
* `$orderby` - _optional_ - Ordering expression using OData notation. One or more comma-separated column names with an optional "desc" (the default) or "asc", e.g. "$orderby=PolicyAssignmentId, ResourceId asc".
* `$select` - _optional_ - Select expression using OData notation. Limits the columns on each record to just those requested, e.g. "$select=PolicyAssignmentId, ResourceId".
* `$from` - _optional_ - ISO 8601 formatted timestamp specifying the start time of the interval to query. When not specified, the service uses ($to - 1-day).
* `$to` - _optional_ - ISO 8601 formatted timestamp specifying the end time of the interval to query. When not specified, the service uses request time.
* `$filter` - _optional_ - OData filter expression.
* `$apply` - _optional_ - OData apply expression for aggregations.

### Summarizes policy states for the resource group level policy assignment.

#### Input Parameters
* `policyStatesSummaryResource` - _required_ - The virtual resource under PolicyStates resource type for summarize action. In a given time range, 'latest' represents the latest policy state(s) and is the only allowed value.
    Possible values: latest.
* `subscriptionId` - _required_ - Microsoft Azure subscription ID.
* `resourceGroupName` - _required_ - Resource group name.
* `authorizationNamespace` - _required_ - The namespace for Microsoft Authorization resource provider; only "Microsoft.Authorization" is allowed.
    Possible values: Microsoft.Authorization.
* `policyAssignmentName` - _required_ - Policy assignment name.
* `api-version` - _required_ - Client Api Version.
* `$top` - _optional_ - Maximum number of records to return.
* `$from` - _optional_ - ISO 8601 formatted timestamp specifying the start time of the interval to query. When not specified, the service uses ($to - 1-day).
* `$to` - _optional_ - ISO 8601 formatted timestamp specifying the end time of the interval to query. When not specified, the service uses request time.
* `$filter` - _optional_ - OData filter expression.

### Queries policy states for the resource.

#### Input Parameters
* `policyStatesResource` - _required_ - The virtual resource under PolicyStates resource type. In a given time range, 'latest' represents the latest policy state(s), whereas 'default' represents all policy state(s).
    Possible values: default, latest.
* `resourceId` - _required_ - Resource ID.
* `api-version` - _required_ - Client Api Version.
* `$top` - _optional_ - Maximum number of records to return.
* `$orderby` - _optional_ - Ordering expression using OData notation. One or more comma-separated column names with an optional "desc" (the default) or "asc", e.g. "$orderby=PolicyAssignmentId, ResourceId asc".
* `$select` - _optional_ - Select expression using OData notation. Limits the columns on each record to just those requested, e.g. "$select=PolicyAssignmentId, ResourceId".
* `$from` - _optional_ - ISO 8601 formatted timestamp specifying the start time of the interval to query. When not specified, the service uses ($to - 1-day).
* `$to` - _optional_ - ISO 8601 formatted timestamp specifying the end time of the interval to query. When not specified, the service uses request time.
* `$filter` - _optional_ - OData filter expression.
* `$apply` - _optional_ - OData apply expression for aggregations.
* `$expand` - _optional_ - The $expand query parameter. For example, to expand policyEvaluationDetails, use $expand=policyEvaluationDetails

### Summarizes policy states for the resource.

#### Input Parameters
* `policyStatesSummaryResource` - _required_ - The virtual resource under PolicyStates resource type for summarize action. In a given time range, 'latest' represents the latest policy state(s) and is the only allowed value.
    Possible values: latest.
* `resourceId` - _required_ - Resource ID.
* `api-version` - _required_ - Client Api Version.
* `$top` - _optional_ - Maximum number of records to return.
* `$from` - _optional_ - ISO 8601 formatted timestamp specifying the start time of the interval to query. When not specified, the service uses ($to - 1-day).
* `$to` - _optional_ - ISO 8601 formatted timestamp specifying the end time of the interval to query. When not specified, the service uses request time.
* `$filter` - _optional_ - OData filter expression.

### Gets OData metadata XML document.

#### Input Parameters
* `scope` - _required_ - A valid scope, i.e. management group, subscription, resource group, or resource ID. Scope used has no effect on metadata returned.
* `api-version` - _required_ - Client Api Version.

## License

**flow**ground :- Telekom iPaaS / azure-com-policyinsights-policy-states-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
