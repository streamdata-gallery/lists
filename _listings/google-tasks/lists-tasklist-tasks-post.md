---
swagger: "2.0"
info:
  title: Google Tasks API Add Lists Task List Tasks
  description: Creates a new task on the specified task list.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /tasks/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /lists/{tasklist}/tasks:
    post:
      summary: Add Lists Task List Tasks
      description: Creates a new task on the specified task list
      operationId: tasks.tasks.insert
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: parent
        description: Parent task identifier
      - in: query
        name: previous
        description: Previous sibling task identifier
      - in: path
        name: tasklist
        description: Task list identifier
      responses:
        200:
          description: OK
      tags:
      - lists
      - task
      - list
      - tasks
definitions:
  Task:
    properties:
      completed:
        description: This is a default description.
        type: put
      deleted:
        description: This is a default description.
        type: put
      due:
        description: This is a default description.
        type: put
      etag:
        description: This is a default description.
        type: put
      hidden:
        description: This is a default description.
        type: put
      id:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      links:
        description: This is a default description.
        type: put
      notes:
        description: This is a default description.
        type: put
      parent:
        description: This is a default description.
        type: put
  TaskList:
    properties:
      etag:
        description: This is a default description.
        type: put
      id:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      selfLink:
        description: This is a default description.
        type: put
      title:
        description: This is a default description.
        type: put
      updated:
        description: This is a default description.
        type: put
  TaskLists:
    properties:
      etag:
        description: This is a default description.
        type: put
      items:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      nextPageToken:
        description: This is a default description.
        type: put
  Tasks:
    properties:
      etag:
        description: This is a default description.
        type: put
      items:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      nextPageToken:
        description: This is a default description.
        type: put
x-collection-name: Google Tasks
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