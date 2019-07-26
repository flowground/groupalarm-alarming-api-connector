# ![LOGO](logo.png)  groupalarm Alarming API **flow**ground Connector

## Description

A generated **flow**ground connector for the  groupalarm Alarming API API (version 1.16.7).

Generated from: https://app.groupalarm.com/api/v1<br/>
Generated at: 2019-07-26T13:59:32+03:00

## API Description

The alarming service implements the alarming logic and connected items, e.g. labels or units<br/>
<br/>
# Authentication<br/>
<br/>
<!-- ReDoc-Inject: <security-definitions> --><br/>

## Authorization

Supported authorization schemes:
- API Key
- API Key

## Actions

### CreateAlarm
> Creates an alarm for an event and calculate required user for a notification<br/>

*Tags:* `alarm`

### GetAlarm
> Returns an alarm payload for requested alarm id<br/>

*Tags:* `alarm`

#### Input Parameters
* `alarmID` - _required_

### CloseAlarm
> Closes the alarm with the passed alarm id<br/>

*Tags:* `alarm`

#### Input Parameters
* `alarmID` - _required_

### PreviewAlarm
> Closes the alarm with the passed alarm id<br/>

*Tags:* `alarm`

#### Input Parameters
* `alarmID` - _required_
* `scenarioID` - _required_

### GetAlarms
> Returns all alarms<br/>

*Tags:* `alarm`

#### Input Parameters
* `organization` - _required_ - id of organization<br/>
* `limit` - _optional_ - limits alarm list output to passed amount.<br/>
* `offset` - _optional_ - defines the offset for pagination<br/>
* `event` - _optional_ - id of an event, to get all alarms for this event<br/>

### CreateAlarmTemplate
> Creates an alarm template with the passed parameters<br/>

*Tags:* `alarm`

#### Input Parameters
* `template` - _required_ - template payload<br/>

### GetAlarmTemplate
> Returns a specific alarm template for passed template id<br/>

*Tags:* `alarm`

#### Input Parameters
* `id` - _required_ - id of the template<br/>
* `organization_id` - _required_ - id of organization<br/>

### UpdateAlarmTemplate
> Updates an alarm template with the passed parameters<br/>

*Tags:* `alarm`

#### Input Parameters
* `id` - _required_ - id of the alarm template<br/>
* `template` - _required_ - template payload<br/>

### DeleteAlarmTemplate
> Updates an alarm template with the passed parameters<br/>

*Tags:* `alarm`

#### Input Parameters
* `id` - _required_ - id of the alarm template<br/>

### GetAlarmTemplates
> Returns all alarm templates for passed organization id<br/>

*Tags:* `alarm`

#### Input Parameters
* `organization_id` - _required_ - id of organization<br/>

### CreateEvent
> Creates an event with the passed event payload<br/>

*Tags:* `event`

### GetEvent
> Creates an event with the passed event ID<br/>

*Tags:* `event`

#### Input Parameters
* `eventID` - _required_

### CloseEvent
> Closes an event with the passed event ID<br/>

*Tags:* `event`

#### Input Parameters
* `eventID` - _required_

### GetEvents
> Returns paginated events of a passed organization<br/>

*Tags:* `event`

#### Input Parameters
* `organization` - _required_ - ID of an organization<br/>
* `limit` - _optional_ - max. amount of entries in list<br/>
* `offset` - _optional_ - amount of entries to skip<br/>

### GetOpenEvents
> Returns all open events of a passed organization<br/>

*Tags:* `event`

#### Input Parameters
* `organization` - _required_ - ID of an organization<br/>

### CreateLabel
> Creates a new label with the passed label payload parameters<br/>

*Tags:* `labels`

### GetLabel
> Returns a specific label with passed ID<br/>

*Tags:* `labels`

#### Input Parameters
* `labelID` - _required_

### UpdateLabel
> Updates a specific label by a passed label ID and a label payload<br/>

*Tags:* `labels`

#### Input Parameters
* `labelID` - _required_

### DeleteLabel
> Deletes the label with passed ID<br/>

*Tags:* `labels`

