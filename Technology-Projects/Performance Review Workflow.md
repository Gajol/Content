# Performance Review Workflow

Simple Workflow Manaagement

Goal:  Create a short-term solution that provides key functionality.

| Feature                 | Platform           | Notes                                                        |
| ----------------------- | ------------------ | ------------------------------------------------------------ |
| Tasking                 | ServiceNow         | Every employee is assigned a task to complete their perforamnce and evaluation review (PER). |
| Worklow                 | ServiceNow         | The PER tasking is tracked in a basic workflow to understand the current state of the employee's PER |
| Analytics               | ServiceNow         | Each workflow has metadata to allow for analytics based on organization structure (directorate, branch, supervisor). |
| Workflow Administration | ServiceNow         | HR employees can manage requests to create, delete, revoke, roll-back PER workflows.   Requests are received through ServiceNow self-administration portal (ServicePlus) |
| PER records management  | Productivity Tools | Individual PER records (PDF document) are manually stored in the corporate repository (manual Put-Away). |
|                         |                    |                                                              |



PER Template:  Template stored centrally and available to all employees.

Task: Every employee receives a task.  The task should describe the procedure (how to fulfil the task) and can also be a checklist. 

Woirkflow: General workflow is in the following stages:

employee-supervisor stage:   tasks assigned to employee and their supervisor to complete the PER.  Upon completion the PER (a PDF document) is attached to the ServiceNow workflow.  

HR-talent-management stage:  HR TM reviews, approves and closes the tasking.  The attached PER is filed in the appropriate corporate repository.   The HR application is updated as appropriate the PER results (PER score).

# Creating Tasks

Concept:

Someone will provide one or more lists of all the emplooyees to have PER reviews.   The list will include all the information needed to create the task.  This might include:

- employee:  name, id, email
- supervisor name:
- hr tm prime or group: 

Options:

ServiceNow Scripts:  [Scripting Best Practices](https://developer.servicenow.com/dev.do#!/guides/tokyo/now-platform/tpb-guide/scripting_technical_best_practices)

- [SNOW - Scripting Fundamentals](https://www.servicenow.com/services/training-and-certification/scripting-in-servicenow-training.html)
- [SNOW - Server-Side Scripting](https://developer.servicenow.com/dev.do#!/learn/learning-plans/tokyo/new_to_servicenow/app_store_learnv2_scripting_tokyo_introduction_to_server_side_scripting)
- [Glide Record Script Examples](https://www.servicenowelite.com/blog/2019/9/29/gliderecord-scripting)
- [Client Script Examples](https://interviewquestions.guru/servicenow-client-script/)

### Development Steps

- whiteboard & paper design of workflow
- servicenow stuff:
  1. extend task table for PER

Glide Functionality

- Create a Javascript script that reads a CSV file and creates record in the "PER Task Table"

Workflow

From ServiceNow Tokyo onwards "Workflow is legacy" and the new product is "Flow Designer"

Challenge:

- Glide: How to read a local desktop file or server-side file

Vaccination Attestation:  How did this one get done?

# Resources

https://snprotips.com/ - also author this [*book*](https://learning.oreilly.com/library/view/learning-servicenow/9781788837040/)