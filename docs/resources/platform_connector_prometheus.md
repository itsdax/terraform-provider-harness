---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "harness_platform_connector_prometheus Resource - terraform-provider-harness"
subcategory: "NextGen"
description: |-
  Resource for creating a Prometheus connector.
---

# harness_platform_connector_prometheus (Resource)

Resource for creating a Prometheus connector.



<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `identifier` (String) Unique identifier of the resource.
- `name` (String) Name of the resource.
- `url` (String) Url of the Prometheus server.

### Optional

- `delegate_selectors` (Set of String) Connect using only the delegates which have these tags.
- `description` (String) Description of the resource.
- `org_id` (String) Unique identifier of the organization.
- `project_id` (String) Unique identifier of the project.
- `tags` (Set of String) Tags to associate with the resource. Tags should be in the form `name:value`.

### Read-Only

- `id` (String) The ID of this resource.


