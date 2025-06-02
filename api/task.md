---
title: Task
layout: page
---

# Task Resource

The Task resource represents a cooking-related task such as prep work, cleaning, or timing-related actions.

## Properties
| Property        | Type   | Description                                         |
| --------------- | ------ | --------------------------------------------------- |
| `id`            | number | Unique task ID                                      |
| `title`         | string | Short name of the task                              |
| `description`   | string | Detailed description                                |
| `due_date`      | string | Due timestamp in ISO 8601 format                    |
| `warning`       | number | Minutes before due time to alert user               |
| `assigned_user` | string | Who the task is assigned to                         |
| `status`        | string | Task progress: 'pending', 'in progress', 'complete' |

## Example

{
  "id": 1,
  "title": "Boil water",
  "description": "Bring water to a boil for pasta",
  "due_date": "2025-06-02T18:00",
  "warning": "-15",
  "assigned_user": "lyle",
  "status": "pending"
}
