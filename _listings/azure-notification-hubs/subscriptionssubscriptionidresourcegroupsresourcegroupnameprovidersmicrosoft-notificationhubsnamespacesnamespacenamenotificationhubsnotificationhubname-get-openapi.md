---
swagger: "2.0"
x-collection-name: Azure Notification Hubs
x-complete: 0
info:
  title: Azure Notification Hubs API Notification Hubs Get
  description: Lists the notification hubs associated with a namespace.
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.NotificationHubs/namespaces/{namespaceName}/notificationHubs/{notificationHubName}
  : put:
      summary: Notification Hubs Create Or Update
      description: Creates/Update a NotificationHub in a namespace.
      operationId: NotificationHubs_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-notificationhubsnamespacesnamespacenamenotificationhubsnotificationhubname-put
      parameters:
      - in: path
        name: namespaceName
        description: The namespace name
      - in: query
        name: No Name
      - in: path
        name: notificationHubName
        description: The notification hub name
      - in: body
        name: parameters
        description: Parameters supplied to the create/update a NotificationHub Resource
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Notification Hubs
    delete:
      summary: Notification Hubs Delete
      description: Deletes a notification hub associated with a namespace.
      operationId: NotificationHubs_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-notificationhubsnamespacesnamespacenamenotificationhubsnotificationhubname-delete
      parameters:
      - in: path
        name: namespaceName
        description: The namespace name
      - in: query
        name: No Name
      - in: path
        name: notificationHubName
        description: The notification hub name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Notification Hubs
    get:
      summary: Notification Hubs Get
      description: Lists the notification hubs associated with a namespace.
      operationId: NotificationHubs_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-notificationhubsnamespacesnamespacenamenotificationhubsnotificationhubname-get
      parameters:
      - in: path
        name: namespaceName
        description: The namespace name
      - in: query
        name: No Name
      - in: path
        name: notificationHubName
        description: The notification hub name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Notification Hubs
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.NotificationHubs/namespaces/{namespaceName}/notificationHubs
  : get:
      summary: Notification Hubs List
      description: Lists the notification hubs associated with a namespace.
      operationId: NotificationHubs_List
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-notificationhubsnamespacesnamespacenamenotificationhubs-get
      parameters:
      - in: path
        name: namespaceName
        description: The namespace name
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Notification Hubs
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.NotificationHubs/namespaces/{namespaceName}/notificationHubs/{notificationHubName}/AuthorizationRules/{authorizationRuleName}
  : put:
      summary: Notification Hubs Create Or Update Authorization Rule
      description: Creates/Updates an authorization rule for a NotificationHub
      operationId: NotificationHubs_CreateOrUpdateAuthorizationRule
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-notificationhubsnamespacesnamespacenamenotificationhubsnotificationhubnameauthorizationrulesauthorizationrulename-put
      parameters:
      - in: path
        name: authorizationRuleName
        description: Authorization Rule Name
      - in: path
        name: namespaceName
        description: The namespace name
      - in: query
        name: No Name
      - in: path
        name: notificationHubName
        description: The notification hub name
      - in: body
        name: parameters
        description: The shared access authorization rule
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Notification Hubs Authorization Rule
    delete:
      summary: Notification Hubs Delete Authorization Rule
      description: Deletes a notificationHub authorization rule
      operationId: NotificationHubs_DeleteAuthorizationRule
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-notificationhubsnamespacesnamespacenamenotificationhubsnotificationhubnameauthorizationrulesauthorizationrulename-delete
      parameters:
      - in: path
        name: authorizationRuleName
        description: Authorization Rule Name
      - in: path
        name: namespaceName
        description: The namespace name
      - in: query
        name: No Name
      - in: path
        name: notificationHubName
        description: The notification hub name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Notification Hubs Authorization Rule
    get:
      summary: Notification Hubs Get Authorization Rule
      description: Gets an authorization rule for a NotificationHub by name.
      operationId: NotificationHubs_GetAuthorizationRule
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-notificationhubsnamespacesnamespacenamenotificationhubsnotificationhubnameauthorizationrulesauthorizationrulename-get
      parameters:
      - in: path
        name: authorizationRuleName
        description: authorization rule name
      - in: path
        name: namespaceName
        description: The namespace name
      - in: query
        name: No Name
      - in: path
        name: notificationHubName
        description: The notification hub name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Notification Hubs Authorization Rule
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.NotificationHubs/namespaces/{namespaceName}/notificationHubs/{notificationHubName}/AuthorizationRules
  : get:
      summary: Notification Hubs List Authorization Rules
      description: Gets the authorization rules for a NotificationHub.
      operationId: NotificationHubs_ListAuthorizationRules
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-notificationhubsnamespacesnamespacenamenotificationhubsnotificationhubnameauthorizationrules-get
      parameters:
      - in: path
        name: namespaceName
        description: The namespace name
      - in: query
        name: No Name
      - in: path
        name: notificationHubName
        description: The notification hub name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Notification Hubs Authorization Rules
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.NotificationHubs/namespaces/{namespaceName}/checkNotificationHubAvailability
  : post:
      summary: Notification Hubs Check Availability
      description: Checks the availability of the given notificationHub in a namespace.
      operationId: NotificationHubs_CheckAvailability
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-notificationhubsnamespacesnamespacenamechecknotificationhubavailability-post
      parameters:
      - in: path
        name: namespaceName
        description: The namespace name
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The notificationHub name
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Notification Hubs Availability
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.NotificationHubs/namespaces/{namespaceName}/notificationHubs/{notificationHubName}/AuthorizationRules/{authorizationRuleName}/listKeys
  : post:
      summary: Notification Hubs List Keys
      description: Gets the Primary and Secondary ConnectionStrings to the NotificationHub
      operationId: NotificationHubs_ListKeys
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-notificationhubsnamespacesnamespacenamenotificationhubsnotificationhubnameauthorizationrulesauthorizationrulenamelistkeys-post
      parameters:
      - in: path
        name: authorizationRuleName
        description: The connection string of the NotificationHub for the specified
          authorizationRule
      - in: path
        name: namespaceName
        description: The namespace name
      - in: query
        name: No Name
      - in: path
        name: notificationHubName
        description: The notification hub name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Notification Hubs Keys
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.NotificationHubs/namespaces/{namespaceName}/notificationHubs/{notificationHubName}/pnsCredentials
  : post:
      summary: Notification Hubs Get Pns Credentials
      description: Lists the PNS Credentials associated with a notification hub .
      operationId: NotificationHubs_GetPnsCredentials
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-notificationhubsnamespacesnamespacenamenotificationhubsnotificationhubnamepnscredentials-post
      parameters:
      - in: path
        name: namespaceName
        description: The namespace name
      - in: query
        name: No Name
      - in: path
        name: notificationHubName
        description: The notification hub name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Notification Hubs Pns Credentials
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.NotificationHubs/namespaces/{namespaceName}/notificationHubs/{notificationHubName}/AuthorizationRules/{authorizationRuleName}/regenerateKeys
  : post:
      summary: Notification Hubs Regenerate Keys
      description: Regenerates the Primary/Secondary Keys to the NotificationHub Authorization
        Rule
      operationId: NotificationHubs_RegenerateKeys
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-notificationhubsnamespacesnamespacenamenotificationhubsnotificationhubnameauthorizationrulesauthorizationrulenameregeneratekeys-post
      parameters:
      - in: path
        name: authorizationRuleName
        description: The connection string of the NotificationHub for the specified
          authorizationRule
      - in: path
        name: namespaceName
        description: The namespace name
      - in: query
        name: No Name
      - in: path
        name: notificationHubName
        description: The notification hub name
      - in: body
        name: parameters
        description: Parameters supplied to regenerate the NotificationHub Authorization
          Rule Key
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Notification Hubs Regenerate Keys
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---