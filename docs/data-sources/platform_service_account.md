---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "harness_platform_service_account Data Source - terraform-provider-harness"
subcategory: "NextGen"
description: |-
  Data source for retrieving service account.
---

# harness_platform_service_account (Data Source)

Data source for retrieving service account.



<!-- schema generated by tfplugindocs -->
## Schema

### Optional

- `identifier` (String) Unique identifier of the resource.
- `name` (String) Name of the resource.
- `org_id` (String) Unique identifier of the organization.
- `project_id` (String) Unique identifier of the project.

### Read-Only

- `account_id` (String) Account Identifier for the Entity.
- `description` (String) Description of the resource.
- `email` (String) Email of the Service Account.
- `id` (String) The ID of this resource.
- `tags` (Set of String) Tags to associate with the resource. Tags should be in the form `name:value`.