#### Input Parameters
* `labelID` - _required_

### AssignLabel
> Assignes a user to a label<br/>

*Tags:* `labels`

#### Input Parameters
* `labelID` - _required_
* `userID` - _required_

### UnassignLabel
> Unassignes a user from a label<br/>

*Tags:* `labels`

#### Input Parameters
* `labelID` - _required_
* `userID` - _required_

### GetLabels
> Get all labels for queried organization<br/>

*Tags:* `labels`

#### Input Parameters
* `organization` - _required_ - id of an organization<br/>
* `user` - _optional_ - id of an user, e.g. for user label assignment<br/>

### GetLabelsCSV
> Get all labels for queried organization<br/>

*Tags:* `labels`

#### Input Parameters
* `organizationID` - _required_ - id of an organization<br/>

### ImportLabels
> Imports multiple labels for the passed organization<br/>

*Tags:* `labels`

#### Input Parameters
* `organizationID` - _required_ - id of an organization<br/>

### GetStrength
> Get label to strength configuration for passed organization<br/>

*Tags:* `strength`

#### Input Parameters
* `organization` - _required_ - id of an organization<br/>

### UpsertStrength
> Creates a new or changes an existing strength configuration for passed organization<br/>

*Tags:* `strength`

#### Input Parameters
* `organization` - _required_ - id of an organization<br/>

### GetUserRanks
> Get all assigned ranks for every user of the passed organization<br/>

*Tags:* `strength`

#### Input Parameters
* `organization` - _required_ - id of an organization<br/>

### AssignUserRank
> Assing a rank to passed user<br/>

*Tags:* `strength`

#### Input Parameters
* `organization` - _required_ - id of an organization<br/>

### CreateScenario
> Creates a scenario with the passed parameters of a scenario payload<br/>

*Tags:* `scenario`

### GetScenario
> Returns a specific scenario payload for a scenario with passed ID<br/>

*Tags:* `scenario`

#### Input Parameters
* `scenarioID` - _required_

### UpdateScenario
> Updates an existing scenario with passed scenario ID and scenario payload<br/>

*Tags:* `scenario`

#### Input Parameters
* `scenarioID` - _required_

### DeleteScenario
> Deletes an existing scenario with passed scenario ID<br/>

*Tags:* `scenario`

#### Input Parameters
* `scenarioID` - _required_

### GetScenarios
> Returns all scenarios in the organization with the passed ID<br/>

*Tags:* `scenario`

#### Input Parameters
* `organizationID` - _required_

### GetSchedules
> Get all shift schedules for queried organization<br/>

*Tags:* `schedules`

#### Input Parameters
* `organization` - _required_ - id of an organization<br/>

### CreateSchedule
> Create a new shift schedule<br/>

*Tags:* `schedules`

### GetSchedules
> Get a single shift schedule<br/>

*Tags:* `schedules`

#### Input Parameters
* `id` - _required_ - id of a shift schedule<br/>

### UpdateSchedule
> Update an existing shift schedule<br/>

*Tags:* `schedules`

#### Input Parameters
* `id` - _required_ - id of a shift schedule<br/>

### DeleteSchedule
> Delete an existing shift schedule<br/>

*Tags:* `schedules`

#### Input Parameters
* `id` - _required_ - id of a shift schedule<br/>

### CreateUnit
> Creates an unit with passed unit payload<br/>

*Tags:* `units`

### GetUnit
> Returns a specific unit with the passed unit ID<br/>

*Tags:* `units`

#### Input Parameters
* `unitID` - _required_

### UpdateUnit
> Updates a specific unit by a passed unit ID and a unit creation payload<br/>

*Tags:* `units`

#### Input Parameters
* `unitID` - _required_

### DeleteUnit
> Deletes the unit with the passed unit ID<br/>

*Tags:* `units`

#### Input Parameters
* `unitID` - _required_

### GetUnits
> Returns all units of a passed organization<br/>

*Tags:* `units`

#### Input Parameters
* `organization` - _required_

## License

**flow**ground :- Telekom iPaaS / groupalarm-alarming-api-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
