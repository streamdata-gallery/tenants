---
swagger: "2.0"
x-collection-name: Azure API Management
x-complete: 0
info:
  title: Azure API Management API TenantPolicy Get
  description: Get the global policy configuration of the tenant.
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
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/tenant/access
  : get:
      summary: TenantAccess Get
      description: Get tenant access information details.
      operationId: TenantAccess_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenametenantaccess-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Tenants
    patch:
      summary: TenantAccess Update
      description: Update tenant access information details.
      operationId: TenantAccess_Update
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenametenantaccess-patch
      parameters:
      - in: header
        name: If-Match
        description: The entity state (Etag) version of the tenant access settings
          to update
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Parameters
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Tenants
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/tenant/access/regeneratePrimaryKey
  : post:
      summary: TenantAccess RegeneratePrimaryKey
      description: Regenerate primary access key.
      operationId: TenantAccess_RegeneratePrimaryKey
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenametenantaccessregenerateprimarykey-post
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Tenants
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/tenant/access/regenerateSecondaryKey
  : post:
      summary: TenantAccess RegenerateSecondaryKey
      description: Regenerate secondary access key.
      operationId: TenantAccess_RegenerateSecondaryKey
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenametenantaccessregeneratesecondarykey-post
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Tenants
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/tenant/access/git
  : get:
      summary: TenantAccessGit Get
      description: Gets the Git access configuration for the tenant.
      operationId: TenantAccessGit_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenametenantaccessgit-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Tenants
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/tenant/access/git/regeneratePrimaryKey
  : post:
      summary: TenantAccessGit RegeneratePrimaryKey
      description: Regenerate primary access key for GIT.
      operationId: TenantAccessGit_RegeneratePrimaryKey
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenametenantaccessgitregenerateprimarykey-post
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Tenants
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/tenant/access/git/regenerateSecondaryKey
  : post:
      summary: TenantAccessGit RegenerateSecondaryKey
      description: Regenerate secondary access key for GIT.
      operationId: TenantAccessGit_RegenerateSecondaryKey
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenametenantaccessgitregeneratesecondarykey-post
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Tenants
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/tenant/configuration/deploy
  : post:
      summary: TenantConfiguration Deploy
      description: This operation applies changes from the specified Git branch to
        the configuration database. This is a long running operation and could take
        several minutes to complete.
      operationId: TenantConfiguration_Deploy
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenametenantconfigurationdeploy-post
      parameters:
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Deploy Configuration parameters
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Tenants
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/tenant/configuration/save
  : post:
      summary: TenantConfiguration Save
      description: This operation creates a commit with the current configuration
        snapshot to the specified branch in the repository. This is a long running
        operation and could take several minutes to complete.
      operationId: TenantConfiguration_Save
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenametenantconfigurationsave-post
      parameters:
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Save Configuration parameters
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Tenants
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/tenant/configuration/validate
  : post:
      summary: TenantConfiguration Validate
      description: This operation validates the changes in the specified Git branch.
        This is a long running operation and could take several minutes to complete.
      operationId: TenantConfiguration_Validate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenametenantconfigurationvalidate-post
      parameters:
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Validate Configuration parameters
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Tenants
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/tenant/configuration/syncState
  : get:
      summary: TenantConfigurationSyncState Get
      description: Gets the status of the most recent synchronization between the
        configuration database and the Git repository.
      operationId: TenantConfigurationSyncState_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenametenantconfigurationsyncstate-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Tenants
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/tenant/policy
  : get:
      summary: TenantPolicy Get
      description: Get the global policy configuration of the tenant.
      operationId: TenantPolicy_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenametenantpolicy-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Tenant Policy
    put:
      summary: TenantPolicy CreateOrUpdate
      description: Creates or updates global policy configuration for the tenant.
      operationId: TenantPolicy_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenametenantpolicy-put
      parameters:
      - in: header
        name: If-Match
        description: The entity state (Etag) version of the tenant policy to update
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The policy content details
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Tenant Policy
    delete:
      summary: TenantPolicy Delete
      description: Deletes the global tenant policy configuration.
      operationId: TenantPolicy_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenametenantpolicy-delete
      parameters:
      - in: header
        name: If-Match
        description: The entity state (Etag) version of the tenant policy to update
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Tenant Policy
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