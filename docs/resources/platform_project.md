---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "harness_platform_project Resource - terraform-provider-harness"
subcategory: "NextGen"
description: |-
  Resource for creating a Harness project.
---

# harness_platform_project (Resource)

Resource for creating a Harness project.



<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `identifier` (String) Unique identifier of the resource.
- `name` (String) Name of the resource.
- `org_id` (String) Unique identifier of the organization.

### Optional

- `color` (String) Color of the project.
- `description` (String) Description of the resource.
- `tags` (Set of String) Tags to associate with the resource. Tags should be in the form `name:value`.

### Read-Only

- `id` (String) The ID of this resource.
- `modules` (Set of String) Modules in the project.


