# School 21 GQL Operations

## Index

* [getUserRestrictionsInfo](#getUserRestrictionsInfo)
* [userRoleLoaderGetRoles](#userRoleLoaderGetRoles)
* [getUserFeatureFlags](#getUserFeatureFlags)
* [getStudentIsDeadlinesEnabled](#getStudentIsDeadlinesEnabled)
* [getTournamentNotificationResults](#getTournamentNotificationResults)
* [deadlinesGetStudentData](#deadlinesGetStudentData)
* [deadlineReminderGetClosestDeadlinePopup](#deadlineReminderGetClosestDeadlinePopup)
* [eventsWithoutFeedback](#eventsWithoutFeedback)
* [getSaleProgressPercentages](#getSaleProgressPercentages)
* [getUserNotificationsCount](#getUserNotificationsCount)
* [dashboardHeaderGetInfo](#dashboardHeaderGetInfo)
* [deadlinesGetDeadlines](#deadlinesGetDeadlines)
* [getDashboardBuildings](#getDashboardBuildings)
* [widgetAchievementsGetLastBadges](#widgetAchievementsGetLastBadges)
* [getDashboardWorkstation](#getDashboardWorkstation)
* [getAsapWidgets](#getAsapWidgets)
* [getCurrentUser](#getCurrentUser)
* [calendarGetMyBookings](#calendarGetMyBookings)
* [calendarGetMyReviews](#calendarGetMyReviews)
* [calendarDeleteEventSlot](#calendarDeleteEventSlot)
* [getAgendaP2P](#getAgendaP2P)
* [createFilledChecklist](#createFilledChecklist)
* [getCredentialsByLogin](#getCredentialsByLogin)
* [publicProfileGetPersonalInfo](#publicProfileGetPersonalInfo)
* [getDismissInfoByStudentId](#getDismissInfoByStudentId)
* [publicProfileGetCoalition](#publicProfileGetCoalition)
* [publicProfileGetAchievements](#publicProfileGetAchievements)
* [publicProfileLoadAverageLogtime](#publicProfileLoadAverageLogtime)
* [publicProfileLoadStageGroups](#publicProfileLoadStageGroups)
* [publicProfileGetSoftSkills](#publicProfileGetSoftSkills)
* [publicProfileGetXpGraph](#publicProfileGetXpGraph)
* [publicProfileGetStudentTraffic](#publicProfileGetStudentTraffic)
* [getUserNotifications](#getUserNotifications)
* [readUserNotifications](#readUserNotifications)
* [saveFilledChecklist](#saveFilledChecklist)
* [getInvitationsCount](#getInvitationsCount)
* [getStudentCurrentProjects](#getStudentCurrentProjects)
* [getAvailableCodeReviewProjects](#getAvailableCodeReviewProjects)
* [getFirstRoundCodeReviewProjects](#getFirstRoundCodeReviewProjects)
* [getSecondRoundCodeReviewProjects](#getSecondRoundCodeReviewProjects)
* [getCodeReviewProjectInfo](#getCodeReviewProjectInfo)
* [getCodeReviewMyStudent](#getCodeReviewMyStudent)
* [calendarGetStudentCodeReviews](#calendarGetStudentCodeReviews)
* [calendarGetCodeReviewData](#calendarGetCodeReviewData)
* [calendarAddCodeReviewToEventSlot](#calendarAddCodeReviewToEventSlot)
* [calendarAddBookingToEventSlot](#calendarAddBookingToEventSlot)
* [getCodeReviewPointChargedOff](#getCodeReviewPointChargedOff)
* [getProjectConsistencyInfo](#getProjectConsistencyInfo)
* [getProjectInfo](#getProjectInfo)
* [getProjectAttemptEvaluationsInfo](#getProjectAttemptEvaluationsInfo)
* [getProjectGitlabStatus](#getProjectGitlabStatus)
* [calendarGetModule](#calendarGetModule)
* [calendarGetNameLessStudentTimeslotsForReview](#calendarGetNameLessStudentTimeslotsForReview)
* [bonusesGetBadgesWithFakePublicProfile](#bonusesGetBadgesWithFakePublicProfile)
* [getCampusCurrentUser](#getCampusCurrentUser)
* [getCampusWorkstation](#getCampusWorkstation)
* [getCampusBuildings](#getCampusBuildings)
* [getCampusPlanOccupied](#getCampusPlanOccupied)
* [calendarAddEvent](#calendarAddEvent)
* [getActivityTypes](#getActivityTypes)
* [getStageInfo](#getStageInfo)
* [getUsers](#getUsers)
* [getMySuggestedActivities](#getMySuggestedActivities)
* [subscribeToEvent](#subscribeToEvent)
* [unsubscribeFromEvent](#unsubscribeFromEvent)
* [publicProfileGetProjects](#publicProfileGetProjects)
* [publicProfileGetCredentialsByLogin](#publicProfileGetCredentialsByLogin)
* [bonusesGetUserIdByLogin](#bonusesGetUserIdByLogin)
* [competitionCoalitionGetUserTournament](#competitionCoalitionGetUserTournament)
* [competitionCoalitionGetMyCoalitionMembers](#competitionCoalitionGetMyCoalitionMembers)
* [getPenaltyList](#getPenaltyList)
* [getPenaltiesCount](#getPenaltiesCount)
* [getGraphCurrentType](#getGraphCurrentType)
* [getGraphBasisGoals](#getGraphBasisGoals)
* [getTasks](#getTasks)
* [getGitlabLink](#getGitlabLink)
* [createFeedbackOnEvaluation](#createFeedbackOnEvaluation)
* [getProjectTeamWithMembers](#getProjectTeamWithMembers)
* [getIsDisbandRequestAlreadySent](#getIsDisbandRequestAlreadySent)
* [getGitlabSettingsToken](#getGitlabSettingsToken)
* [cancelInvitation](#cancelInvitation)
* [getAvailableStudentsForTeams](#getAvailableStudentsForTeams)
* [sendInvitation](#sendInvitation)
* [removeP2P](#removeP2P)
* [calendarGetExams](#calendarGetExams)
* [userGetTheme](#userGetTheme)
* [getAllInCompletedStudentFeedbackPopup](#getAllInCompletedStudentFeedbackPopup)
* [getIsHonorRatingNeeded](#getIsHonorRatingNeeded)
* [getSearchHistory](#getSearchHistory)
* [getUpcomingEvents](#getUpcomingEvents)
* [getAgendaEvents](#getAgendaEvents)
* [getStudentStageGroupS21](#getStudentStageGroupS21)
* [calendarGetEvents](#calendarGetEvents)
* [getPenaltyReasons](#getPenaltyReasons)

## Operations

### getUserRestrictionsInfo

<details>
<summary> Query </summary>

```
query getUserRestrictionsInfo {
  school21 {
    getUserRestrictions {
      restrictionId
      restrictionType
      userId
      schoolId
      isActive
      createdTs
      updatedTs
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "school21": {
                    "$ref": "#/definitions/School21"
                }
            },
            "required": [
                "school21"
            ],
            "title": "Data"
        },
        "School21": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getUserRestrictions": {
                    "type": "array",
                    "items": {}
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getUserRestrictions"
            ],
            "title": "School21"
        }
    }
}

```

</details>

[[Index](#index)]

### userRoleLoaderGetRoles

<details>
<summary> Query </summary>

```
query userRoleLoaderGetRoles {
  user {
    getCurrentUser {
      functionalRoles {
        code
        __typename
      }
      id
      studentRoles {
        id
        school {
          id
          shortName
          organizationType
          __typename
        }
        status
        __typename
      }
      userSchoolPermissions {
        schoolId
        permissions
        __typename
      }
      systemAdminRole {
        id
        __typename
      }
      businessAdminRolesV2 {
        id
        school {
          id
          organizationType
          __typename
        }
        orgUnitId
        __typename
      }
      __typename
    }
    getCurrentUserSchoolRoles {
      schoolId
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "user": {
                    "$ref": "#/definitions/User"
                }
            },
            "required": [
                "user"
            ],
            "title": "Data"
        },
        "User": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getCurrentUser": {
                    "$ref": "#/definitions/GetCurrentUser"
                },
                "getCurrentUserSchoolRoles": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/GetCurrentUserSchoolRole"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getCurrentUser",
                "getCurrentUserSchoolRoles"
            ],
            "title": "User"
        },
        "GetCurrentUser": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "functionalRoles": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/FunctionalRole"
                    }
                },
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "studentRoles": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/StudentRole"
                    }
                },
                "userSchoolPermissions": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/UserSchoolPermission"
                    }
                },
                "systemAdminRole": {
                    "type": "null"
                },
                "businessAdminRolesV2": {
                    "type": "array",
                    "items": {}
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "businessAdminRolesV2",
                "functionalRoles",
                "id",
                "studentRoles",
                "systemAdminRole",
                "userSchoolPermissions"
            ],
            "title": "GetCurrentUser"
        },
        "FunctionalRole": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "code": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "code"
            ],
            "title": "FunctionalRole"
        },
        "StudentRole": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "school": {
                    "$ref": "#/definitions/School"
                },
                "status": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "school",
                "status"
            ],
            "title": "StudentRole"
        },
        "School": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "shortName": {
                    "type": "string"
                },
                "organizationType": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "organizationType",
                "shortName"
            ],
            "title": "School"
        },
        "UserSchoolPermission": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "schoolId": {
                    "type": "string",
                    "format": "uuid"
                },
                "permissions": {
                    "type": "array",
                    "items": {
                        "type": "string"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "permissions",
                "schoolId"
            ],
            "title": "UserSchoolPermission"
        },
        "GetCurrentUserSchoolRole": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "schoolId": {
                    "type": "string",
                    "format": "uuid"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "schoolId"
            ],
            "title": "GetCurrentUserSchoolRole"
        }
    }
}

```

</details>

[[Index](#index)]

### getUserFeatureFlags

<details>
<summary> Query </summary>

```
query getUserFeatureFlags($entityId: String!) {
  user {
    getAllBackendConfigurations: getAllBackendConfigurationsV2(entityId: $entityId) {
      propertyCode
      value
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "entityId": {
                    "type": "string",
                    "format": "uuid"
                },
                "entityIdList": {
                    "type": "array",
                    "items": {
                        "type": "string",
                        "format": "uuid"
                    }
                }
            },
            "required": [],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "user": {
                    "$ref": "#/definitions/User"
                }
            },
            "required": [
                "user"
            ],
            "title": "Data"
        },
        "User": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getAllBackendConfigurations": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/GetAllBackendConfiguration"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getAllBackendConfigurations"
            ],
            "title": "User"
        },
        "GetAllBackendConfiguration": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "propertyCode": {
                    "type": "string"
                },
                "value": {
                    "type": "string",
                    "qt-uri-protocols": [
                        "https"
                    ]
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "propertyCode",
                "value"
            ],
            "title": "GetAllBackendConfiguration"
        }
    }
}

```

</details>

[[Index](#index)]

### getStudentIsDeadlinesEnabled

<details>
<summary> Query </summary>

```
query getStudentIsDeadlinesEnabled {
  student {
    isDeadlinesEnabled
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "isDeadlinesEnabled": {
                    "type": "boolean"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "isDeadlinesEnabled"
            ],
            "title": "Student"
        }
    }
}

```

</details>

[[Index](#index)]

### getTournamentNotificationResults

<details>
<summary> Query </summary>

```
query getTournamentNotificationResults {
  student {
    getTournamentResults(isShown: false) {
      id
      power
      coalitionRank
      userRank
      firstCoalitionName
      coalitionName
      timeClosed
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getTournamentResults": {
                    "type": "array",
                    "items": {}
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getTournamentResults"
            ],
            "title": "Student"
        }
    }
}

```

</details>

[[Index](#index)]

### deadlinesGetStudentData

<details>
<summary> Query </summary>

```
query deadlinesGetStudentData {
  student {
    getStudentProfile {
      user {
        id
        login
        firstName
        middleName
        lastName
        __typename
      }
      __typename
    }
    getExperience {
      id
      value
      level {
        id
        range {
          id
          levelCode
          rightBorder
          leftBorder
          __typename
        }
        __typename
      }
      __typename
    }
    getExperienceHistory {
      id
      awardDate
      experienceReceived
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getStudentProfile": {
                    "$ref": "#/definitions/GetStudentProfile"
                },
                "getExperience": {
                    "$ref": "#/definitions/GetExperience"
                },
                "getExperienceHistory": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/GetExperienceHistory"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getExperience",
                "getExperienceHistory",
                "getStudentProfile"
            ],
            "title": "Student"
        },
        "GetExperience": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "value": {
                    "type": "integer"
                },
                "level": {
                    "$ref": "#/definitions/Level"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "level",
                "value"
            ],
            "title": "GetExperience"
        },
        "Level": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "integer"
                },
                "range": {
                    "$ref": "#/definitions/Range"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "range"
            ],
            "title": "Level"
        },
        "Range": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "levelCode": {
                    "type": "integer"
                },
                "rightBorder": {
                    "type": "integer"
                },
                "leftBorder": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "leftBorder",
                "levelCode",
                "rightBorder"
            ],
            "title": "Range"
        },
        "GetExperienceHistory": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "awardDate": {
                    "type": "string",
                    "format": "date-time"
                },
                "experienceReceived": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "awardDate",
                "experienceReceived",
                "id"
            ],
            "title": "GetExperienceHistory"
        },
        "GetStudentProfile": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "user": {
                    "$ref": "#/definitions/User"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "user"
            ],
            "title": "GetStudentProfile"
        },
        "User": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "login": {
                    "type": "string"
                },
                "firstName": {
                    "type": "string"
                },
                "middleName": {
                    "type": "string"
                },
                "lastName": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "firstName",
                "id",
                "lastName",
                "login",
                "middleName"
            ],
            "title": "User"
        }
    }
}

```

</details>

[[Index](#index)]

### deadlineReminderGetClosestDeadlinePopup

<details>
<summary> Query </summary>

```
query deadlineReminderGetClosestDeadlinePopup {
  student {
    getClosestDeadlinePopup {
      deadline {
        ...DeadlineData
        __typename
      }
      deadlineGoal {
        ...DeadlineGoalData
        __typename
      }
      shiftCount
      __typename
    }
    __typename
  }
}

fragment DeadlineData on Deadline {
  deadlineId
  description
  comment
  deadlineToDaysArray
  deadlineTs
  createTs
  updateTs
  status
  rules {
    logicalOperatorId
    rulesInGroup {
      logicalOperatorId
      value {
        fieldId
        subFieldKey
        operator
        value
        __typename
      }
      __typename
    }
    __typename
  }
  __typename
}

fragment DeadlineGoalData on DeadlineGoal {
  goalProjects {
    studentGoalId
    project {
      goalName
      goalId
      __typename
    }
    status
    executionType
    finalPercentage
    finalPoint
    pointTask
    __typename
  }
  goalCourses {
    ...GoalCourse
    __typename
  }
  levels {
    ...Level
    __typename
  }
  __typename
}

fragment GoalCourse on CourseCoverInformation {
  localCourseId
  courseName
  courseType
  experienceFact
  finalPercentage
  displayedCourseStatus
  __typename
}

fragment Level on ExperienceLevelRange {
  id
  level
  levelCode
  leftBorder
  rightBorder
  __typename
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getClosestDeadlinePopup": {
                    "type": "null"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getClosestDeadlinePopup"
            ],
            "title": "Student"
        }
    }
}

```

</details>

[[Index](#index)]

### eventsWithoutFeedback

<details>
<summary> Query </summary>

```
query eventsWithoutFeedback($from: DateTime!, $to: DateTime!) {
  student {
    getCalendarEventsWithoutFeedback(from: $from, to: $to) {
      id
      activity {
        eventId
        name
        endDate
        __typename
      }
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "from": {
                    "type": "string",
                    "format": "date-time"
                },
                "to": {
                    "type": "string",
                    "format": "date-time"
                }
            },
            "required": [
                "from",
                "to"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getCalendarEventsWithoutFeedback": {
                    "type": "array",
                    "items": {}
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getCalendarEventsWithoutFeedback"
            ],
            "title": "Student"
        }
    }
}

```

</details>

[[Index](#index)]

### getSaleProgressPercentages

<details>
<summary> Query </summary>

```
query getSaleProgressPercentages {
  school21 {
    getSaleProgressPercentages {
      ...RpSaleInfo
      __typename
    }
    __typename
  }
}

fragment RpSaleInfo on RpSaleProgress {
  rpType
  progressPercentage
  __typename
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "school21": {
                    "$ref": "#/definitions/School21"
                }
            },
            "required": [
                "school21"
            ],
            "title": "Data"
        },
        "School21": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getSaleProgressPercentages": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/GetSaleProgressPercentage"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getSaleProgressPercentages"
            ],
            "title": "School21"
        },
        "GetSaleProgressPercentage": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "rpType": {
                    "type": "string"
                },
                "progressPercentage": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "progressPercentage",
                "rpType"
            ],
            "title": "GetSaleProgressPercentage"
        }
    }
}

```

</details>

[[Index](#index)]

### getUserNotificationsCount

<details>
<summary> Query </summary>

```
query getUserNotificationsCount($wasReadIncluded: Boolean) {
  student {
    getS21NotificationsCount(wasReadIncluded: $wasReadIncluded)
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "wasReadIncluded": {
                    "type": "boolean"
                }
            },
            "required": [
                "wasReadIncluded"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getS21NotificationsCount": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getS21NotificationsCount"
            ],
            "title": "Student"
        }
    }
}

```

</details>

[[Index](#index)]

### dashboardHeaderGetInfo

<details>
<summary> Query </summary>

```
query dashboardHeaderGetInfo {
  user {
    getCurrentUser {
      id
      login
      avatarUrl
      firstName
      middleName
      lastName
      currentSchoolStudentId
      studentRoles {
        id
        status
        school {
          id
          shortName
          __typename
        }
        __typename
      }
      __typename
    }
    __typename
  }
  student {
    getUserTournamentWidget {
      coalitionMember {
        coalition {
          avatarUrl
          color
          name
          memberCount
          __typename
        }
        currentTournamentPowerRank {
          rank
          __typename
        }
        __typename
      }
      lastTournamentResult {
        userRank
        __typename
      }
      __typename
    }
    getExperience {
      id
      value
      level {
        id
        range {
          id
          levelCode
          rightBorder
          leftBorder
          __typename
        }
        __typename
      }
      cookiesCount
      coinsCount
      codeReviewPoints
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "user": {
                    "$ref": "#/definitions/User"
                },
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student",
                "user"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getUserTournamentWidget": {
                    "$ref": "#/definitions/GetUserTournamentWidget"
                },
                "getExperience": {
                    "$ref": "#/definitions/GetExperience"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getExperience",
                "getUserTournamentWidget"
            ],
            "title": "Student"
        },
        "GetExperience": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "value": {
                    "type": "integer"
                },
                "level": {
                    "$ref": "#/definitions/Level"
                },
                "cookiesCount": {
                    "type": "integer"
                },
                "coinsCount": {
                    "type": "integer"
                },
                "codeReviewPoints": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "codeReviewPoints",
                "coinsCount",
                "cookiesCount",
                "id",
                "level",
                "value"
            ],
            "title": "GetExperience"
        },
        "Level": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "integer"
                },
                "range": {
                    "$ref": "#/definitions/Range"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "range"
            ],
            "title": "Level"
        },
        "Range": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "levelCode": {
                    "type": "integer"
                },
                "rightBorder": {
                    "type": "integer"
                },
                "leftBorder": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "leftBorder",
                "levelCode",
                "rightBorder"
            ],
            "title": "Range"
        },
        "GetUserTournamentWidget": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "coalitionMember": {
                    "$ref": "#/definitions/CoalitionMember"
                },
                "lastTournamentResult": {
                    "$ref": "#/definitions/LastTournamentResult"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "coalitionMember",
                "lastTournamentResult"
            ],
            "title": "GetUserTournamentWidget"
        },
        "CoalitionMember": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "coalition": {
                    "$ref": "#/definitions/Coalition"
                },
                "currentTournamentPowerRank": {
                    "$ref": "#/definitions/CurrentTournamentPowerRank"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "coalition",
                "currentTournamentPowerRank"
            ],
            "title": "CoalitionMember"
        },
        "Coalition": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "avatarUrl": {
                    "type": "string"
                },
                "color": {
                    "type": "string"
                },
                "name": {
                    "type": "string"
                },
                "memberCount": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "avatarUrl",
                "color",
                "memberCount",
                "name"
            ],
            "title": "Coalition"
        },
        "CurrentTournamentPowerRank": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "rank": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "rank"
            ],
            "title": "CurrentTournamentPowerRank"
        },
        "LastTournamentResult": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "userRank": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "userRank"
            ],
            "title": "LastTournamentResult"
        },
        "User": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getCurrentUser": {
                    "$ref": "#/definitions/GetCurrentUser"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getCurrentUser"
            ],
            "title": "User"
        },
        "GetCurrentUser": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "login": {
                    "type": "string"
                },
                "avatarUrl": {
                    "type": "string"
                },
                "firstName": {
                    "type": "string"
                },
                "middleName": {
                    "type": "string"
                },
                "lastName": {
                    "type": "string"
                },
                "currentSchoolStudentId": {
                    "type": "string",
                    "format": "uuid"
                },
                "studentRoles": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/StudentRole"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "avatarUrl",
                "currentSchoolStudentId",
                "firstName",
                "id",
                "lastName",
                "login",
                "middleName",
                "studentRoles"
            ],
            "title": "GetCurrentUser"
        },
        "StudentRole": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "status": {
                    "type": "string"
                },
                "school": {
                    "$ref": "#/definitions/School"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "school",
                "status"
            ],
            "title": "StudentRole"
        },
        "School": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "shortName": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "shortName"
            ],
            "title": "School"
        }
    }
}

```

</details>

[[Index](#index)]

### deadlinesGetDeadlines

<details>
<summary> Query </summary>

```
query deadlinesGetDeadlines($deadlineStatuses: [DeadlineStatus!]!, $page: PagingInput!, $deadlinesFrom: DateTime, $deadlinesTo: DateTime, $sorting: [SortingField]) {
  student {
    getDeadlines(
      deadlineStatuses: $deadlineStatuses
      page: $page
      deadlineFrom: $deadlinesFrom
      deadlineTo: $deadlinesTo
      sorting: $sorting
    ) {
      deadline {
        ...DeadlineData
        __typename
      }
      shiftRequests {
        deadlineShiftRequestId
        status
        daysToShift
        createTs
        __typename
      }
      deadlineGoal {
        ...DeadlineGoalData
        __typename
      }
      shiftCount
      __typename
    }
    __typename
  }
}

fragment DeadlineData on Deadline {
  deadlineId
  description
  comment
  deadlineToDaysArray
  deadlineTs
  createTs
  updateTs
  status
  rules {
    logicalOperatorId
    rulesInGroup {
      logicalOperatorId
      value {
        fieldId
        subFieldKey
        operator
        value
        __typename
      }
      __typename
    }
    __typename
  }
  __typename
}

fragment DeadlineGoalData on DeadlineGoal {
  goalProjects {
    studentGoalId
    project {
      goalName
      goalId
      __typename
    }
    status
    executionType
    finalPercentage
    finalPoint
    pointTask
    __typename
  }
  goalCourses {
    ...GoalCourse
    __typename
  }
  levels {
    ...Level
    __typename
  }
  __typename
}

fragment GoalCourse on CourseCoverInformation {
  localCourseId
  courseName
  courseType
  experienceFact
  finalPercentage
  displayedCourseStatus
  __typename
}

fragment Level on ExperienceLevelRange {
  id
  level
  levelCode
  leftBorder
  rightBorder
  __typename
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "page": {
                    "$ref": "#/definitions/Page"
                },
                "deadlineStatuses": {
                    "type": "array",
                    "items": {
                        "type": "string"
                    }
                },
                "sorting": {
                    "$ref": "#/definitions/Sorting"
                }
            },
            "required": [
                "deadlineStatuses",
                "page",
                "sorting"
            ],
            "title": "Variables"
        },
        "Page": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "limit": {
                    "type": "integer"
                },
                "offset": {
                    "type": "integer"
                }
            },
            "required": [
                "limit",
                "offset"
            ],
            "title": "Page"
        },
        "Sorting": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "name": {
                    "type": "string"
                },
                "asc": {
                    "type": "boolean"
                }
            },
            "required": [
                "asc",
                "name"
            ],
            "title": "Sorting"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getDeadlines": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/GetDeadline"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getDeadlines"
            ],
            "title": "Student"
        },
        "GetDeadline": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "deadline": {
                    "$ref": "#/definitions/Deadline"
                },
                "shiftRequests": {
                    "type": "array",
                    "items": {}
                },
                "deadlineGoal": {
                    "$ref": "#/definitions/DeadlineGoal"
                },
                "shiftCount": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "deadline",
                "deadlineGoal",
                "shiftCount",
                "shiftRequests"
            ],
            "title": "GetDeadline"
        },
        "Deadline": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "deadlineId": {
                    "type": "string",
                    "format": "uuid"
                },
                "description": {
                    "type": "string"
                },
                "comment": {
                    "type": "string"
                },
                "deadlineToDaysArray": {
                    "type": "array",
                    "items": {
                        "type": "integer"
                    }
                },
                "deadlineTs": {
                    "type": "string",
                    "format": "date-time"
                },
                "createTs": {
                    "type": "string",
                    "format": "date-time"
                },
                "updateTs": {
                    "anyOf": [
                        {
                            "type": "string",
                            "format": "date-time"
                        },
                        {
                            "type": "null"
                        }
                    ]
                },
                "status": {
                    "type": "string"
                },
                "rules": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/Rule"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "comment",
                "createTs",
                "deadlineId",
                "deadlineToDaysArray",
                "deadlineTs",
                "description",
                "rules",
                "status",
                "updateTs"
            ],
            "title": "Deadline"
        },
        "Rule": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "logicalOperatorId": {
                    "type": "null"
                },
                "rulesInGroup": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/RulesInGroup"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "logicalOperatorId",
                "rulesInGroup"
            ],
            "title": "Rule"
        },
        "RulesInGroup": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "logicalOperatorId": {
                    "type": "null"
                },
                "value": {
                    "$ref": "#/definitions/Value"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "logicalOperatorId",
                "value"
            ],
            "title": "RulesInGroup"
        },
        "Value": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "fieldId": {
                    "type": "string",
                    "format": "integer"
                },
                "subFieldKey": {
                    "type": "null"
                },
                "operator": {
                    "type": "string"
                },
                "value": {
                    "type": "array",
                    "items": {
                        "type": "string",
                        "format": "integer"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "fieldId",
                "operator",
                "subFieldKey",
                "value"
            ],
            "title": "Value"
        },
        "DeadlineGoal": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "goalProjects": {
                    "type": "array",
                    "items": {}
                },
                "goalCourses": {
                    "type": "array",
                    "items": {}
                },
                "levels": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/Level"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "goalCourses",
                "goalProjects",
                "levels"
            ],
            "title": "DeadlineGoal"
        },
        "Level": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "level": {
                    "type": "integer"
                },
                "levelCode": {
                    "type": "integer"
                },
                "leftBorder": {
                    "type": "integer"
                },
                "rightBorder": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "leftBorder",
                "level",
                "levelCode",
                "rightBorder"
            ],
            "title": "Level"
        }
    }
}

```

</details>

[[Index](#index)]

### getDashboardBuildings

<details>
<summary> Query </summary>

```
query getDashboardBuildings {
  student {
    getBuildings {
      id
      classrooms {
        id
        number
        __typename
      }
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getBuildings": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/GetBuilding"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getBuildings"
            ],
            "title": "Student"
        },
        "GetBuilding": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "classrooms": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/Classroom"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "classrooms",
                "id"
            ],
            "title": "GetBuilding"
        },
        "Classroom": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "number": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "number"
            ],
            "title": "Classroom"
        }
    }
}

```

</details>

[[Index](#index)]

### widgetAchievementsGetLastBadges

<details>
<summary> Query </summary>

```
query widgetAchievementsGetLastBadges($limit: Int) {
  student {
    getLastBadges(limit: $limit) {
      id
      points
      badge {
        name
        avatarUrl
        __typename
      }
      award {
        awardBounties {
          awardLevelId
          __typename
        }
        __typename
      }
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "limit": {
                    "type": "integer"
                }
            },
            "required": [
                "limit"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getLastBadges": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/GetLastBadge"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getLastBadges"
            ],
            "title": "Student"
        },
        "GetLastBadge": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "points": {
                    "type": "integer"
                },
                "badge": {
                    "$ref": "#/definitions/Badge"
                },
                "award": {
                    "$ref": "#/definitions/Award"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "award",
                "badge",
                "id",
                "points"
            ],
            "title": "GetLastBadge"
        },
        "Award": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "awardBounties": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/AwardBounty"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "awardBounties"
            ],
            "title": "Award"
        },
        "AwardBounty": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "awardLevelId": {
                    "anyOf": [
                        {
                            "type": "integer"
                        },
                        {
                            "type": "null"
                        }
                    ]
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "awardLevelId"
            ],
            "title": "AwardBounty"
        },
        "Badge": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "name": {
                    "type": "string"
                },
                "avatarUrl": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "avatarUrl",
                "name"
            ],
            "title": "Badge"
        }
    }
}

```

</details>

[[Index](#index)]

### getDashboardWorkstation

<details>
<summary> Query </summary>

```
query getDashboardWorkstation($login: String!) {
  student {
    getWorkstationByLogin(login: $login) {
      id
      classroomId
      hostName
      classroom {
        floor
        __typename
      }
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "login": {
                    "type": "string"
                }
            },
            "required": [
                "login"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getWorkstationByLogin": {
                    "type": "null"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getWorkstationByLogin"
            ],
            "title": "Student"
        }
    }
}

```

</details>

[[Index](#index)]

### getAsapWidgets

<details>
<summary> Query </summary>

```
query getAsapWidgets {
  student {
    getAsapWidgetList {
      widgetList {
        ...AsapWidget
        __typename
      }
      __typename
    }
    __typename
  }
}

fragment AsapWidget on AsapWidgetInfo {
  shortImg
  shortTitle
  shortUrl
  startDate
  finishDate
  showFinishDate
  fullTitle
  text
  fullImgUrl
  adtTypeId
  adtWidgetId
  __typename
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getAsapWidgetList": {
                    "$ref": "#/definitions/GetAsapWidgetList"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getAsapWidgetList"
            ],
            "title": "Student"
        },
        "GetAsapWidgetList": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "widgetList": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/WidgetList"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "widgetList"
            ],
            "title": "GetAsapWidgetList"
        },
        "WidgetList": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "shortImg": {
                    "type": "string"
                },
                "shortTitle": {
                    "type": "string"
                },
                "shortUrl": {
                    "type": "null"
                },
                "startDate": {
                    "type": "string",
                    "format": "date-time"
                },
                "finishDate": {
                    "type": "string",
                    "format": "date-time"
                },
                "showFinishDate": {
                    "type": "boolean"
                },
                "fullTitle": {
                    "type": "string"
                },
                "text": {
                    "type": "string"
                },
                "fullImgUrl": {
                    "type": "string"
                },
                "adtTypeId": {
                    "type": "integer"
                },
                "adtWidgetId": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "adtTypeId",
                "adtWidgetId",
                "finishDate",
                "fullImgUrl",
                "fullTitle",
                "shortImg",
                "shortTitle",
                "shortUrl",
                "showFinishDate",
                "startDate",
                "text"
            ],
            "title": "WidgetList"
        }
    }
}

```

</details>

[[Index](#index)]

### getCurrentUser

<details>
<summary> Query </summary>

```
query getCurrentUser {
  user {
    getCurrentUser {
      ...CurrentUser
      __typename
    }
    __typename
  }
  student {
    getExperience {
      ...CurrentUserExperience
      __typename
    }
    __typename
  }
}

fragment CurrentUser on User {
  id
  avatarUrl
  login
  firstName
  middleName
  lastName
  currentSchoolStudentId
  __typename
}

fragment CurrentUserExperience on UserExperience {
  id
  cookiesCount
  codeReviewPoints
  coinsCount
  level {
    id
    range {
      id
      levelCode
      __typename
    }
    __typename
  }
  __typename
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "user": {
                    "$ref": "#/definitions/User"
                },
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student",
                "user"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getExperience": {
                    "$ref": "#/definitions/GetExperience"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getExperience"
            ],
            "title": "Student"
        },
        "GetExperience": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "cookiesCount": {
                    "type": "integer"
                },
                "codeReviewPoints": {
                    "type": "integer"
                },
                "coinsCount": {
                    "type": "integer"
                },
                "level": {
                    "$ref": "#/definitions/Level"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "codeReviewPoints",
                "coinsCount",
                "cookiesCount",
                "id",
                "level"
            ],
            "title": "GetExperience"
        },
        "Level": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "integer"
                },
                "range": {
                    "$ref": "#/definitions/Range"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "range"
            ],
            "title": "Level"
        },
        "Range": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "levelCode": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "levelCode"
            ],
            "title": "Range"
        },
        "User": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getCurrentUser": {
                    "$ref": "#/definitions/GetCurrentUser"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getCurrentUser"
            ],
            "title": "User"
        },
        "GetCurrentUser": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "avatarUrl": {
                    "type": "string"
                },
                "login": {
                    "type": "string"
                },
                "firstName": {
                    "type": "string"
                },
                "middleName": {
                    "type": "string"
                },
                "lastName": {
                    "type": "string"
                },
                "currentSchoolStudentId": {
                    "type": "string",
                    "format": "uuid"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "avatarUrl",
                "currentSchoolStudentId",
                "firstName",
                "id",
                "lastName",
                "login",
                "middleName"
            ],
            "title": "GetCurrentUser"
        }
    }
}

```

</details>

[[Index](#index)]

### calendarGetMyBookings

<details>
<summary> Query </summary>

```
query calendarGetMyBookings($from: DateTime!, $to: DateTime!) {
  student {
    getMyCalendarBookings(from: $from, to: $to) {
      ...CalendarReviewBooking
      __typename
    }
    __typename
  }
}

fragment CalendarReviewBooking on CalendarBooking {
  id
  answerId
  eventSlotId
  task {
    id
    goalId
    goalName
    studentTaskAdditionalAttributes {
      cookiesCount
      __typename
    }
    assignmentType
    __typename
  }
  eventSlot {
    id
    start
    end
    event {
      eventUserRole
      __typename
    }
    __typename
  }
  verifierUser {
    ...CalendarReviewUser
    __typename
  }
  verifiableStudent {
    id
    user {
      ...CalendarReviewUser
      __typename
    }
    __typename
  }
  bookingStatus
  team {
    ...ProjectTeamMembers
    __typename
  }
  isOnline
  vcLinkUrl
  __typename
}

fragment CalendarReviewUser on User {
  id
  login
  __typename
}

fragment ProjectTeamMembers on ProjectTeamMembers {
  id
  teamLead {
    ...ProjectTeamMember
    __typename
  }
  members {
    ...ProjectTeamMember
    __typename
  }
  invitedUsers {
    ...ProjectTeamMember
    __typename
  }
  teamName
  teamStatus
  minTeamMemberCount
  maxTeamMemberCount
  __typename
}

fragment ProjectTeamMember on User {
  id
  avatarUrl
  login
  userExperience {
    level {
      id
      range {
        levelCode
        __typename
      }
      __typename
    }
    cookiesCount
    codeReviewPoints
    __typename
  }
  __typename
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "from": {
                    "type": "string",
                    "format": "date-time"
                },
                "to": {
                    "type": "string",
                    "format": "date-time"
                }
            },
            "required": [
                "from",
                "to"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getMyCalendarBookings": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/GetMyCalendarBooking"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getMyCalendarBookings"
            ],
            "title": "Student"
        },
        "GetMyCalendarBooking": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "answerId": {
                    "type": "string",
                    "format": "integer"
                },
                "eventSlotId": {
                    "type": "string",
                    "format": "integer"
                },
                "task": {
                    "$ref": "#/definitions/Task"
                },
                "eventSlot": {
                    "$ref": "#/definitions/EventSlot"
                },
                "verifierUser": {
                    "$ref": "#/definitions/User"
                },
                "verifiableStudent": {
                    "$ref": "#/definitions/VerifiableStudent"
                },
                "bookingStatus": {
                    "type": "string"
                },
                "team": {
                    "type": "null"
                },
                "isOnline": {
                    "type": "boolean"
                },
                "vcLinkUrl": {
                    "type": "null"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "answerId",
                "bookingStatus",
                "eventSlot",
                "eventSlotId",
                "id",
                "isOnline",
                "task",
                "team",
                "vcLinkUrl",
                "verifiableStudent",
                "verifierUser"
            ],
            "title": "GetMyCalendarBooking"
        },
        "EventSlot": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "start": {
                    "type": "string",
                    "format": "date-time"
                },
                "end": {
                    "type": "string",
                    "format": "date-time"
                },
                "event": {
                    "$ref": "#/definitions/Event"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "end",
                "event",
                "id",
                "start"
            ],
            "title": "EventSlot"
        },
        "Event": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "eventUserRole": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "eventUserRole"
            ],
            "title": "Event"
        },
        "Task": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "goalId": {
                    "type": "string",
                    "format": "integer"
                },
                "goalName": {
                    "type": "string"
                },
                "studentTaskAdditionalAttributes": {
                    "$ref": "#/definitions/StudentTaskAdditionalAttributes"
                },
                "assignmentType": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "assignmentType",
                "goalId",
                "goalName",
                "id",
                "studentTaskAdditionalAttributes"
            ],
            "title": "Task"
        },
        "StudentTaskAdditionalAttributes": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "cookiesCount": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "cookiesCount"
            ],
            "title": "StudentTaskAdditionalAttributes"
        },
        "VerifiableStudent": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "user": {
                    "$ref": "#/definitions/User"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "user"
            ],
            "title": "VerifiableStudent"
        },
        "User": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "login": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "login"
            ],
            "title": "User"
        }
    }
}

```

</details>

[[Index](#index)]

### calendarGetMyReviews

<details>
<summary> Query </summary>

```
query calendarGetMyReviews($to: DateTime, $limit: Int) {
  student {
    getMyUpcomingBookings(to: $to, limit: $limit) {
      ...Review
      __typename
    }
    __typename
  }
}

fragment Review on CalendarBooking {
  id
  answerId
  eventSlot {
    id
    start
    end
    __typename
  }
  task {
    id
    title
    assignmentType
    goalId
    goalName
    studentTaskAdditionalAttributes {
      cookiesCount
      __typename
    }
    __typename
  }
  verifierUser {
    ...UserInBooking
    __typename
  }
  verifiableStudent {
    id
    user {
      ...UserInBooking
      __typename
    }
    __typename
  }
  team {
    ...ProjectTeamMembers
    __typename
  }
  bookingStatus
  isOnline
  vcLinkUrl
  __typename
}

fragment UserInBooking on User {
  id
  login
  avatarUrl
  userExperience {
    level {
      id
      range {
        levelCode
        __typename
      }
      __typename
    }
    __typename
  }
  __typename
}

fragment ProjectTeamMembers on ProjectTeamMembers {
  id
  teamLead {
    ...ProjectTeamMember
    __typename
  }
  members {
    ...ProjectTeamMember
    __typename
  }
  invitedUsers {
    ...ProjectTeamMember
    __typename
  }
  teamName
  teamStatus
  minTeamMemberCount
  maxTeamMemberCount
  __typename
}

fragment ProjectTeamMember on User {
  id
  avatarUrl
  login
  userExperience {
    level {
      id
      range {
        levelCode
        __typename
      }
      __typename
    }
    cookiesCount
    codeReviewPoints
    __typename
  }
  __typename
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "limit": {
                    "type": "integer"
                }
            },
            "required": [
                "limit"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getMyUpcomingBookings": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/GetMyUpcomingBooking"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getMyUpcomingBookings"
            ],
            "title": "Student"
        },
        "GetMyUpcomingBooking": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "answerId": {
                    "anyOf": [
                        {
                            "type": "string",
                            "format": "integer"
                        },
                        {
                            "type": "null"
                        }
                    ]
                },
                "eventSlot": {
                    "$ref": "#/definitions/EventSlot"
                },
                "task": {
                    "anyOf": [
                        {
                            "$ref": "#/definitions/Task"
                        },
                        {
                            "type": "null"
                        }
                    ]
                },
                "verifierUser": {
                    "$ref": "#/definitions/User"
                },
                "verifiableStudent": {
                    "anyOf": [
                        {
                            "$ref": "#/definitions/VerifiableStudent"
                        },
                        {
                            "type": "null"
                        }
                    ]
                },
                "team": {
                    "anyOf": [
                        {
                            "$ref": "#/definitions/Team"
                        },
                        {
                            "type": "null"
                        }
                    ]
                },
                "bookingStatus": {
                    "type": "string"
                },
                "isOnline": {
                    "type": "boolean"
                },
                "vcLinkUrl": {
                    "type": "null"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "answerId",
                "bookingStatus",
                "eventSlot",
                "id",
                "isOnline",
                "task",
                "team",
                "vcLinkUrl",
                "verifiableStudent",
                "verifierUser"
            ],
            "title": "GetMyUpcomingBooking"
        },
        "EventSlot": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "start": {
                    "type": "string",
                    "format": "date-time"
                },
                "end": {
                    "type": "string",
                    "format": "date-time"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "end",
                "id",
                "start"
            ],
            "title": "EventSlot"
        },
        "Task": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "title": {
                    "type": "string"
                },
                "assignmentType": {
                    "type": "string"
                },
                "goalId": {
                    "type": "string",
                    "format": "integer"
                },
                "goalName": {
                    "type": "string"
                },
                "studentTaskAdditionalAttributes": {
                    "$ref": "#/definitions/StudentTaskAdditionalAttributes"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "assignmentType",
                "goalId",
                "goalName",
                "id",
                "studentTaskAdditionalAttributes",
                "title"
            ],
            "title": "Task"
        },
        "StudentTaskAdditionalAttributes": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "cookiesCount": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "cookiesCount"
            ],
            "title": "StudentTaskAdditionalAttributes"
        },
        "Team": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "teamLead": {
                    "$ref": "#/definitions/TeamLead"
                },
                "members": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/TeamLead"
                    }
                },
                "invitedUsers": {
                    "type": "array",
                    "items": {}
                },
                "teamName": {
                    "type": "string"
                },
                "teamStatus": {
                    "type": "string"
                },
                "minTeamMemberCount": {
                    "type": "integer"
                },
                "maxTeamMemberCount": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "invitedUsers",
                "maxTeamMemberCount",
                "members",
                "minTeamMemberCount",
                "teamLead",
                "teamName",
                "teamStatus"
            ],
            "title": "Team"
        },
        "TeamLead": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "avatarUrl": {
                    "type": "string"
                },
                "login": {
                    "type": "string"
                },
                "userExperience": {
                    "$ref": "#/definitions/TeamLeadUserExperience"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "avatarUrl",
                "id",
                "login",
                "userExperience"
            ],
            "title": "TeamLead"
        },
        "TeamLeadUserExperience": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "level": {
                    "$ref": "#/definitions/Level"
                },
                "cookiesCount": {
                    "type": "integer"
                },
                "codeReviewPoints": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "codeReviewPoints",
                "cookiesCount",
                "level"
            ],
            "title": "TeamLeadUserExperience"
        },
        "Level": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "integer"
                },
                "range": {
                    "$ref": "#/definitions/Range"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "range"
            ],
            "title": "Level"
        },
        "Range": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "levelCode": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "levelCode"
            ],
            "title": "Range"
        },
        "VerifiableStudent": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "user": {
                    "$ref": "#/definitions/User"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "user"
            ],
            "title": "VerifiableStudent"
        },
        "User": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "login": {
                    "type": "string"
                },
                "avatarUrl": {
                    "type": "string"
                },
                "userExperience": {
                    "$ref": "#/definitions/VerifierUserUserExperience"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "avatarUrl",
                "id",
                "login",
                "userExperience"
            ],
            "title": "User"
        },
        "VerifierUserUserExperience": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "level": {
                    "$ref": "#/definitions/Level"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "level"
            ],
            "title": "VerifierUserUserExperience"
        }
    }
}

```

</details>

[[Index](#index)]

### calendarDeleteEventSlot

<details>
<summary> Query </summary>

```
mutation calendarDeleteEventSlot($eventSlotId: ID!) {
  student {
    deleteEventSlot(eventSlotId: $eventSlotId)
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "eventSlotId": {
                    "type": "string",
                    "format": "integer"
                }
            },
            "required": [
                "eventSlotId"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "deleteEventSlot": {
                    "type": "boolean"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "deleteEventSlot"
            ],
            "title": "Student"
        }
    }
}

```

</details>

[[Index](#index)]

### getAgendaP2P

<details>
<summary> Query </summary>

```
query getAgendaP2P($bookingId: ID!) {
  student {
    getEnrichedBooking(bookingId: $bookingId) {
      id
      eventSlot {
        start
        __typename
      }
      task {
        goalId
        goalName
        assignmentType
        studentTaskAdditionalAttributes {
          cookiesCount
          __typename
        }
        __typename
      }
      verifierUser {
        id
        login
        avatarUrl
        userExperience {
          level {
            range {
              levelCode
              __typename
            }
            __typename
          }
          __typename
        }
        __typename
      }
      verifiableStudent {
        user {
          id
          login
          avatarUrl
          userExperience {
            level {
              range {
                levelCode
                __typename
              }
              __typename
            }
            __typename
          }
          __typename
        }
        __typename
      }
      answerId
      team {
        teamName
        teamLead {
          id
          avatarUrl
          login
          userExperience {
            level {
              range {
                levelCode
                __typename
              }
              __typename
            }
            __typename
          }
          __typename
        }
        members {
          id
          avatarUrl
          login
          userExperience {
            level {
              range {
                levelCode
                __typename
              }
              __typename
            }
            __typename
          }
          __typename
        }
        __typename
      }
      bookingStatus
      isOnline
      vcLinkUrl
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "bookingId": {
                    "type": "string",
                    "format": "integer"
                }
            },
            "required": [
                "bookingId"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getEnrichedBooking": {
                    "$ref": "#/definitions/GetEnrichedBooking"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getEnrichedBooking"
            ],
            "title": "Student"
        },
        "GetEnrichedBooking": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "eventSlot": {
                    "$ref": "#/definitions/EventSlot"
                },
                "task": {
                    "anyOf": [
                        {
                            "$ref": "#/definitions/Task"
                        },
                        {
                            "type": "null"
                        }
                    ]
                },
                "verifierUser": {
                    "$ref": "#/definitions/VerifierUser"
                },
                "verifiableStudent": {
                    "anyOf": [
                        {
                            "$ref": "#/definitions/VerifiableStudent"
                        },
                        {
                            "type": "null"
                        }
                    ]
                },
                "answerId": {
                    "anyOf": [
                        {
                            "type": "string",
                            "format": "integer"
                        },
                        {
                            "type": "null"
                        }
                    ]
                },
                "team": {
                    "anyOf": [
                        {
                            "$ref": "#/definitions/Team"
                        },
                        {
                            "type": "null"
                        }
                    ]
                },
                "bookingStatus": {
                    "type": "string"
                },
                "isOnline": {
                    "type": "boolean"
                },
                "vcLinkUrl": {
                    "type": "null"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "answerId",
                "bookingStatus",
                "eventSlot",
                "id",
                "isOnline",
                "task",
                "team",
                "vcLinkUrl",
                "verifiableStudent",
                "verifierUser"
            ],
            "title": "GetEnrichedBooking"
        },
        "EventSlot": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "start": {
                    "type": "string",
                    "format": "date-time"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "start"
            ],
            "title": "EventSlot"
        },
        "Task": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "goalId": {
                    "type": "string",
                    "format": "integer"
                },
                "goalName": {
                    "type": "string"
                },
                "assignmentType": {
                    "type": "string"
                },
                "studentTaskAdditionalAttributes": {
                    "$ref": "#/definitions/StudentTaskAdditionalAttributes"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "assignmentType",
                "goalId",
                "goalName",
                "studentTaskAdditionalAttributes"
            ],
            "title": "Task"
        },
        "StudentTaskAdditionalAttributes": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "cookiesCount": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "cookiesCount"
            ],
            "title": "StudentTaskAdditionalAttributes"
        },
        "Team": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "teamName": {
                    "type": "string"
                },
                "teamLead": {
                    "$ref": "#/definitions/VerifierUser"
                },
                "members": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/VerifierUser"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "members",
                "teamLead",
                "teamName"
            ],
            "title": "Team"
        },
        "VerifierUser": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "login": {
                    "type": "string"
                },
                "avatarUrl": {
                    "type": "string"
                },
                "userExperience": {
                    "$ref": "#/definitions/UserExperience"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "avatarUrl",
                "id",
                "login",
                "userExperience"
            ],
            "title": "VerifierUser"
        },
        "UserExperience": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "level": {
                    "$ref": "#/definitions/Level"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "level"
            ],
            "title": "UserExperience"
        },
        "Level": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "range": {
                    "$ref": "#/definitions/Range"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "range"
            ],
            "title": "Level"
        },
        "Range": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "levelCode": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "levelCode"
            ],
            "title": "Range"
        },
        "VerifiableStudent": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "user": {
                    "$ref": "#/definitions/VerifierUser"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "user"
            ],
            "title": "VerifiableStudent"
        }
    }
}

```

</details>

[[Index](#index)]

### createFilledChecklist

<details>
<summary> Query </summary>

```
mutation createFilledChecklist($studentAnswerId: ID!) {
  student {
    createFilledChecklist(studentAnswerId: $studentAnswerId) {
      id
      gitlabStudentProjectUrl {
        sshLink
        httpsLink
        __typename
      }
      checklist {
        ...FormChecklist
        __typename
      }
      moduleInfoP2P {
        ...FilledChecklistModuleInfo
        __typename
      }
      progressCheckInfo {
        reviewUserCount
        reviewUserCountExecuted
        __typename
      }
      verifiableUsers {
        teamWithMembers {
          team {
            id
            name
            __typename
          }
          members {
            ...TeamMember
            __typename
          }
          __typename
        }
        user {
          ...TeamMemberUser
          __typename
        }
        __typename
      }
      video {
        filledChecklistId
        link
        status
        statusDetails
        __typename
      }
      __typename
    }
    __typename
  }
}

fragment FormChecklist on Checklist {
  language
  introduction
  guidelines
  sectionList {
    ...FormChecklistSection
    __typename
  }
  quickActions
  __typename
}

fragment FormChecklistSection on ChecklistSection {
  checklistSectionId
  name
  description
  kindQuestionId
  questionList {
    ...FormChecklistQuestion
    __typename
  }
  __typename
}

fragment FormChecklistQuestion on SectionQuestion {
  sectionQuestionId
  name
  description
  taskAssessmentScale {
    criterionScaleId
    type
    description
    scaleWeights {
      key
      value
      __typename
    }
    __typename
  }
  __typename
}

fragment FilledChecklistModuleInfo on ModuleInfoP2P {
  moduleName
  executionType
  periodOfVerification
  __typename
}

fragment TeamMember on TeamMember {
  user {
    ...TeamMemberUser
    __typename
  }
  role
  __typename
}

fragment TeamMemberUser on User {
  id
  avatarUrl
  login
  userExperience {
    level {
      id
      levelCode
      range {
        levelCode
        __typename
      }
      __typename
    }
    cookiesCount
    codeReviewPoints
    __typename
  }
  __typename
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "studentAnswerId": {
                    "type": "string",
                    "format": "integer"
                }
            },
            "required": [
                "studentAnswerId"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "createFilledChecklist": {
                    "$ref": "#/definitions/CreateFilledChecklist"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "createFilledChecklist"
            ],
            "title": "Student"
        },
        "CreateFilledChecklist": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "gitlabStudentProjectUrl": {
                    "$ref": "#/definitions/GitlabStudentProjectURL"
                },
                "checklist": {
                    "$ref": "#/definitions/Checklist"
                },
                "moduleInfoP2P": {
                    "$ref": "#/definitions/ModuleInfoP2P"
                },
                "progressCheckInfo": {
                    "$ref": "#/definitions/ProgressCheckInfo"
                },
                "verifiableUsers": {
                    "$ref": "#/definitions/VerifiableUsers"
                },
                "video": {
                    "type": "null"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "checklist",
                "gitlabStudentProjectUrl",
                "id",
                "moduleInfoP2P",
                "progressCheckInfo",
                "verifiableUsers",
                "video"
            ],
            "title": "CreateFilledChecklist"
        },
        "Checklist": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "language": {
                    "type": "string"
                },
                "introduction": {
                    "type": "string"
                },
                "guidelines": {
                    "type": "string"
                },
                "sectionList": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/SectionList"
                    }
                },
                "quickActions": {
                    "type": "array",
                    "items": {
                        "type": "string"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "guidelines",
                "introduction",
                "language",
                "quickActions",
                "sectionList"
            ],
            "title": "Checklist"
        },
        "SectionList": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "checklistSectionId": {
                    "type": "string",
                    "format": "integer"
                },
                "name": {
                    "type": "string"
                },
                "description": {
                    "type": "string"
                },
                "kindQuestionId": {
                    "type": "string",
                    "format": "integer"
                },
                "questionList": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/QuestionList"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "checklistSectionId",
                "description",
                "kindQuestionId",
                "name",
                "questionList"
            ],
            "title": "SectionList"
        },
        "QuestionList": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "sectionQuestionId": {
                    "type": "string",
                    "format": "integer"
                },
                "name": {
                    "type": "string"
                },
                "description": {
                    "type": "string"
                },
                "taskAssessmentScale": {
                    "$ref": "#/definitions/TaskAssessmentScale"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "description",
                "name",
                "sectionQuestionId",
                "taskAssessmentScale"
            ],
            "title": "QuestionList"
        },
        "TaskAssessmentScale": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "criterionScaleId": {
                    "type": "string",
                    "format": "integer"
                },
                "type": {
                    "type": "string"
                },
                "description": {
                    "type": "string"
                },
                "scaleWeights": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/ScaleWeight"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "criterionScaleId",
                "description",
                "scaleWeights",
                "type"
            ],
            "title": "TaskAssessmentScale"
        },
        "ScaleWeight": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "key": {
                    "type": "string",
                    "format": "integer"
                },
                "value": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "key",
                "value"
            ],
            "title": "ScaleWeight"
        },
        "GitlabStudentProjectURL": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "sshLink": {
                    "type": "string"
                },
                "httpsLink": {
                    "type": "string",
                    "format": "uri",
                    "qt-uri-protocols": [
                        "https"
                    ],
                    "qt-uri-extensions": [
                        ".git"
                    ]
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "httpsLink",
                "sshLink"
            ],
            "title": "GitlabStudentProjectURL"
        },
        "ModuleInfoP2P": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "moduleName": {
                    "type": "string"
                },
                "executionType": {
                    "type": "string"
                },
                "periodOfVerification": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "executionType",
                "moduleName",
                "periodOfVerification"
            ],
            "title": "ModuleInfoP2P"
        },
        "ProgressCheckInfo": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "reviewUserCount": {
                    "type": "integer"
                },
                "reviewUserCountExecuted": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "reviewUserCount",
                "reviewUserCountExecuted"
            ],
            "title": "ProgressCheckInfo"
        },
        "VerifiableUsers": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "teamWithMembers": {
                    "anyOf": [
                        {
                            "$ref": "#/definitions/TeamWithMembers"
                        },
                        {
                            "type": "null"
                        }
                    ]
                },
                "user": {
                    "anyOf": [
                        {
                            "$ref": "#/definitions/User"
                        },
                        {
                            "type": "null"
                        }
                    ]
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "teamWithMembers",
                "user"
            ],
            "title": "VerifiableUsers"
        },
        "TeamWithMembers": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "team": {
                    "$ref": "#/definitions/Team"
                },
                "members": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/Member"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "members",
                "team"
            ],
            "title": "TeamWithMembers"
        },
        "Member": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "user": {
                    "$ref": "#/definitions/User"
                },
                "role": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "role",
                "user"
            ],
            "title": "Member"
        },
        "UserExperience": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "level": {
                    "$ref": "#/definitions/Level"
                },
                "cookiesCount": {
                    "type": "integer"
                },
                "codeReviewPoints": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "codeReviewPoints",
                "cookiesCount",
                "level"
            ],
            "title": "UserExperience"
        },
        "Level": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "integer"
                },
                "levelCode": {
                    "type": "integer"
                },
                "range": {
                    "$ref": "#/definitions/Range"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "levelCode",
                "range"
            ],
            "title": "Level"
        },
        "Range": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "levelCode": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "levelCode"
            ],
            "title": "Range"
        },
        "Team": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "name": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "name"
            ],
            "title": "Team"
        },
        "User": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "avatarUrl": {
                    "type": "string"
                },
                "login": {
                    "type": "string"
                },
                "userExperience": {
                    "$ref": "#/definitions/UserExperience"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "avatarUrl",
                "id",
                "login",
                "userExperience"
            ],
            "title": "User"
        }
    }
}

```

</details>

[[Index](#index)]

### getCredentialsByLogin

<details>
<summary> Query </summary>

```
query getCredentialsByLogin($login: String!) {
  school21 {
    getStudentByLogin(login: $login) {
      studentId
      userId
      schoolId
      isActive
      isGraduate
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "login": {
                    "type": "string"
                }
            },
            "required": [
                "login"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "school21": {
                    "$ref": "#/definitions/School21"
                }
            },
            "required": [
                "school21"
            ],
            "title": "Data"
        },
        "School21": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getStudentByLogin": {
                    "$ref": "#/definitions/GetStudentByLogin"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getStudentByLogin"
            ],
            "title": "School21"
        },
        "GetStudentByLogin": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "studentId": {
                    "type": "string",
                    "format": "uuid"
                },
                "userId": {
                    "type": "string",
                    "format": "uuid"
                },
                "schoolId": {
                    "type": "string",
                    "format": "uuid"
                },
                "isActive": {
                    "type": "boolean"
                },
                "isGraduate": {
                    "type": "boolean"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "isActive",
                "isGraduate",
                "schoolId",
                "studentId",
                "userId"
            ],
            "title": "GetStudentByLogin"
        }
    }
}

```

</details>

[[Index](#index)]

### publicProfileGetPersonalInfo

<details>
<summary> Query </summary>

```
query publicProfileGetPersonalInfo($userId: UUID!, $studentId: UUID!, $login: String!, $schoolId: UUID!) {
  student {
    getAvatarByUserId(userId: $userId)
    getStageGroupS21PublicProfile(studentId: $studentId) {
      waveId
      waveName
      eduForm
      __typename
    }
    getExperiencePublicProfile(userId: $userId) {
      value
      level {
        levelCode
        range {
          leftBorder
          rightBorder
          __typename
        }
        __typename
      }
      cookiesCount
      coinsCount
      codeReviewPoints
      __typename
    }
    getEmailbyUserId(userId: $userId)
    getWorkstationByLogin(login: $login) {
      workstationId
      hostName
      row
      number
      __typename
    }
    getClassRoomByLogin(login: $login) {
      id
      number
      floor
      __typename
    }
    getFeedbackStatisticsAverageScore(studentId: $studentId) {
      countFeedback
      feedbackAverageScore {
        categoryCode
        categoryName
        value
        __typename
      }
      __typename
    }
    __typename
  }
  user {
    getSchool(schoolId: $schoolId) {
      id
      fullName
      shortName
      address
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "userId": {
                    "type": "string",
                    "format": "uuid"
                },
                "studentId": {
                    "type": "string",
                    "format": "uuid"
                },
                "schoolId": {
                    "type": "string",
                    "format": "uuid"
                },
                "login": {
                    "type": "string"
                }
            },
            "required": [
                "login",
                "schoolId",
                "studentId",
                "userId"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                },
                "user": {
                    "$ref": "#/definitions/User"
                }
            },
            "required": [
                "student",
                "user"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getAvatarByUserId": {
                    "type": "string"
                },
                "getStageGroupS21PublicProfile": {
                    "$ref": "#/definitions/GetStageGroupS21PublicProfile"
                },
                "getExperiencePublicProfile": {
                    "$ref": "#/definitions/GetExperiencePublicProfile"
                },
                "getEmailbyUserId": {
                    "type": "string"
                },
                "getWorkstationByLogin": {
                    "anyOf": [
                        {
                            "$ref": "#/definitions/GetWorkstationByLogin"
                        },
                        {
                            "type": "null"
                        }
                    ]
                },
                "getClassRoomByLogin": {
                    "anyOf": [
                        {
                            "$ref": "#/definitions/GetClassRoomByLogin"
                        },
                        {
                            "type": "null"
                        }
                    ]
                },
                "getFeedbackStatisticsAverageScore": {
                    "$ref": "#/definitions/GetFeedbackStatisticsAverageScore"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getAvatarByUserId",
                "getClassRoomByLogin",
                "getEmailbyUserId",
                "getExperiencePublicProfile",
                "getFeedbackStatisticsAverageScore",
                "getStageGroupS21PublicProfile",
                "getWorkstationByLogin"
            ],
            "title": "Student"
        },
        "GetClassRoomByLogin": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "number": {
                    "type": "string"
                },
                "floor": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "floor",
                "id",
                "number"
            ],
            "title": "GetClassRoomByLogin"
        },
        "GetExperiencePublicProfile": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "value": {
                    "type": "integer"
                },
                "level": {
                    "$ref": "#/definitions/Level"
                },
                "cookiesCount": {
                    "type": "integer"
                },
                "coinsCount": {
                    "type": "integer"
                },
                "codeReviewPoints": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "codeReviewPoints",
                "coinsCount",
                "cookiesCount",
                "level",
                "value"
            ],
            "title": "GetExperiencePublicProfile"
        },
        "Level": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "levelCode": {
                    "type": "integer"
                },
                "range": {
                    "$ref": "#/definitions/Range"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "levelCode",
                "range"
            ],
            "title": "Level"
        },
        "Range": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "leftBorder": {
                    "type": "integer"
                },
                "rightBorder": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "leftBorder",
                "rightBorder"
            ],
            "title": "Range"
        },
        "GetFeedbackStatisticsAverageScore": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "countFeedback": {
                    "type": "integer"
                },
                "feedbackAverageScore": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/FeedbackAverageScore"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "countFeedback",
                "feedbackAverageScore"
            ],
            "title": "GetFeedbackStatisticsAverageScore"
        },
        "FeedbackAverageScore": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "categoryCode": {
                    "type": "string"
                },
                "categoryName": {
                    "type": "string"
                },
                "value": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "categoryCode",
                "categoryName",
                "value"
            ],
            "title": "FeedbackAverageScore"
        },
        "GetStageGroupS21PublicProfile": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "waveId": {
                    "type": "integer"
                },
                "waveName": {
                    "type": "string"
                },
                "eduForm": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "eduForm",
                "waveId",
                "waveName"
            ],
            "title": "GetStageGroupS21PublicProfile"
        },
        "GetWorkstationByLogin": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "workstationId": {
                    "type": "integer"
                },
                "hostName": {
                    "type": "string"
                },
                "row": {
                    "type": "string"
                },
                "number": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "hostName",
                "number",
                "row",
                "workstationId"
            ],
            "title": "GetWorkstationByLogin"
        },
        "User": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getSchool": {
                    "$ref": "#/definitions/GetSchool"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getSchool"
            ],
            "title": "User"
        },
        "GetSchool": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "fullName": {
                    "type": "string"
                },
                "shortName": {
                    "type": "string"
                },
                "address": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "address",
                "fullName",
                "id",
                "shortName"
            ],
            "title": "GetSchool"
        }
    }
}

```

</details>

[[Index](#index)]

### getDismissInfoByStudentId

<details>
<summary> Query </summary>

```
query getDismissInfoByStudentId($studentId: UUID!) {
  school21 {
    getDismissInfoByStudentId(studentId: $studentId) {
      dismissTypeId
      dismissTs
      lastStageGroupS21 {
        waveId
        waveName
        eduForm
        active
        __typename
      }
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "studentId": {
                    "type": "string",
                    "format": "uuid"
                }
            },
            "required": [
                "studentId"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "school21": {
                    "$ref": "#/definitions/School21"
                }
            },
            "required": [
                "school21"
            ],
            "title": "Data"
        },
        "School21": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getDismissInfoByStudentId": {
                    "type": "null"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getDismissInfoByStudentId"
            ],
            "title": "School21"
        }
    }
}

```

</details>

[[Index](#index)]

### publicProfileGetCoalition

<details>
<summary> Query </summary>

```
query publicProfileGetCoalition($userId: UUID!) {
  student {
    getUserTournamentWidget(userId: $userId) {
      coalitionMember {
        coalition {
          avatarUrl
          color
          name
          memberCount
          __typename
        }
        currentTournamentPowerRank {
          rank
          power {
            id
            points
            __typename
          }
          __typename
        }
        __typename
      }
      lastTournamentResult {
        userRank
        power
        __typename
      }
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "userId": {
                    "type": "string",
                    "format": "uuid"
                }
            },
            "required": [
                "userId"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getUserTournamentWidget": {
                    "$ref": "#/definitions/GetUserTournamentWidget"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getUserTournamentWidget"
            ],
            "title": "Student"
        },
        "GetUserTournamentWidget": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "coalitionMember": {
                    "$ref": "#/definitions/CoalitionMember"
                },
                "lastTournamentResult": {
                    "$ref": "#/definitions/LastTournamentResult"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "coalitionMember",
                "lastTournamentResult"
            ],
            "title": "GetUserTournamentWidget"
        },
        "CoalitionMember": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "coalition": {
                    "$ref": "#/definitions/Coalition"
                },
                "currentTournamentPowerRank": {
                    "$ref": "#/definitions/CurrentTournamentPowerRank"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "coalition",
                "currentTournamentPowerRank"
            ],
            "title": "CoalitionMember"
        },
        "Coalition": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "avatarUrl": {
                    "type": "string"
                },
                "color": {
                    "type": "string"
                },
                "name": {
                    "type": "string"
                },
                "memberCount": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "avatarUrl",
                "color",
                "memberCount",
                "name"
            ],
            "title": "Coalition"
        },
        "CurrentTournamentPowerRank": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "rank": {
                    "type": "integer"
                },
                "power": {
                    "$ref": "#/definitions/Power"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "power",
                "rank"
            ],
            "title": "CurrentTournamentPowerRank"
        },
        "Power": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "points": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "points"
            ],
            "title": "Power"
        },
        "LastTournamentResult": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "userRank": {
                    "type": "integer"
                },
                "power": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "power",
                "userRank"
            ],
            "title": "LastTournamentResult"
        }
    }
}

```

</details>

[[Index](#index)]

### publicProfileGetAchievements

<details>
<summary> Query </summary>

```
query publicProfileGetAchievements($userId: UUID!) {
  student {
    getBadgesPublicProfile(userId: $userId) {
      points
      id
      badge {
        id
        name
        avatarUrl
        __typename
      }
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "userId": {
                    "type": "string",
                    "format": "uuid"
                }
            },
            "required": [
                "userId"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getBadgesPublicProfile": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/GetBadgesPublicProfile"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getBadgesPublicProfile"
            ],
            "title": "Student"
        },
        "GetBadgesPublicProfile": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "points": {
                    "type": "integer"
                },
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "badge": {
                    "$ref": "#/definitions/Badge"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "badge",
                "id",
                "points"
            ],
            "title": "GetBadgesPublicProfile"
        },
        "Badge": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "name": {
                    "type": "string"
                },
                "avatarUrl": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "avatarUrl",
                "id",
                "name"
            ],
            "title": "Badge"
        }
    }
}

```

</details>

[[Index](#index)]

### publicProfileLoadAverageLogtime

<details>
<summary> Query </summary>

```
query publicProfileLoadAverageLogtime($login: String!, $schoolID: UUID!, $date: Date!) {
  school21 {
    loadAverageLogtime(login: $login, schoolID: $schoolID, date: $date) {
      week
      month
      weekPerMonth
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "login": {
                    "type": "string"
                },
                "schoolID": {
                    "type": "string",
                    "format": "uuid"
                },
                "date": {
                    "type": "string",
                    "format": "date"
                }
            },
            "required": [
                "date",
                "login",
                "schoolID"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "school21": {
                    "$ref": "#/definitions/School21"
                }
            },
            "required": [
                "school21"
            ],
            "title": "Data"
        },
        "School21": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "loadAverageLogtime": {
                    "$ref": "#/definitions/LoadAverageLogtime"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "loadAverageLogtime"
            ],
            "title": "School21"
        },
        "LoadAverageLogtime": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "week": {
                    "type": "integer"
                },
                "month": {
                    "type": "integer"
                },
                "weekPerMonth": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "month",
                "week",
                "weekPerMonth"
            ],
            "title": "LoadAverageLogtime"
        }
    }
}

```

</details>

[[Index](#index)]

### publicProfileLoadStageGroups

<details>
<summary> Query </summary>

```
query publicProfileLoadStageGroups($userId: UUID!, $schoolId: UUID!) {
  school21 {
    loadStudentStageGroupsS21PublicProfile(userId: $userId, schoolId: $schoolId) {
      stageGroupStudentId
      studentId
      stageGroupS21 {
        waveId
        waveName
        eduForm
        active
        __typename
      }
      safeSchool {
        fullName
        __typename
      }
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "userId": {
                    "type": "string",
                    "format": "uuid"
                },
                "schoolId": {
                    "type": "string",
                    "format": "uuid"
                }
            },
            "required": [
                "schoolId",
                "userId"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "school21": {
                    "$ref": "#/definitions/School21"
                }
            },
            "required": [
                "school21"
            ],
            "title": "Data"
        },
        "School21": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "loadStudentStageGroupsS21PublicProfile": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/LoadStudentStageGroupsS21PublicProfile"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "loadStudentStageGroupsS21PublicProfile"
            ],
            "title": "School21"
        },
        "LoadStudentStageGroupsS21PublicProfile": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "stageGroupStudentId": {
                    "type": "string",
                    "format": "integer"
                },
                "studentId": {
                    "type": "string",
                    "format": "uuid"
                },
                "stageGroupS21": {
                    "$ref": "#/definitions/StageGroupS21"
                },
                "safeSchool": {
                    "$ref": "#/definitions/SafeSchool"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "safeSchool",
                "stageGroupS21",
                "stageGroupStudentId",
                "studentId"
            ],
            "title": "LoadStudentStageGroupsS21PublicProfile"
        },
        "SafeSchool": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "fullName": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "fullName"
            ],
            "title": "SafeSchool"
        },
        "StageGroupS21": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "waveId": {
                    "type": "integer"
                },
                "waveName": {
                    "type": "string"
                },
                "eduForm": {
                    "type": "string"
                },
                "active": {
                    "type": "boolean"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "active",
                "eduForm",
                "waveId",
                "waveName"
            ],
            "title": "StageGroupS21"
        }
    }
}

```

</details>

[[Index](#index)]

### publicProfileGetSoftSkills

<details>
<summary> Query </summary>

```
query publicProfileGetSoftSkills($studentId: UUID!) {
  school21 {
    getSoftSkillsByStudentId(studentId: $studentId) {
      id
      type
      code
      totalPower
      hueSaturationLightness
      __typename
    }
    getSoftSkillLimitByStudentId(studentId: $studentId) {
      powerLimit
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "studentId": {
                    "type": "string",
                    "format": "uuid"
                }
            },
            "required": [
                "studentId"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "school21": {
                    "$ref": "#/definitions/School21"
                }
            },
            "required": [
                "school21"
            ],
            "title": "Data"
        },
        "School21": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getSoftSkillsByStudentId": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/GetSoftSkillsByStudentID"
                    }
                },
                "getSoftSkillLimitByStudentId": {
                    "$ref": "#/definitions/GetSoftSkillLimitByStudentID"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getSoftSkillLimitByStudentId",
                "getSoftSkillsByStudentId"
            ],
            "title": "School21"
        },
        "GetSoftSkillLimitByStudentID": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "powerLimit": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "powerLimit"
            ],
            "title": "GetSoftSkillLimitByStudentID"
        },
        "GetSoftSkillsByStudentID": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string"
                },
                "type": {
                    "type": "string"
                },
                "code": {
                    "type": "string"
                },
                "totalPower": {
                    "type": "integer"
                },
                "hueSaturationLightness": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "code",
                "hueSaturationLightness",
                "id",
                "totalPower",
                "type"
            ],
            "title": "GetSoftSkillsByStudentID"
        }
    }
}

```

</details>

[[Index](#index)]

### publicProfileGetXpGraph

<details>
<summary> Query </summary>

```
query publicProfileGetXpGraph($userId: UUID!) {
  student {
    getExperienceHistoryDate(userId: $userId) {
      history {
        awardDate
        expValue
        __typename
      }
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "userId": {
                    "type": "string",
                    "format": "uuid"
                }
            },
            "required": [
                "userId"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getExperienceHistoryDate": {
                    "$ref": "#/definitions/GetExperienceHistoryDate"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getExperienceHistoryDate"
            ],
            "title": "Student"
        },
        "GetExperienceHistoryDate": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "history": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/History"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "history"
            ],
            "title": "GetExperienceHistoryDate"
        },
        "History": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "awardDate": {
                    "type": "string",
                    "format": "date"
                },
                "expValue": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "awardDate",
                "expValue"
            ],
            "title": "History"
        }
    }
}

```

</details>

[[Index](#index)]

### publicProfileGetStudentTraffic

<details>
<summary> Query </summary>

```
query publicProfileGetStudentTraffic($login: String!, $schoolID: UUID!, $date: Date!) {
  student {
    getStudentTraffic(login: $login, schoolID: $schoolID, date: $date) {
      days {
        date
        periodOnCampus
        periodAuthorizSDP
        periodAuthorizIMac
        __typename
      }
      endDate
      startDate
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "login": {
                    "type": "string"
                },
                "schoolID": {
                    "type": "string",
                    "format": "uuid"
                },
                "date": {
                    "type": "string",
                    "format": "date"
                }
            },
            "required": [
                "date",
                "login",
                "schoolID"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getStudentTraffic": {
                    "$ref": "#/definitions/GetStudentTraffic"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getStudentTraffic"
            ],
            "title": "Student"
        },
        "GetStudentTraffic": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "days": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/Day"
                    }
                },
                "endDate": {
                    "type": "string",
                    "format": "date"
                },
                "startDate": {
                    "type": "string",
                    "format": "date"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "days",
                "endDate",
                "startDate"
            ],
            "title": "GetStudentTraffic"
        },
        "Day": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "date": {
                    "type": "string",
                    "format": "date"
                },
                "periodOnCampus": {
                    "type": "string",
                    "format": "integer"
                },
                "periodAuthorizSDP": {
                    "type": "string",
                    "format": "integer"
                },
                "periodAuthorizIMac": {
                    "type": "string",
                    "format": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "date",
                "periodAuthorizIMac",
                "periodAuthorizSDP",
                "periodOnCampus"
            ],
            "title": "Day"
        }
    }
}

```

</details>

[[Index](#index)]

### getUserNotifications

<details>
<summary> Query </summary>

```
query getUserNotifications($paging: PagingInput!) {
  student {
    getS21Notifications(paging: $paging) {
      notifications {
        id
        relatedObjectType
        relatedObjectId
        message
        time
        wasRead
        groupName
        __typename
      }
      totalCount
      groupNames
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "paging": {
                    "$ref": "#/definitions/Paging"
                }
            },
            "required": [
                "paging"
            ],
            "title": "Variables"
        },
        "Paging": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "offset": {
                    "type": "integer"
                },
                "limit": {
                    "type": "integer"
                }
            },
            "required": [
                "limit",
                "offset"
            ],
            "title": "Paging"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getS21Notifications": {
                    "$ref": "#/definitions/GetS21Notifications"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getS21Notifications"
            ],
            "title": "Student"
        },
        "GetS21Notifications": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "notifications": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/Notification"
                    }
                },
                "totalCount": {
                    "type": "integer"
                },
                "groupNames": {
                    "type": "array",
                    "items": {
                        "type": "string"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "groupNames",
                "notifications",
                "totalCount"
            ],
            "title": "GetS21Notifications"
        },
        "Notification": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string"
                },
                "relatedObjectType": {
                    "type": "string"
                },
                "relatedObjectId": {
                    "$ref": "#/definitions/RelatedObjectID"
                },
                "message": {
                    "type": "string"
                },
                "time": {
                    "type": "string",
                    "format": "date-time"
                },
                "wasRead": {
                    "type": "boolean"
                },
                "groupName": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "groupName",
                "id",
                "message",
                "relatedObjectId",
                "relatedObjectType",
                "time",
                "wasRead"
            ],
            "title": "Notification"
        },
        "RelatedObjectID": {
            "anyOf": [
                {
                    "type": "string",
                    "format": "integer"
                },
                {
                    "type": "string",
                    "format": "uuid"
                }
            ],
            "title": "RelatedObjectID"
        }
    }
}

```

</details>

[[Index](#index)]

### readUserNotifications

<details>
<summary> Query </summary>

```
mutation readUserNotifications($notificationIds: [ID!]!) {
  student {
    readNotifications(notificationIds: $notificationIds)
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "notificationIds": {
                    "type": "array",
                    "items": {
                        "type": "string"
                    }
                }
            },
            "required": [
                "notificationIds"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "readNotifications": {
                    "type": "array",
                    "items": {
                        "type": "string"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "readNotifications"
            ],
            "title": "Student"
        }
    }
}

```

</details>

[[Index](#index)]

### saveFilledChecklist

<details>
<summary> Query </summary>

```
mutation saveFilledChecklist($filledChecklistInput: ChecklistFilledInput!) {
  student {
    completeP2pCheck(checklistFilledInput: $filledChecklistInput)
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "filledChecklistInput": {
                    "$ref": "#/definitions/FilledChecklistInput"
                }
            },
            "required": [
                "filledChecklistInput"
            ],
            "title": "Variables"
        },
        "FilledChecklistInput": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "quickAction": {
                    "type": "null"
                },
                "comment": {
                    "type": "string"
                },
                "scoreQuestions": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/ScoreQuestion"
                    }
                },
                "filledChecklistId": {
                    "type": "string",
                    "format": "integer"
                }
            },
            "required": [
                "comment",
                "filledChecklistId",
                "quickAction",
                "scoreQuestions"
            ],
            "title": "FilledChecklistInput"
        },
        "ScoreQuestion": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "sectionQuestionId": {
                    "type": "string",
                    "format": "integer"
                },
                "ratingWeightId": {
                    "type": "string",
                    "format": "integer"
                }
            },
            "required": [
                "ratingWeightId",
                "sectionQuestionId"
            ],
            "title": "ScoreQuestion"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "completeP2pCheck": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "completeP2pCheck"
            ],
            "title": "Student"
        }
    }
}

```

</details>

[[Index](#index)]

### getInvitationsCount

<details>
<summary> Query </summary>

```
query getInvitationsCount {
  team {
    getCreatedJoinTeamRequestCount
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "team": {
                    "$ref": "#/definitions/Team"
                }
            },
            "required": [
                "team"
            ],
            "title": "Data"
        },
        "Team": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getCreatedJoinTeamRequestCount": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getCreatedJoinTeamRequestCount"
            ],
            "title": "Team"
        }
    }
}

```

</details>

[[Index](#index)]

### getStudentCurrentProjects

<details>
<summary> Query </summary>

```
query getStudentCurrentProjects($userId: ID!) {
  student {
    getStudentCurrentProjects(userId: $userId) {
      ...StudentProjectItem
      __typename
    }
    __typename
  }
}

fragment StudentProjectItem on StudentItem {
  goalId
  name
  description
  experience
  dateTime
  finalPercentage
  laboriousness
  executionType
  goalStatus
  courseType
  displayedCourseStatus
  amountAnswers
  amountMembers
  amountJoinedMembers
  amountReviewedAnswers
  amountCodeReviewMembers
  amountCurrentCodeReviewMembers
  groupName
  localCourseId
  __typename
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "userId": {
                    "type": "string",
                    "format": "uuid"
                }
            },
            "required": [
                "userId"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getStudentCurrentProjects": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/GetStudentCurrentProject"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getStudentCurrentProjects"
            ],
            "title": "Student"
        },
        "GetStudentCurrentProject": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "goalId": {
                    "anyOf": [
                        {
                            "type": "integer"
                        },
                        {
                            "type": "null"
                        }
                    ]
                },
                "name": {
                    "type": "string"
                },
                "description": {
                    "type": "string"
                },
                "experience": {
                    "type": "integer"
                },
                "dateTime": {
                    "type": "null"
                },
                "finalPercentage": {
                    "type": "null"
                },
                "laboriousness": {
                    "type": "integer"
                },
                "executionType": {
                    "anyOf": [
                        {
                            "type": "null"
                        },
                        {
                            "type": "string"
                        }
                    ]
                },
                "goalStatus": {
                    "anyOf": [
                        {
                            "type": "null"
                        },
                        {
                            "type": "string"
                        }
                    ]
                },
                "courseType": {
                    "anyOf": [
                        {
                            "type": "null"
                        },
                        {
                            "type": "string"
                        }
                    ]
                },
                "displayedCourseStatus": {
                    "anyOf": [
                        {
                            "type": "null"
                        },
                        {
                            "type": "string"
                        }
                    ]
                },
                "amountAnswers": {
                    "anyOf": [
                        {
                            "type": "integer"
                        },
                        {
                            "type": "null"
                        }
                    ]
                },
                "amountMembers": {
                    "anyOf": [
                        {
                            "type": "integer"
                        },
                        {
                            "type": "null"
                        }
                    ]
                },
                "amountJoinedMembers": {
                    "anyOf": [
                        {
                            "type": "integer"
                        },
                        {
                            "type": "null"
                        }
                    ]
                },
                "amountReviewedAnswers": {
                    "anyOf": [
                        {
                            "type": "integer"
                        },
                        {
                            "type": "null"
                        }
                    ]
                },
                "amountCodeReviewMembers": {
                    "anyOf": [
                        {
                            "type": "integer"
                        },
                        {
                            "type": "null"
                        }
                    ]
                },
                "amountCurrentCodeReviewMembers": {
                    "anyOf": [
                        {
                            "type": "integer"
                        },
                        {
                            "type": "null"
                        }
                    ]
                },
                "groupName": {
                    "type": "string"
                },
                "localCourseId": {
                    "anyOf": [
                        {
                            "type": "integer"
                        },
                        {
                            "type": "null"
                        }
                    ]
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "amountAnswers",
                "amountCodeReviewMembers",
                "amountCurrentCodeReviewMembers",
                "amountJoinedMembers",
                "amountMembers",
                "amountReviewedAnswers",
                "courseType",
                "dateTime",
                "description",
                "displayedCourseStatus",
                "executionType",
                "experience",
                "finalPercentage",
                "goalId",
                "goalStatus",
                "groupName",
                "laboriousness",
                "localCourseId",
                "name"
            ],
            "title": "GetStudentCurrentProject"
        }
    }
}

```

</details>

[[Index](#index)]

### getAvailableCodeReviewProjects

<details>
<summary> Query </summary>

```
query getAvailableCodeReviewProjects($paging: PagingInput!) {
  student {
    getAvailableCodeReviewProjects(paging: $paging) {
      ...CodeReviewProject
      __typename
    }
    __typename
  }
}

fragment CodeReviewProject on CodeReview {
  goalId
  goalTitle
  studentGoalId
  studentCodeReviewStatus
  goalExecutionType
  studentTaskAdditionalAttributesModel {
    codeReviewCost
    codeReviewDuration
    __typename
  }
  __typename
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "paging": {
                    "$ref": "#/definitions/Paging"
                }
            },
            "required": [
                "paging"
            ],
            "title": "Variables"
        },
        "Paging": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "offset": {
                    "type": "integer"
                },
                "limit": {
                    "type": "integer"
                }
            },
            "required": [
                "limit",
                "offset"
            ],
            "title": "Paging"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getAvailableCodeReviewProjects": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/GetAvailableCodeReviewProject"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getAvailableCodeReviewProjects"
            ],
            "title": "Student"
        },
        "GetAvailableCodeReviewProject": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "goalId": {
                    "type": "string",
                    "format": "integer"
                },
                "goalTitle": {
                    "type": "string"
                },
                "studentGoalId": {
                    "type": "string",
                    "format": "integer"
                },
                "studentCodeReviewStatus": {
                    "type": "string"
                },
                "goalExecutionType": {
                    "type": "string"
                },
                "studentTaskAdditionalAttributesModel": {
                    "$ref": "#/definitions/StudentTaskAdditionalAttributesModel"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "goalExecutionType",
                "goalId",
                "goalTitle",
                "studentCodeReviewStatus",
                "studentGoalId",
                "studentTaskAdditionalAttributesModel"
            ],
            "title": "GetAvailableCodeReviewProject"
        },
        "StudentTaskAdditionalAttributesModel": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "codeReviewCost": {
                    "type": "integer"
                },
                "codeReviewDuration": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "codeReviewCost",
                "codeReviewDuration"
            ],
            "title": "StudentTaskAdditionalAttributesModel"
        }
    }
}

```

</details>

[[Index](#index)]

### getFirstRoundCodeReviewProjects

<details>
<summary> Query </summary>

```
query getFirstRoundCodeReviewProjects($paging: PagingInput!) {
  student {
    getFirstRoundCodeReviewProjects(paging: $paging) {
      ...CodeReviewProject
      __typename
    }
    __typename
  }
}

fragment CodeReviewProject on CodeReview {
  goalId
  goalTitle
  studentGoalId
  studentCodeReviewStatus
  goalExecutionType
  studentTaskAdditionalAttributesModel {
    codeReviewCost
    codeReviewDuration
    __typename
  }
  __typename
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "paging": {
                    "$ref": "#/definitions/Paging"
                }
            },
            "required": [
                "paging"
            ],
            "title": "Variables"
        },
        "Paging": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "offset": {
                    "type": "integer"
                },
                "limit": {
                    "type": "integer"
                }
            },
            "required": [
                "limit",
                "offset"
            ],
            "title": "Paging"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getFirstRoundCodeReviewProjects": {
                    "type": "array",
                    "items": {}
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getFirstRoundCodeReviewProjects"
            ],
            "title": "Student"
        }
    }
}

```

</details>

[[Index](#index)]

### getSecondRoundCodeReviewProjects

<details>
<summary> Query </summary>

```
query getSecondRoundCodeReviewProjects($paging: PagingInput!) {
  student {
    getSecondRoundCodeReviewProjects(paging: $paging) {
      ...CodeReviewProject
      __typename
    }
    __typename
  }
}

fragment CodeReviewProject on CodeReview {
  goalId
  goalTitle
  studentGoalId
  studentCodeReviewStatus
  goalExecutionType
  studentTaskAdditionalAttributesModel {
    codeReviewCost
    codeReviewDuration
    __typename
  }
  __typename
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "paging": {
                    "$ref": "#/definitions/Paging"
                }
            },
            "required": [
                "paging"
            ],
            "title": "Variables"
        },
        "Paging": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "offset": {
                    "type": "integer"
                },
                "limit": {
                    "type": "integer"
                }
            },
            "required": [
                "limit",
                "offset"
            ],
            "title": "Paging"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getSecondRoundCodeReviewProjects": {
                    "type": "array",
                    "items": {}
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getSecondRoundCodeReviewProjects"
            ],
            "title": "Student"
        }
    }
}

```

</details>

[[Index](#index)]

### getCodeReviewProjectInfo

<details>
<summary> Query </summary>

```
query getCodeReviewProjectInfo($studentGoalId: ID!) {
  student {
    getStudentModuleByStudentGoalId(studentGoalId: $studentGoalId) {
      ...CodeReviewProjectInfo
      __typename
    }
    __typename
  }
}

fragment CodeReviewProjectInfo on StudentModule {
  id
  moduleTitle
  studyModule {
    duration
    stage {
      name
      __typename
    }
    __typename
  }
  currentTask {
    ...CodeReviewCurrentTaskInfo
    __typename
  }
  __typename
}

fragment CodeReviewCurrentTaskInfo on StudentTask {
  id
  taskId
  task {
    content {
      body
      __typename
    }
    assignmentType
    studentTaskAdditionalAttributes {
      codeReviewDuration
      codeReviewCost
      __typename
    }
    __typename
  }
  __typename
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "studentGoalId": {
                    "type": "string",
                    "format": "integer"
                }
            },
            "required": [
                "studentGoalId"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getStudentModuleByStudentGoalId": {
                    "$ref": "#/definitions/GetStudentModuleByStudentGoalID"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getStudentModuleByStudentGoalId"
            ],
            "title": "Student"
        },
        "GetStudentModuleByStudentGoalID": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "moduleTitle": {
                    "type": "string"
                },
                "studyModule": {
                    "$ref": "#/definitions/StudyModule"
                },
                "currentTask": {
                    "$ref": "#/definitions/CurrentTask"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "currentTask",
                "id",
                "moduleTitle",
                "studyModule"
            ],
            "title": "GetStudentModuleByStudentGoalID"
        },
        "CurrentTask": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "taskId": {
                    "type": "string",
                    "format": "integer"
                },
                "task": {
                    "$ref": "#/definitions/Task"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "task",
                "taskId"
            ],
            "title": "CurrentTask"
        },
        "Task": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "content": {
                    "$ref": "#/definitions/Content"
                },
                "assignmentType": {
                    "type": "string"
                },
                "studentTaskAdditionalAttributes": {
                    "$ref": "#/definitions/StudentTaskAdditionalAttributes"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "assignmentType",
                "content",
                "studentTaskAdditionalAttributes"
            ],
            "title": "Task"
        },
        "Content": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "body": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "body"
            ],
            "title": "Content"
        },
        "StudentTaskAdditionalAttributes": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "codeReviewDuration": {
                    "type": "integer"
                },
                "codeReviewCost": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "codeReviewCost",
                "codeReviewDuration"
            ],
            "title": "StudentTaskAdditionalAttributes"
        },
        "StudyModule": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "duration": {
                    "type": "integer"
                },
                "stage": {
                    "$ref": "#/definitions/Stage"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "duration",
                "stage"
            ],
            "title": "StudyModule"
        },
        "Stage": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "name": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "name"
            ],
            "title": "Stage"
        }
    }
}

```

</details>

[[Index](#index)]

### getCodeReviewMyStudent

<details>
<summary> Query </summary>

```
query getCodeReviewMyStudent($studentGoalId: ID!) {
  student {
    getMyStudentCodeReview(studentGoalId: $studentGoalId) {
      reviewerCommentsCount
      codeReviewRounds {
        ...CodeReviewRound
        __typename
      }
      __typename
    }
    __typename
  }
}

fragment CodeReviewRound on CodeReviewRound {
  eventId
  codeReviewRoundType
  codeReviewStatus
  startTime
  endTime
  mergeRequestURL
  createTime
  __typename
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "studentGoalId": {
                    "type": "string",
                    "format": "integer"
                }
            },
            "required": [
                "studentGoalId"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getMyStudentCodeReview": {
                    "anyOf": [
                        {
                            "$ref": "#/definitions/GetMyStudentCodeReview"
                        },
                        {
                            "type": "null"
                        }
                    ]
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getMyStudentCodeReview"
            ],
            "title": "Student"
        },
        "GetMyStudentCodeReview": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "reviewerCommentsCount": {
                    "type": "integer"
                },
                "codeReviewRounds": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/CodeReviewRound"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "codeReviewRounds",
                "reviewerCommentsCount"
            ],
            "title": "GetMyStudentCodeReview"
        },
        "CodeReviewRound": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "eventId": {
                    "anyOf": [
                        {
                            "type": "string",
                            "format": "integer"
                        },
                        {
                            "type": "null"
                        }
                    ]
                },
                "codeReviewRoundType": {
                    "type": "string"
                },
                "codeReviewStatus": {
                    "type": "string"
                },
                "startTime": {
                    "type": "string",
                    "format": "date-time"
                },
                "endTime": {
                    "type": "string",
                    "format": "date-time"
                },
                "mergeRequestURL": {
                    "type": "string",
                    "format": "uri",
                    "qt-uri-protocols": [
                        "https"
                    ]
                },
                "createTime": {
                    "type": "string",
                    "format": "date-time"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "codeReviewRoundType",
                "codeReviewStatus",
                "createTime",
                "endTime",
                "eventId",
                "mergeRequestURL",
                "startTime"
            ],
            "title": "CodeReviewRound"
        }
    }
}

```

</details>

[[Index](#index)]

### calendarGetStudentCodeReviews

<details>
<summary> Query </summary>

```
query calendarGetStudentCodeReviews($studentGoalId: ID!) {
  student {
    getStudentCodeReviews(studentGoalId: $studentGoalId) {
      secondRoundStartDate
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "studentGoalId": {
                    "type": "string",
                    "format": "integer"
                }
            },
            "required": [
                "studentGoalId"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getStudentCodeReviews": {
                    "$ref": "#/definitions/GetStudentCodeReviews"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getStudentCodeReviews"
            ],
            "title": "Student"
        },
        "GetStudentCodeReviews": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "secondRoundStartDate": {
                    "type": "string",
                    "format": "date"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "secondRoundStartDate"
            ],
            "title": "GetStudentCodeReviews"
        }
    }
}

```

</details>

[[Index](#index)]

### calendarGetCodeReviewData

<details>
<summary> Query </summary>

```
query calendarGetCodeReviewData($studentGoalId: ID!) {
  student {
    getStudentModuleByStudentGoalId(studentGoalId: $studentGoalId) {
      moduleTitle
      currentTask {
        task {
          studentTaskAdditionalAttributes {
            codeReviewDuration
            __typename
          }
          __typename
        }
        __typename
      }
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "studentGoalId": {
                    "type": "string",
                    "format": "integer"
                }
            },
            "required": [
                "studentGoalId"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getStudentModuleByStudentGoalId": {
                    "$ref": "#/definitions/GetStudentModuleByStudentGoalID"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getStudentModuleByStudentGoalId"
            ],
            "title": "Student"
        },
        "GetStudentModuleByStudentGoalID": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "moduleTitle": {
                    "type": "string"
                },
                "currentTask": {
                    "$ref": "#/definitions/CurrentTask"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "currentTask",
                "moduleTitle"
            ],
            "title": "GetStudentModuleByStudentGoalID"
        },
        "CurrentTask": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "task": {
                    "$ref": "#/definitions/Task"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "task"
            ],
            "title": "CurrentTask"
        },
        "Task": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "studentTaskAdditionalAttributes": {
                    "$ref": "#/definitions/StudentTaskAdditionalAttributes"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "studentTaskAdditionalAttributes"
            ],
            "title": "Task"
        },
        "StudentTaskAdditionalAttributes": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "codeReviewDuration": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "codeReviewDuration"
            ],
            "title": "StudentTaskAdditionalAttributes"
        }
    }
}

```

</details>

[[Index](#index)]

### calendarAddCodeReviewToEventSlot

<details>
<summary> Query </summary>

```
mutation calendarAddCodeReviewToEventSlot($studentGoalId: ID!, $startTime: DateTime!) {
  student {
    addBookingCodeReviewToEventSlot(
      studentGoalId: $studentGoalId
      startTime: $startTime
    ) {
      id
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "studentGoalId": {
                    "type": "string",
                    "format": "integer"
                },
                "startTime": {
                    "type": "string",
                    "format": "date-time"
                }
            },
            "required": [
                "startTime",
                "studentGoalId"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "addBookingCodeReviewToEventSlot": {
                    "$ref": "#/definitions/AddBookingCodeReviewToEventSlot"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "addBookingCodeReviewToEventSlot"
            ],
            "title": "Student"
        },
        "AddBookingCodeReviewToEventSlot": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id"
            ],
            "title": "AddBookingCodeReviewToEventSlot"
        }
    }
}

```

</details>

[[Index](#index)]

### calendarAddBookingToEventSlot

<details>
<summary> Query </summary>

```
mutation calendarAddBookingToEventSlot(
	$answerId: ID!
	$startTime: DateTime!
	$wasStaffSlotChosen: Boolean!
	$isOnline: Boolean
) {
	student {
		addBookingP2PToEventSlot(
			answerId: $answerId
			startTime: $startTime
			wasStaffSlotChosen: $wasStaffSlotChosen
			isOnline: $isOnline
		) {
			id
			__typename
		}
		__typename
	}
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "answerId": {
                    "type": "string",
                    "format": "integer"
                },
                "startTime": {
                    "type": "string"
                },
                "wasStaffSlotChosen": {
                    "type": "string"
                },
                "isOnline": {
                    "type": "boolean"
                }
            },
            "required": [
                "answerId",
                "isOnline",
                "startTime",
                "wasStaffSlotChosen"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "addBookingP2PToEventSlot": {
                    "$ref": "#/definitions/AddBookingP2PToEventSlot"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "addBookingP2PToEventSlot"
            ],
            "title": "Student"
        },
        "AddBookingP2PToEventSlot": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id"
            ],
            "title": "AddBookingP2PToEventSlot"
        }
    }
}

```

</details>

[[Index](#index)]

### getCodeReviewPointChargedOff

<details>
<summary> Query </summary>

```
query getCodeReviewPointChargedOff($goalId: ID!) {
  student {
    getCodeReviewPointChargedOff(goalId: $goalId)
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "goalId": {
                    "type": "string",
                    "format": "integer"
                }
            },
            "required": [
                "goalId"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getCodeReviewPointChargedOff": {
                    "type": "boolean"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getCodeReviewPointChargedOff"
            ],
            "title": "Student"
        }
    }
}

```

</details>

[[Index](#index)]

### getProjectConsistencyInfo

<details>
<summary> Query </summary>

```
query getProjectConsistencyInfo($goalId: ID!) {
  school21 {
    loadGoalConsistencyInfo(goalId: $goalId) {
      goalId
      isConsistent
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "goalId": {
                    "type": "string",
                    "format": "integer"
                }
            },
            "required": [
                "goalId"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "school21": {
                    "$ref": "#/definitions/School21"
                }
            },
            "required": [
                "school21"
            ],
            "title": "Data"
        },
        "School21": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "loadGoalConsistencyInfo": {
                    "$ref": "#/definitions/LoadGoalConsistencyInfo"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "loadGoalConsistencyInfo"
            ],
            "title": "School21"
        },
        "LoadGoalConsistencyInfo": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "goalId": {
                    "type": "string",
                    "format": "integer"
                },
                "isConsistent": {
                    "type": "boolean"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "goalId",
                "isConsistent"
            ],
            "title": "LoadGoalConsistencyInfo"
        }
    }
}

```

</details>

[[Index](#index)]

### getProjectInfo

<details>
<summary> Query </summary>

```
query getProjectInfo($goalId: ID!) {
  student {
    getModuleById(goalId: $goalId) {
      ...ProjectInfo
      __typename
    }
    getModuleCoverInformation(goalId: $goalId) {
      ...ModuleCoverInfo
      __typename
    }
    getP2PChecksInfo(goalId: $goalId) {
      ...P2PInfo
      __typename
    }
    getStudentCodeReviewByGoalId(goalId: $goalId) {
      ...StudentsCodeReview
      __typename
    }
    __typename
  }
}

fragment ProjectInfo on StudentModule {
  id
  moduleTitle
  finalPercentage
  finalPoint
  goalExecutionType
  displayedGoalStatus
  accessBeforeStartProgress
  resultModuleCompletion
  finishedExecutionDateByScheduler
  durationFromStageSubjectGroupPlan
  currentAttemptNumber
  isDeadlineFree
  isRetryAvailable
  localCourseId
  courseBaseParameters {
    isGradedCourse
    __typename
  }
  teamSettings {
    ...teamSettingsInfo
    __typename
  }
  studyModule {
    id
    idea
    duration
    goalPoint
    retrySettings {
      ...RetrySettings
      __typename
    }
    levels {
      id
      goalElements {
        id
        tasks {
          id
          taskId
          __typename
        }
        __typename
      }
      __typename
    }
    __typename
  }
  currentTask {
    ...CurrentInternshipTaskInfo
    __typename
  }
  __typename
}

fragment teamSettingsInfo on TeamSettings {
  teamCreateOption
  minAmountMember
  maxAmountMember
  enableSurrenderTeam
  __typename
}

fragment RetrySettings on ModuleAttemptsSettings {
  maxModuleAttempts
  isUnlimitedAttempts
  __typename
}

fragment CurrentInternshipTaskInfo on StudentTask {
  id
  taskId
  task {
    id
    assignmentType
    studentTaskAdditionalAttributes {
      cookiesCount
      maxCodeReviewCount
      codeReviewCost
      ciCdMode
      __typename
    }
    checkTypes
    __typename
  }
  lastAnswer {
    id
    __typename
  }
  teamSettings {
    ...teamSettingsInfo
    __typename
  }
  __typename
}

fragment ModuleCoverInfo on ModuleCoverInformation {
  isOwnStudentTimeline
  softSkills {
    softSkillId
    softSkillName
    totalPower
    maxPower
    currentUserPower
    achievedUserPower
    teamRole
    __typename
  }
  timeline {
    ...TimelineItem
    __typename
  }
  projectStatistics {
    ...ProjectStatistics
    __typename
  }
  __typename
}

fragment TimelineItem on ProjectTimelineItem {
  type
  status
  start
  end
  children {
    ...TimelineItemChildren
    __typename
  }
  __typename
}

fragment TimelineItemChildren on ProjectTimelineItem {
  type
  elementType
  status
  start
  end
  order
  __typename
}

fragment ProjectStatistics on ProjectStatistics {
  registeredStudents
  inProgressStudents
  evaluationStudents
  finishedStudents
  acceptedStudents
  failedStudents
  retriedStudentsPercentage
  groupProjectStatistics {
    ...GroupProjectStatistics
    __typename
  }
  __typename
}

fragment GroupProjectStatistics on GroupProjectStatistics {
  inProgressTeams
  evaluationTeams
  finishedTeams
  acceptedTeams
  failedTeams
  __typename
}

fragment P2PInfo on P2PChecksInfo {
  cookiesCount
  periodOfVerification
  projectReviewsInfo {
    ...ProjectReviewsInfo
    __typename
  }
  __typename
}

fragment ProjectReviewsInfo on ProjectReviewsInfo {
  reviewByStudentCount
  relevantReviewByStudentsCount
  reviewByInspectionStaffCount
  relevantReviewByInspectionStaffCount
  __typename
}

fragment StudentsCodeReview on StudentCodeReviewsWithCountRound {
  countRound1
  countRound2
  codeReviewsInfo {
    maxCodeReviewCount
    codeReviewDuration
    codeReviewCost
    __typename
  }
  __typename
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "goalId": {
                    "type": "string",
                    "format": "integer"
                }
            },
            "required": [
                "goalId"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getModuleById": {
                    "$ref": "#/definitions/GetModuleByID"
                },
                "getModuleCoverInformation": {
                    "$ref": "#/definitions/GetModuleCoverInformation"
                },
                "getP2PChecksInfo": {
                    "$ref": "#/definitions/GetP2PChecksInfo"
                },
                "getStudentCodeReviewByGoalId": {
                    "$ref": "#/definitions/GetStudentCodeReviewByGoalID"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getModuleById",
                "getModuleCoverInformation",
                "getP2PChecksInfo",
                "getStudentCodeReviewByGoalId"
            ],
            "title": "Student"
        },
        "GetModuleByID": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "moduleTitle": {
                    "type": "string"
                },
                "finalPercentage": {
                    "anyOf": [
                        {
                            "type": "integer"
                        },
                        {
                            "type": "null"
                        }
                    ]
                },
                "finalPoint": {
                    "anyOf": [
                        {
                            "type": "integer"
                        },
                        {
                            "type": "null"
                        }
                    ]
                },
                "goalExecutionType": {
                    "type": "string"
                },
                "displayedGoalStatus": {
                    "type": "string"
                },
                "accessBeforeStartProgress": {
                    "type": "boolean"
                },
                "resultModuleCompletion": {
                    "anyOf": [
                        {
                            "type": "null"
                        },
                        {
                            "type": "string"
                        }
                    ]
                },
                "finishedExecutionDateByScheduler": {
                    "type": "null"
                },
                "durationFromStageSubjectGroupPlan": {
                    "type": "integer"
                },
                "currentAttemptNumber": {
                    "type": "integer"
                },
                "isDeadlineFree": {
                    "type": "boolean"
                },
                "isRetryAvailable": {
                    "type": "boolean"
                },
                "localCourseId": {
                    "type": "null"
                },
                "courseBaseParameters": {
                    "type": "null"
                },
                "teamSettings": {
                    "anyOf": [
                        {
                            "$ref": "#/definitions/TeamSettings"
                        },
                        {
                            "type": "null"
                        }
                    ]
                },
                "studyModule": {
                    "$ref": "#/definitions/StudyModule"
                },
                "currentTask": {
                    "$ref": "#/definitions/CurrentTask"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "accessBeforeStartProgress",
                "currentAttemptNumber",
                "currentTask",
                "displayedGoalStatus",
                "durationFromStageSubjectGroupPlan",
                "finalPercentage",
                "finalPoint",
                "finishedExecutionDateByScheduler",
                "goalExecutionType",
                "id",
                "isDeadlineFree",
                "isRetryAvailable",
                "localCourseId",
                "moduleTitle",
                "resultModuleCompletion",
                "studyModule",
                "teamSettings"
            ],
            "title": "GetModuleByID"
        },
        "CurrentTask": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "taskId": {
                    "type": "string",
                    "format": "integer"
                },
                "task": {
                    "$ref": "#/definitions/CurrentTaskTask"
                },
                "lastAnswer": {
                    "anyOf": [
                        {
                            "$ref": "#/definitions/LastAnswer"
                        },
                        {
                            "type": "null"
                        }
                    ]
                },
                "teamSettings": {
                    "anyOf": [
                        {
                            "$ref": "#/definitions/TeamSettings"
                        },
                        {
                            "type": "null"
                        }
                    ]
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "lastAnswer",
                "task",
                "taskId",
                "teamSettings"
            ],
            "title": "CurrentTask"
        },
        "LastAnswer": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id"
            ],
            "title": "LastAnswer"
        },
        "CurrentTaskTask": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "assignmentType": {
                    "type": "string"
                },
                "studentTaskAdditionalAttributes": {
                    "$ref": "#/definitions/StudentTaskAdditionalAttributes"
                },
                "checkTypes": {
                    "type": "array",
                    "items": {
                        "type": "string"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "assignmentType",
                "checkTypes",
                "id",
                "studentTaskAdditionalAttributes"
            ],
            "title": "CurrentTaskTask"
        },
        "StudentTaskAdditionalAttributes": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "cookiesCount": {
                    "type": "integer"
                },
                "maxCodeReviewCount": {
                    "type": "integer"
                },
                "codeReviewCost": {
                    "type": "integer"
                },
                "ciCdMode": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "ciCdMode",
                "codeReviewCost",
                "cookiesCount",
                "maxCodeReviewCount"
            ],
            "title": "StudentTaskAdditionalAttributes"
        },
        "TeamSettings": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "teamCreateOption": {
                    "type": "string"
                },
                "minAmountMember": {
                    "type": "integer"
                },
                "maxAmountMember": {
                    "type": "integer"
                },
                "enableSurrenderTeam": {
                    "type": "boolean"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "enableSurrenderTeam",
                "maxAmountMember",
                "minAmountMember",
                "teamCreateOption"
            ],
            "title": "TeamSettings"
        },
        "StudyModule": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "idea": {
                    "type": "string"
                },
                "duration": {
                    "type": "integer"
                },
                "goalPoint": {
                    "type": "integer"
                },
                "retrySettings": {
                    "$ref": "#/definitions/RetrySettings"
                },
                "levels": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/Level"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "duration",
                "goalPoint",
                "id",
                "idea",
                "levels",
                "retrySettings"
            ],
            "title": "StudyModule"
        },
        "Level": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "goalElements": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/GoalElement"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "goalElements",
                "id"
            ],
            "title": "Level"
        },
        "GoalElement": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "tasks": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/TaskElement"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "tasks"
            ],
            "title": "GoalElement"
        },
        "TaskElement": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "taskId": {
                    "type": "string",
                    "format": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "taskId"
            ],
            "title": "TaskElement"
        },
        "RetrySettings": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "maxModuleAttempts": {
                    "type": "integer"
                },
                "isUnlimitedAttempts": {
                    "type": "boolean"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "isUnlimitedAttempts",
                "maxModuleAttempts"
            ],
            "title": "RetrySettings"
        },
        "GetModuleCoverInformation": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "isOwnStudentTimeline": {
                    "type": "boolean"
                },
                "softSkills": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/SoftSkill"
                    }
                },
                "timeline": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/Timeline"
                    }
                },
                "projectStatistics": {
                    "$ref": "#/definitions/ProjectStatistics"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "isOwnStudentTimeline",
                "projectStatistics",
                "softSkills",
                "timeline"
            ],
            "title": "GetModuleCoverInformation"
        },
        "ProjectStatistics": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "registeredStudents": {
                    "type": "integer"
                },
                "inProgressStudents": {
                    "type": "integer"
                },
                "evaluationStudents": {
                    "type": "integer"
                },
                "finishedStudents": {
                    "type": "integer"
                },
                "acceptedStudents": {
                    "type": "integer"
                },
                "failedStudents": {
                    "type": "integer"
                },
                "retriedStudentsPercentage": {
                    "type": "integer"
                },
                "groupProjectStatistics": {
                    "anyOf": [
                        {
                            "$ref": "#/definitions/GroupProjectStatistics"
                        },
                        {
                            "type": "null"
                        }
                    ]
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "acceptedStudents",
                "evaluationStudents",
                "failedStudents",
                "finishedStudents",
                "groupProjectStatistics",
                "inProgressStudents",
                "registeredStudents",
                "retriedStudentsPercentage"
            ],
            "title": "ProjectStatistics"
        },
        "GroupProjectStatistics": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "inProgressTeams": {
                    "type": "integer"
                },
                "evaluationTeams": {
                    "type": "integer"
                },
                "finishedTeams": {
                    "type": "integer"
                },
                "acceptedTeams": {
                    "type": "integer"
                },
                "failedTeams": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "acceptedTeams",
                "evaluationTeams",
                "failedTeams",
                "finishedTeams",
                "inProgressTeams"
            ],
            "title": "GroupProjectStatistics"
        },
        "SoftSkill": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "softSkillId": {
                    "type": "integer"
                },
                "softSkillName": {
                    "type": "string"
                },
                "totalPower": {
                    "type": "integer"
                },
                "maxPower": {
                    "type": "integer"
                },
                "currentUserPower": {
                    "type": "integer"
                },
                "achievedUserPower": {
                    "anyOf": [
                        {
                            "type": "integer"
                        },
                        {
                            "type": "null"
                        }
                    ]
                },
                "teamRole": {
                    "anyOf": [
                        {
                            "type": "null"
                        },
                        {
                            "type": "string"
                        }
                    ]
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "achievedUserPower",
                "currentUserPower",
                "maxPower",
                "softSkillId",
                "softSkillName",
                "teamRole",
                "totalPower"
            ],
            "title": "SoftSkill"
        },
        "Timeline": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "type": {
                    "type": "string"
                },
                "status": {
                    "type": "string"
                },
                "start": {
                    "type": "null"
                },
                "end": {
                    "type": "null"
                },
                "children": {
                    "anyOf": [
                        {
                            "type": "array",
                            "items": {
                                "$ref": "#/definitions/Child"
                            }
                        },
                        {
                            "type": "null"
                        }
                    ]
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "children",
                "end",
                "start",
                "status",
                "type"
            ],
            "title": "Timeline"
        },
        "Child": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "type": {
                    "type": "string"
                },
                "elementType": {
                    "type": "string"
                },
                "status": {
                    "type": "string"
                },
                "start": {
                    "anyOf": [
                        {
                            "type": "string",
                            "format": "date-time"
                        },
                        {
                            "type": "null"
                        }
                    ]
                },
                "end": {
                    "anyOf": [
                        {
                            "type": "string",
                            "format": "date-time"
                        },
                        {
                            "type": "null"
                        }
                    ]
                },
                "order": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "elementType",
                "end",
                "order",
                "start",
                "status",
                "type"
            ],
            "title": "Child"
        },
        "GetP2PChecksInfo": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "cookiesCount": {
                    "type": "integer"
                },
                "periodOfVerification": {
                    "type": "integer"
                },
                "projectReviewsInfo": {
                    "$ref": "#/definitions/ProjectReviewsInfo"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "cookiesCount",
                "periodOfVerification",
                "projectReviewsInfo"
            ],
            "title": "GetP2PChecksInfo"
        },
        "ProjectReviewsInfo": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "reviewByStudentCount": {
                    "type": "integer"
                },
                "relevantReviewByStudentsCount": {
                    "type": "integer"
                },
                "reviewByInspectionStaffCount": {
                    "type": "integer"
                },
                "relevantReviewByInspectionStaffCount": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "relevantReviewByInspectionStaffCount",
                "relevantReviewByStudentsCount",
                "reviewByInspectionStaffCount",
                "reviewByStudentCount"
            ],
            "title": "ProjectReviewsInfo"
        },
        "GetStudentCodeReviewByGoalID": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "countRound1": {
                    "type": "integer"
                },
                "countRound2": {
                    "type": "integer"
                },
                "codeReviewsInfo": {
                    "type": "null"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "codeReviewsInfo",
                "countRound1",
                "countRound2"
            ],
            "title": "GetStudentCodeReviewByGoalID"
        }
    }
}

```

</details>

[[Index](#index)]

### getProjectAttemptEvaluationsInfo

<details>
<summary> Query </summary>

```
query getProjectAttemptEvaluationsInfo($goalId: ID!, $studentId: UUID!) {
  school21 {
    getProjectAttemptEvaluationsInfo_V1(goalId: $goalId, studentId: $studentId) {
      ...ProjectAttemptEvaluations_V1
      __typename
    }
    __typename
  }
}

fragment ProjectAttemptEvaluations_V1 on ProjectAttemptEvaluationsInfo_V1 {
  studentAnswerId
  studentGoalAttemptId
  attemptStatus
  attemptResult {
    ...AtemptResult
    __typename
  }
  team {
    ...AttemptTeamWithMembers
    __typename
  }
  p2p {
    ...P2PEvaluation
    __typename
  }
  auto {
    status
    receivedPercentage
    endTimeCheck
    resultInfo
    __typename
  }
  codeReview {
    averageMark
    studentCodeReviews {
      user {
        avatarUrl
        login
        __typename
      }
      finalMark
      markTime
      reviewerCommentsCount
      __typename
    }
    __typename
  }
  __typename
}

fragment AtemptResult on StudentGoalAttempt {
  finalPointProject
  finalPercentageProject
  resultModuleCompletion
  resultDate
  __typename
}

fragment AttemptTeamWithMembers on TeamWithMembers {
  team {
    id
    name
    __typename
  }
  members {
    ...TeamMemberWithRole
    __typename
  }
  __typename
}

fragment TeamMemberWithRole on TeamMember {
  role
  user {
    ...ProjectTeamMember
    __typename
  }
  __typename
}

fragment ProjectTeamMember on User {
  id
  avatarUrl
  login
  userExperience {
    level {
      id
      range {
        levelCode
        __typename
      }
      __typename
    }
    cookiesCount
    codeReviewPoints
    __typename
  }
  __typename
}

fragment P2PEvaluation on P2PEvaluationInfo {
  status
  checklist {
    ...Checklist
    __typename
  }
  __typename
}

fragment Checklist on FilledChecklist {
  id
  checklistId
  endTimeCheck
  startTimeCheck
  reviewer {
    avatarUrl
    login
    businessAdminRoles {
      id
      school {
        id
        organizationType
        __typename
      }
      __typename
    }
    __typename
  }
  reviewFeedback {
    ...EvaluationFeedback
    __typename
  }
  comment
  receivedPoint
  receivedPercentage
  quickAction
  checkType
  video {
    ...P2PReviewVideo
    __typename
  }
  __typename
}

fragment EvaluationFeedback on ReviewFeedback {
  id
  comment
  filledChecklist {
    id
    __typename
  }
  reviewFeedbackCategoryValues {
    feedbackCategory
    feedbackValue
    id
    __typename
  }
  __typename
}

fragment P2PReviewVideo on OnlineReviewVideo {
  link
  status
  __typename
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "goalId": {
                    "type": "string",
                    "format": "integer"
                },
                "studentId": {
                    "type": "string",
                    "format": "uuid"
                }
            },
            "required": [
                "goalId",
                "studentId"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "school21": {
                    "$ref": "#/definitions/School21"
                }
            },
            "required": [
                "school21"
            ],
            "title": "Data"
        },
        "School21": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getProjectAttemptEvaluationsInfo_V1": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/GetProjectAttemptEvaluationsInfoV1"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getProjectAttemptEvaluationsInfo_V1"
            ],
            "title": "School21"
        },
        "GetProjectAttemptEvaluationsInfoV1": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "studentAnswerId": {
                    "anyOf": [
                        {
                            "type": "string",
                            "format": "integer"
                        },
                        {
                            "type": "null"
                        }
                    ]
                },
                "studentGoalAttemptId": {
                    "type": "string",
                    "format": "integer"
                },
                "attemptStatus": {
                    "type": "string"
                },
                "attemptResult": {
                    "anyOf": [
                        {
                            "$ref": "#/definitions/AttemptResult"
                        },
                        {
                            "type": "null"
                        }
                    ]
                },
                "team": {
                    "type": "null"
                },
                "p2p": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/P2P"
                    }
                },
                "auto": {
                    "$ref": "#/definitions/Auto"
                },
                "codeReview": {
                    "$ref": "#/definitions/CodeReview"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "attemptResult",
                "auto",
                "codeReview",
                "p2p",
                "studentAnswerId",
                "studentGoalAttemptId",
                "team"
            ],
            "title": "GetProjectAttemptEvaluationsInfoV1"
        },
        "AttemptResult": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "finalPointProject": {
                    "type": "integer"
                },
                "finalPercentageProject": {
                    "type": "integer"
                },
                "resultModuleCompletion": {
                    "type": "string"
                },
                "resultDate": {
                    "type": "string",
                    "format": "date-time"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "finalPercentageProject",
                "finalPointProject",
                "resultDate",
                "resultModuleCompletion"
            ],
            "title": "AttemptResult"
        },
        "Auto": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "status": {
                    "type": "string"
                },
                "receivedPercentage": {
                    "type": "integer"
                },
                "endTimeCheck": {
                    "type": "null"
                },
                "resultInfo": {
                    "type": "null"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "endTimeCheck",
                "receivedPercentage",
                "resultInfo",
                "status"
            ],
            "title": "Auto"
        },
        "CodeReview": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "averageMark": {
                    "anyOf": [
                        {
                            "type": "null"
                        },
                        {
                            "type": "string"
                        }
                    ]
                },
                "studentCodeReviews": {
                    "type": "array",
                    "items": {}
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "averageMark",
                "studentCodeReviews"
            ],
            "title": "CodeReview"
        },
        "P2P": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "status": {
                    "type": "string"
                },
                "checklist": {
                    "anyOf": [
                        {
                            "$ref": "#/definitions/Checklist"
                        },
                        {
                            "type": "null"
                        }
                    ]
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "checklist",
                "status"
            ],
            "title": "P2P"
        },
        "Checklist": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "checklistId": {
                    "type": "string",
                    "format": "integer"
                },
                "endTimeCheck": {
                    "type": "string",
                    "format": "date-time"
                },
                "startTimeCheck": {
                    "type": "string",
                    "format": "date-time"
                },
                "reviewer": {
                    "$ref": "#/definitions/Reviewer"
                },
                "reviewFeedback": {
                    "anyOf": [
                        {
                            "$ref": "#/definitions/ReviewFeedback"
                        },
                        {
                            "type": "null"
                        }
                    ]
                },
                "comment": {
                    "type": "string"
                },
                "receivedPoint": {
                    "type": "integer"
                },
                "receivedPercentage": {
                    "type": "integer"
                },
                "quickAction": {
                    "type": "null"
                },
                "checkType": {
                    "type": "string"
                },
                "video": {
                    "type": "null"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "checkType",
                "checklistId",
                "comment",
                "endTimeCheck",
                "id",
                "quickAction",
                "receivedPercentage",
                "receivedPoint",
                "reviewFeedback",
                "reviewer",
                "startTimeCheck",
                "video"
            ],
            "title": "Checklist"
        },
        "ReviewFeedback": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "comment": {
                    "type": "string"
                },
                "filledChecklist": {
                    "$ref": "#/definitions/FilledChecklist"
                },
                "reviewFeedbackCategoryValues": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/ReviewFeedbackCategoryValue"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "comment",
                "filledChecklist",
                "id",
                "reviewFeedbackCategoryValues"
            ],
            "title": "ReviewFeedback"
        },
        "FilledChecklist": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id"
            ],
            "title": "FilledChecklist"
        },
        "ReviewFeedbackCategoryValue": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "feedbackCategory": {
                    "type": "string"
                },
                "feedbackValue": {
                    "type": "string"
                },
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "feedbackCategory",
                "feedbackValue",
                "id"
            ],
            "title": "ReviewFeedbackCategoryValue"
        },
        "Reviewer": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "avatarUrl": {
                    "type": "string"
                },
                "login": {
                    "type": "string"
                },
                "businessAdminRoles": {
                    "type": "array",
                    "items": {}
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "avatarUrl",
                "businessAdminRoles",
                "login"
            ],
            "title": "Reviewer"
        }
    }
}

```

</details>

[[Index](#index)]

### getProjectGitlabStatus

<details>
<summary> Query </summary>

```
query getProjectGitlabStatus($taskId: ID!) {
  student {
    getGitlabLinksWithStatus(taskId: $taskId) {
      id
      sshLink
      httpsLink
      readyToUse
      restartsCounter
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "taskId": {
                    "type": "string",
                    "format": "integer"
                }
            },
            "required": [
                "taskId"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getGitlabLinksWithStatus": {
                    "$ref": "#/definitions/GetGitlabLinksWithStatus"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getGitlabLinksWithStatus"
            ],
            "title": "Student"
        },
        "GetGitlabLinksWithStatus": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "integer"
                },
                "sshLink": {
                    "type": "string"
                },
                "httpsLink": {
                    "type": "string",
                    "format": "uri",
                    "qt-uri-protocols": [
                        "https"
                    ],
                    "qt-uri-extensions": [
                        ".git"
                    ]
                },
                "readyToUse": {
                    "type": "string"
                },
                "restartsCounter": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "httpsLink",
                "id",
                "readyToUse",
                "restartsCounter",
                "sshLink"
            ],
            "title": "GetGitlabLinksWithStatus"
        }
    }
}

```

</details>

[[Index](#index)]

### calendarGetModule

<details>
<summary> Query </summary>

```
query calendarGetModule($moduleId: ID!) {
  student {
    getModuleById(goalId: $moduleId) {
      id
      moduleTitle
      subjectTitle
      goalExecutionType
      trajectory {
        ...CalendarModuleTrajectory
        __typename
      }
      currentTask {
        id
        task {
          id
          assignmentType
          __typename
        }
        __typename
      }
      __typename
    }
    __typename
  }
}

fragment CalendarModuleTrajectory on PersonalTrajectory {
  id
  levels {
    id
    goalElements {
      id
      points {
        id
        studentTask {
          ...CalendarStudentTask
          __typename
        }
        __typename
      }
      __typename
    }
    __typename
  }
  __typename
}

fragment CalendarStudentTask on StudentTask {
  id
  taskId
  task {
    id
    studentTaskAdditionalAttributes {
      ...CalendarStudentTaskAdditionalAttributes
      __typename
    }
    __typename
  }
  lastAnswer {
    id
    __typename
  }
  __typename
}

fragment CalendarStudentTaskAdditionalAttributes on StudentTaskAdditionalAttributes {
  cookiesCount
  __typename
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "moduleId": {
                    "type": "string",
                    "format": "integer"
                }
            },
            "required": [
                "moduleId"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getModuleById": {
                    "$ref": "#/definitions/GetModuleByID"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getModuleById"
            ],
            "title": "Student"
        },
        "GetModuleByID": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "moduleTitle": {
                    "type": "string"
                },
                "subjectTitle": {
                    "type": "string"
                },
                "goalExecutionType": {
                    "type": "string"
                },
                "trajectory": {
                    "$ref": "#/definitions/Trajectory"
                },
                "currentTask": {
                    "$ref": "#/definitions/CurrentTask"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "currentTask",
                "goalExecutionType",
                "id",
                "moduleTitle",
                "subjectTitle",
                "trajectory"
            ],
            "title": "GetModuleByID"
        },
        "CurrentTask": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "task": {
                    "$ref": "#/definitions/CurrentTaskTask"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "task"
            ],
            "title": "CurrentTask"
        },
        "CurrentTaskTask": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "assignmentType": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "assignmentType",
                "id"
            ],
            "title": "CurrentTaskTask"
        },
        "Trajectory": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "levels": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/Level"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "levels"
            ],
            "title": "Trajectory"
        },
        "Level": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "goalElements": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/GoalElement"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "goalElements",
                "id"
            ],
            "title": "Level"
        },
        "GoalElement": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "points": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/Point"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "points"
            ],
            "title": "GoalElement"
        },
        "Point": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "studentTask": {
                    "$ref": "#/definitions/StudentTask"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "studentTask"
            ],
            "title": "Point"
        },
        "StudentTask": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "taskId": {
                    "type": "string",
                    "format": "integer"
                },
                "task": {
                    "$ref": "#/definitions/StudentTaskTask"
                },
                "lastAnswer": {
                    "$ref": "#/definitions/LastAnswer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "lastAnswer",
                "task",
                "taskId"
            ],
            "title": "StudentTask"
        },
        "LastAnswer": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id"
            ],
            "title": "LastAnswer"
        },
        "StudentTaskTask": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "studentTaskAdditionalAttributes": {
                    "$ref": "#/definitions/StudentTaskAdditionalAttributes"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "studentTaskAdditionalAttributes"
            ],
            "title": "StudentTaskTask"
        },
        "StudentTaskAdditionalAttributes": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "cookiesCount": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "cookiesCount"
            ],
            "title": "StudentTaskAdditionalAttributes"
        }
    }
}

```

</details>

[[Index](#index)]

### calendarGetNameLessStudentTimeslotsForReview

<details>
<summary> Query </summary>

```
query calendarGetNameLessStudentTimeslotsForReview($from: DateTime!, $taskId: ID!, $to: DateTime!) {
  student {
    getNameLessStudentTimeslotsForReview(from: $from, taskId: $taskId, to: $to) {
      checkDuration
      projectReviewsInfo {
        ...ProjectReviewsInfo
        __typename
      }
      timeSlots {
        ...CalendarNameLessTimeslot
        __typename
      }
      __typename
    }
    __typename
  }
}

fragment ProjectReviewsInfo on ProjectReviewsInfo {
  reviewByStudentCount
  relevantReviewByStudentsCount
  reviewByInspectionStaffCount
  relevantReviewByInspectionStaffCount
  __typename
}

fragment CalendarNameLessTimeslot on CalendarNamelessTimeSlot {
  start
  end
  validStartTimes
  staffSlot
  __typename
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "taskId": {
                    "type": "string",
                    "format": "integer"
                },
                "from": {
                    "type": "string",
                    "format": "date-time"
                },
                "to": {
                    "type": "string",
                    "format": "date-time"
                }
            },
            "required": [
                "from",
                "taskId",
                "to"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getNameLessStudentTimeslotsForReview": {
                    "$ref": "#/definitions/GetNameLessStudentTimeslotsForReview"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getNameLessStudentTimeslotsForReview"
            ],
            "title": "Student"
        },
        "GetNameLessStudentTimeslotsForReview": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "checkDuration": {
                    "type": "integer"
                },
                "projectReviewsInfo": {
                    "$ref": "#/definitions/ProjectReviewsInfo"
                },
                "timeSlots": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/TimeSlot"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "checkDuration",
                "projectReviewsInfo",
                "timeSlots"
            ],
            "title": "GetNameLessStudentTimeslotsForReview"
        },
        "ProjectReviewsInfo": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "reviewByStudentCount": {
                    "type": "integer"
                },
                "relevantReviewByStudentsCount": {
                    "type": "integer"
                },
                "reviewByInspectionStaffCount": {
                    "type": "integer"
                },
                "relevantReviewByInspectionStaffCount": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "relevantReviewByInspectionStaffCount",
                "relevantReviewByStudentsCount",
                "reviewByInspectionStaffCount",
                "reviewByStudentCount"
            ],
            "title": "ProjectReviewsInfo"
        },
        "TimeSlot": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "start": {
                    "type": "string",
                    "format": "date-time"
                },
                "end": {
                    "type": "string",
                    "format": "date-time"
                },
                "validStartTimes": {
                    "type": "array",
                    "items": {
                        "type": "string",
                        "format": "date-time"
                    }
                },
                "staffSlot": {
                    "type": "boolean"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "end",
                "staffSlot",
                "start",
                "validStartTimes"
            ],
            "title": "TimeSlot"
        }
    }
}

```

</details>

[[Index](#index)]

### bonusesGetBadgesWithFakePublicProfile

<details>
<summary> Query </summary>

```
query bonusesGetBadgesWithFakePublicProfile($userId: UUID) {
  student {
    getBadgesWithFakePublicProfile(userId: $userId) {
      ...UserAchievements
      __typename
    }
    __typename
  }
}

fragment UserAchievements on UserBadgeAward {
  id
  histories {
    id
    rewardDate
    awardPoints
    __typename
  }
  badge {
    id
    kind {
      id
      name
      order
      __typename
    }
    name
    description
    avatarUrl
    bigAvatarUrl
    __typename
  }
  award {
    id
    awardCondition {
      id
      description
      __typename
    }
    awardBounties {
      awardBountyId
      description
      cookies
      coins
      experienceValue
      coalitionPoints
      softSkillPowers {
        softSkillId
        power
        softSkill {
          id
          name
          __typename
        }
        __typename
      }
      __typename
    }
    __typename
  }
  points
  isFake
  __typename
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "userId": {
                    "anyOf": [
                        {
                            "type": "null"
                        },
                        {
                            "type": "string",
                            "format": "uuid"
                        }
                    ]
                }
            },
            "required": [
                "userId"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getBadgesWithFakePublicProfile": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/GetBadgesWithFakePublicProfile"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getBadgesWithFakePublicProfile"
            ],
            "title": "Student"
        },
        "GetBadgesWithFakePublicProfile": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "histories": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/History"
                    }
                },
                "badge": {
                    "$ref": "#/definitions/Badge"
                },
                "award": {
                    "$ref": "#/definitions/Award"
                },
                "points": {
                    "type": "integer"
                },
                "isFake": {
                    "type": "boolean"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "award",
                "badge",
                "histories",
                "id",
                "isFake",
                "points"
            ],
            "title": "GetBadgesWithFakePublicProfile"
        },
        "Award": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "awardCondition": {
                    "$ref": "#/definitions/AwardCondition"
                },
                "awardBounties": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/AwardBounty"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "awardBounties",
                "awardCondition",
                "id"
            ],
            "title": "Award"
        },
        "AwardBounty": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "awardBountyId": {
                    "type": "string",
                    "format": "integer"
                },
                "description": {
                    "type": "string"
                },
                "cookies": {
                    "type": "integer"
                },
                "coins": {
                    "type": "integer"
                },
                "experienceValue": {
                    "type": "integer"
                },
                "coalitionPoints": {
                    "type": "integer"
                },
                "softSkillPowers": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/SoftSkillPower"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "awardBountyId",
                "coalitionPoints",
                "coins",
                "cookies",
                "description",
                "experienceValue",
                "softSkillPowers"
            ],
            "title": "AwardBounty"
        },
        "SoftSkillPower": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "softSkillId": {
                    "type": "integer"
                },
                "power": {
                    "type": "integer"
                },
                "softSkill": {
                    "$ref": "#/definitions/SoftSkill"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "power",
                "softSkill",
                "softSkillId"
            ],
            "title": "SoftSkillPower"
        },
        "SoftSkill": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "name": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "name"
            ],
            "title": "SoftSkill"
        },
        "AwardCondition": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "integer"
                },
                "description": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "description",
                "id"
            ],
            "title": "AwardCondition"
        },
        "Badge": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "kind": {
                    "$ref": "#/definitions/Kind"
                },
                "name": {
                    "type": "string"
                },
                "description": {
                    "type": "string"
                },
                "avatarUrl": {
                    "type": "string"
                },
                "bigAvatarUrl": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "avatarUrl",
                "bigAvatarUrl",
                "description",
                "id",
                "kind",
                "name"
            ],
            "title": "Badge"
        },
        "Kind": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "integer"
                },
                "name": {
                    "type": "string"
                },
                "order": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "name",
                "order"
            ],
            "title": "Kind"
        },
        "History": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "rewardDate": {
                    "type": "string",
                    "format": "date-time"
                },
                "awardPoints": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "awardPoints",
                "id",
                "rewardDate"
            ],
            "title": "History"
        }
    }
}

```

</details>

[[Index](#index)]

### getCampusCurrentUser

<details>
<summary> Query </summary>

```
query getCampusCurrentUser {
  user {
    getCurrentUser {
      id
      login
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "user": {
                    "$ref": "#/definitions/User"
                }
            },
            "required": [
                "user"
            ],
            "title": "Data"
        },
        "User": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getCurrentUser": {
                    "$ref": "#/definitions/GetCurrentUser"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getCurrentUser"
            ],
            "title": "User"
        },
        "GetCurrentUser": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "login": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "login"
            ],
            "title": "GetCurrentUser"
        }
    }
}

```

</details>

[[Index](#index)]

### getCampusWorkstation

<details>
<summary> Query </summary>

```
query getCampusWorkstation($login: String!) {
  student {
    getWorkstationByLogin(login: $login) {
      id
      classroomId
      hostName
      workstationRow
      workstationNumber
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "login": {
                    "type": "string"
                }
            },
            "required": [
                "login"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getWorkstationByLogin": {
                    "type": "null"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getWorkstationByLogin"
            ],
            "title": "Student"
        }
    }
}

```

</details>

[[Index](#index)]

### getCampusBuildings

<details>
<summary> Query </summary>

```
query getCampusBuildings {
  student {
    getBuildings {
      id
      name
      classrooms {
        id
        number
        capacity
        availableCapacity
        floor
        classroomPlan {
          classroomPlanId
          planMeta
          __typename
        }
        specializations
        __typename
      }
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getBuildings": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/GetBuilding"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getBuildings"
            ],
            "title": "Student"
        },
        "GetBuilding": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "name": {
                    "type": "string"
                },
                "classrooms": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/Classroom"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "classrooms",
                "id",
                "name"
            ],
            "title": "GetBuilding"
        },
        "Classroom": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "number": {
                    "type": "string"
                },
                "capacity": {
                    "type": "integer"
                },
                "availableCapacity": {
                    "type": "integer"
                },
                "floor": {
                    "type": "integer"
                },
                "classroomPlan": {
                    "$ref": "#/definitions/ClassroomPlan"
                },
                "specializations": {
                    "type": "array",
                    "items": {
                        "type": "string"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "availableCapacity",
                "capacity",
                "classroomPlan",
                "floor",
                "id",
                "number",
                "specializations"
            ],
            "title": "Classroom"
        },
        "ClassroomPlan": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "classroomPlanId": {
                    "type": "string",
                    "format": "integer"
                },
                "planMeta": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "classroomPlanId",
                "planMeta"
            ],
            "title": "ClassroomPlan"
        }
    }
}

```

</details>

[[Index](#index)]

### getCampusPlanOccupied

<details>
<summary> Query </summary>

```
query getCampusPlanOccupied($clusterId: ID!) {
  student {
    getClusterPlanStudentsByClusterId(clusterId: $clusterId) {
      occupiedPlaces {
        row
        number
        stageGroupName
        stageName
        user {
          id
          login
          avatarUrl
          __typename
        }
        experience {
          id
          value
          level {
            id
            range {
              id
              levelCode
              leftBorder
              rightBorder
              __typename
            }
            __typename
          }
          __typename
        }
        studentType
        __typename
      }
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "clusterId": {
                    "type": "string",
                    "format": "integer"
                }
            },
            "required": [
                "clusterId"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getClusterPlanStudentsByClusterId": {
                    "$ref": "#/definitions/GetClusterPlanStudentsByClusterID"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getClusterPlanStudentsByClusterId"
            ],
            "title": "Student"
        },
        "GetClusterPlanStudentsByClusterID": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "occupiedPlaces": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/OccupiedPlace"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "occupiedPlaces"
            ],
            "title": "GetClusterPlanStudentsByClusterID"
        },
        "OccupiedPlace": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "row": {
                    "type": "string"
                },
                "number": {
                    "type": "integer"
                },
                "stageGroupName": {
                    "type": "string"
                },
                "stageName": {
                    "type": "string"
                },
                "user": {
                    "$ref": "#/definitions/User"
                },
                "experience": {
                    "$ref": "#/definitions/Experience"
                },
                "studentType": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "experience",
                "number",
                "row",
                "stageGroupName",
                "stageName",
                "studentType",
                "user"
            ],
            "title": "OccupiedPlace"
        },
        "Experience": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "value": {
                    "type": "integer"
                },
                "level": {
                    "$ref": "#/definitions/Level"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "level",
                "value"
            ],
            "title": "Experience"
        },
        "Level": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "integer"
                },
                "range": {
                    "$ref": "#/definitions/Range"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "range"
            ],
            "title": "Level"
        },
        "Range": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "levelCode": {
                    "type": "integer"
                },
                "leftBorder": {
                    "type": "integer"
                },
                "rightBorder": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "leftBorder",
                "levelCode",
                "rightBorder"
            ],
            "title": "Range"
        },
        "User": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "login": {
                    "type": "string"
                },
                "avatarUrl": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "avatarUrl",
                "id",
                "login"
            ],
            "title": "User"
        }
    }
}

```

</details>

[[Index](#index)]

### calendarAddEvent

<details>
<summary> Query </summary>

```
mutation calendarAddEvent($start: DateTime!, $end: DateTime!) {
  student {
    addEventToTimetable(start: $start, end: $end) {
      ...CalendarEvent
      __typename
    }
    __typename
  }
}

fragment CalendarEvent on CalendarEvent {
  id
  start
  end
  description
  eventType
  eventCode
  eventSlots {
    id
    type
    start
    end
    __typename
  }
  bookings {
    ...CalendarReviewBooking
    __typename
  }
  exam {
    ...CalendarEventExam
    __typename
  }
  studentCodeReview {
    studentGoalId
    __typename
  }
  activity {
    ...CalendarEventActivity
    studentFeedback {
      id
      rating
      comment
      __typename
    }
    status
    activityType
    isMandatory
    isWaitListActive
    isVisible
    comments {
      type
      createTs
      comment
      __typename
    }
    organizers {
      id
      login
      __typename
    }
    __typename
  }
  goals {
    goalId
    goalName
    __typename
  }
  penalty {
    ...Penalty
    __typename
  }
  __typename
}

fragment CalendarReviewBooking on CalendarBooking {
  id
  answerId
  eventSlotId
  task {
    id
    goalId
    goalName
    studentTaskAdditionalAttributes {
      cookiesCount
      __typename
    }
    assignmentType
    __typename
  }
  eventSlot {
    id
    start
    end
    event {
      eventUserRole
      __typename
    }
    __typename
  }
  verifierUser {
    ...CalendarReviewUser
    __typename
  }
  verifiableStudent {
    id
    user {
      ...CalendarReviewUser
      __typename
    }
    __typename
  }
  bookingStatus
  team {
    ...ProjectTeamMembers
    __typename
  }
  isOnline
  vcLinkUrl
  __typename
}

fragment CalendarReviewUser on User {
  id
  login
  __typename
}

fragment ProjectTeamMembers on ProjectTeamMembers {
  id
  teamLead {
    ...ProjectTeamMember
    __typename
  }
  members {
    ...ProjectTeamMember
    __typename
  }
  invitedUsers {
    ...ProjectTeamMember
    __typename
  }
  teamName
  teamStatus
  minTeamMemberCount
  maxTeamMemberCount
  __typename
}

fragment ProjectTeamMember on User {
  id
  avatarUrl
  login
  userExperience {
    level {
      id
      range {
        levelCode
        __typename
      }
      __typename
    }
    cookiesCount
    codeReviewPoints
    __typename
  }
  __typename
}

fragment CalendarEventExam on Exam {
  examId
  eventId
  beginDate
  endDate
  name
  location
  currentStudentsCount
  maxStudentCount
  updateDate
  goalId
  goalName
  isWaitListActive
  isInWaitList
  stopRegisterDate
  __typename
}

fragment CalendarEventActivity on ActivityEvent {
  activityEventId
  eventId
  name
  beginDate
  endDate
  isRegistered
  description
  currentStudentsCount
  maxStudentCount
  location
  updateDate
  isWaitListActive
  isInWaitList
  stopRegisterDate
  __typename
}

fragment Penalty on Penalty {
  comment
  id
  duration
  status
  startTime
  createTime
  penaltySlot {
    currentStudentsCount
    description
    duration
    startTime
    id
    endTime
    __typename
  }
  reasonId
  __typename
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "start": {
                    "type": "string",
                    "format": "date-time"
                },
                "end": {
                    "type": "string",
                    "format": "date-time"
                }
            },
            "required": [
                "end",
                "start"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "addEventToTimetable": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/AddEventToTimetable"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "addEventToTimetable"
            ],
            "title": "Student"
        },
        "AddEventToTimetable": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "start": {
                    "type": "string",
                    "format": "date-time"
                },
                "end": {
                    "type": "string",
                    "format": "date-time"
                },
                "description": {
                    "type": "string"
                },
                "eventType": {
                    "type": "string"
                },
                "eventCode": {
                    "type": "null"
                },
                "eventSlots": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/EventSlot"
                    }
                },
                "bookings": {
                    "type": "array",
                    "items": {}
                },
                "exam": {
                    "type": "null"
                },
                "studentCodeReview": {
                    "type": "null"
                },
                "activity": {
                    "type": "null"
                },
                "goals": {
                    "type": "array",
                    "items": {}
                },
                "penalty": {
                    "type": "null"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "activity",
                "bookings",
                "description",
                "end",
                "eventCode",
                "eventSlots",
                "eventType",
                "exam",
                "goals",
                "id",
                "penalty",
                "start",
                "studentCodeReview"
            ],
            "title": "AddEventToTimetable"
        },
        "EventSlot": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "type": {
                    "type": "string"
                },
                "start": {
                    "type": "string",
                    "format": "date-time"
                },
                "end": {
                    "type": "string",
                    "format": "date-time"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "end",
                "id",
                "start",
                "type"
            ],
            "title": "EventSlot"
        }
    }
}

```

</details>

[[Index](#index)]

### getActivityTypes

<details>
<summary> Query </summary>

```
query getActivityTypes {
  school21 {
    getActivityTypes {
      id
      description
      category
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "school21": {
                    "$ref": "#/definitions/School21"
                }
            },
            "required": [
                "school21"
            ],
            "title": "Data"
        },
        "School21": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getActivityTypes": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/GetActivityType"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getActivityTypes"
            ],
            "title": "School21"
        },
        "GetActivityType": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "description": {
                    "type": "string"
                },
                "category": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "category",
                "description",
                "id"
            ],
            "title": "GetActivityType"
        }
    }
}

```

</details>

[[Index](#index)]

### getStageInfo

<details>
<summary> Query </summary>

```
query getStageInfo {
  user {
    getCurrentUser {
      id
      studentRoles {
        status
        school {
          organizationType
          __typename
        }
        stageGroup {
          classSubjects {
            stage {
              name
              __typename
            }
            __typename
          }
          name
          stage
          isActive
          __typename
        }
        __typename
      }
      __typename
    }
    getAllStagesTenantAware {
      id
      name
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "user": {
                    "$ref": "#/definitions/User"
                }
            },
            "required": [
                "user"
            ],
            "title": "Data"
        },
        "User": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getCurrentUser": {
                    "$ref": "#/definitions/GetCurrentUser"
                },
                "getAllStagesTenantAware": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/GetAllStagesTenantAware"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getAllStagesTenantAware",
                "getCurrentUser"
            ],
            "title": "User"
        },
        "GetAllStagesTenantAware": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "name": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "name"
            ],
            "title": "GetAllStagesTenantAware"
        },
        "GetCurrentUser": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "studentRoles": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/StudentRole"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "studentRoles"
            ],
            "title": "GetCurrentUser"
        },
        "StudentRole": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "status": {
                    "type": "string"
                },
                "school": {
                    "$ref": "#/definitions/School"
                },
                "stageGroup": {
                    "$ref": "#/definitions/StageGroup"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "school",
                "stageGroup",
                "status"
            ],
            "title": "StudentRole"
        },
        "School": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "organizationType": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "organizationType"
            ],
            "title": "School"
        },
        "StageGroup": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "classSubjects": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/ClassSubject"
                    }
                },
                "name": {
                    "type": "string"
                },
                "stage": {
                    "type": "integer"
                },
                "isActive": {
                    "type": "boolean"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "classSubjects",
                "isActive",
                "name",
                "stage"
            ],
            "title": "StageGroup"
        },
        "ClassSubject": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "stage": {
                    "$ref": "#/definitions/Stage"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "stage"
            ],
            "title": "ClassSubject"
        },
        "Stage": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "name": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "name"
            ],
            "title": "Stage"
        }
    }
}

```

</details>

[[Index](#index)]

### getUsers

<details>
<summary> Query </summary>

```
query getUsers($userIds: [UUID!]!) {
  school21 {
    getUsers(userIds: $userIds) {
      userId
      login
      firstName
      middleName
      lastName
      avatarUrl
      level
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "userIds": {
                    "type": "array",
                    "items": {
                        "type": "string",
                        "format": "uuid"
                    }
                }
            },
            "required": [
                "userIds"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "school21": {
                    "$ref": "#/definitions/School21"
                }
            },
            "required": [
                "school21"
            ],
            "title": "Data"
        },
        "School21": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getUsers": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/GetUser"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getUsers"
            ],
            "title": "School21"
        },
        "GetUser": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "userId": {
                    "type": "string",
                    "format": "uuid"
                },
                "login": {
                    "type": "string"
                },
                "firstName": {
                    "type": "string"
                },
                "middleName": {
                    "type": "null"
                },
                "lastName": {
                    "type": "string"
                },
                "avatarUrl": {
                    "type": "string"
                },
                "level": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "avatarUrl",
                "firstName",
                "lastName",
                "level",
                "login",
                "middleName",
                "userId"
            ],
            "title": "GetUser"
        }
    }
}

```

</details>

[[Index](#index)]

### getMySuggestedActivities

<details>
<summary> Query </summary>

```
query getMySuggestedActivities($page: PagingInput!, $statuses: [ParticipantEventStatus]) {
  school21 {
    getMySuggestedActivities(page: $page, statuses: $statuses) {
      id
      start
      end
      eventType
      description
      eventCode
      activity {
        organizers {
          id
          login
          __typename
        }
        eventCreator {
          id
          login
          __typename
        }
        comments {
          type
          createTs
          comment
          __typename
        }
        averageFeedbackRating
        isVisible
        activityType
        status
        activityEventId
        eventId
        name
        description
        location
        currentStudentsCount
        maxStudentCount
        isRegistered
        isInWaitList
        isWaitListActive
        stopRegisterDate
        beginDate
        endDate
        __typename
      }
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "page": {
                    "$ref": "#/definitions/Page"
                }
            },
            "required": [
                "page"
            ],
            "title": "Variables"
        },
        "Page": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "offset": {
                    "type": "integer"
                },
                "limit": {
                    "type": "integer"
                }
            },
            "required": [
                "limit",
                "offset"
            ],
            "title": "Page"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "school21": {
                    "$ref": "#/definitions/School21"
                }
            },
            "required": [
                "school21"
            ],
            "title": "Data"
        },
        "School21": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getMySuggestedActivities": {
                    "type": "array",
                    "items": {}
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getMySuggestedActivities"
            ],
            "title": "School21"
        }
    }
}

```

</details>

[[Index](#index)]

### subscribeToEvent

<details>
<summary> Query </summary>

```
mutation subscribeToEvent($eventId: ID!) {
  student {
    subscribeToEvent(eventId: $eventId) {
      ...UpcomingEvent
      __typename
    }
    __typename
  }
}

fragment UpcomingEvent on CalendarEvent {
  id
  start
  end
  bookings {
    id
    task {
      id
      goalName
      __typename
    }
    __typename
  }
  eventSlots {
    id
    eventId
    type
    start
    end
    __typename
  }
  maxStudentCount
  location
  ipRange
  eventType
  eventCode
  description
  externalId
  currentStudentsCount
  exam {
    examId
    eventId
    beginDate
    endDate
    location
    ip
    maxStudentCount
    isVisible
    name
    goalId
    isWaitListActive
    isInWaitList
    currentStudentsCount
    createDate
    updateDate
    schoolId
    stopRegisterDate
    isRegistered
    goalName
    eventType
    registrationAccessStatus
    __typename
  }
  studentCodeReview {
    studentGoalId
    __typename
  }
  activity {
    activityEventId
    eventId
    beginDate
    endDate
    location
    description
    maxStudentCount
    isVisible
    name
    isWaitListActive
    isInWaitList
    currentStudentsCount
    createDate
    updateDate
    schoolId
    stopRegisterDate
    isRegistered
    activityType
    eventType
    isMandatory
    status
    organizers {
      id
      login
      __typename
    }
    __typename
  }
  penalty {
    ...Penalty
    __typename
  }
  __typename
}

fragment Penalty on Penalty {
  comment
  id
  duration
  status
  startTime
  createTime
  penaltySlot {
    currentStudentsCount
    description
    duration
    startTime
    id
    endTime
    __typename
  }
  reasonId
  __typename
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "eventId": {
                    "type": "string",
                    "format": "integer"
                }
            },
            "required": [
                "eventId"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "subscribeToEvent": {
                    "$ref": "#/definitions/SubscribeToEvent"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "subscribeToEvent"
            ],
            "title": "Student"
        },
        "SubscribeToEvent": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "start": {
                    "type": "string",
                    "format": "date-time"
                },
                "end": {
                    "type": "string",
                    "format": "date-time"
                },
                "bookings": {
                    "type": "array",
                    "items": {}
                },
                "eventSlots": {
                    "type": "array",
                    "items": {}
                },
                "maxStudentCount": {
                    "type": "integer"
                },
                "location": {
                    "type": "string"
                },
                "ipRange": {
                    "type": "string"
                },
                "eventType": {
                    "type": "string"
                },
                "eventCode": {
                    "type": "string"
                },
                "description": {
                    "type": "string"
                },
                "externalId": {
                    "type": "integer"
                },
                "currentStudentsCount": {
                    "type": "integer"
                },
                "exam": {
                    "type": "null"
                },
                "studentCodeReview": {
                    "type": "null"
                },
                "activity": {
                    "$ref": "#/definitions/Activity"
                },
                "penalty": {
                    "type": "null"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "activity",
                "bookings",
                "currentStudentsCount",
                "description",
                "end",
                "eventCode",
                "eventSlots",
                "eventType",
                "exam",
                "externalId",
                "id",
                "ipRange",
                "location",
                "maxStudentCount",
                "penalty",
                "start",
                "studentCodeReview"
            ],
            "title": "SubscribeToEvent"
        },
        "Activity": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "activityEventId": {
                    "type": "string",
                    "format": "integer"
                },
                "eventId": {
                    "type": "string",
                    "format": "integer"
                },
                "beginDate": {
                    "type": "string",
                    "format": "date-time"
                },
                "endDate": {
                    "type": "string",
                    "format": "date-time"
                },
                "location": {
                    "type": "string"
                },
                "description": {
                    "type": "string"
                },
                "maxStudentCount": {
                    "type": "integer"
                },
                "isVisible": {
                    "type": "boolean"
                },
                "name": {
                    "type": "string"
                },
                "isWaitListActive": {
                    "type": "boolean"
                },
                "isInWaitList": {
                    "type": "boolean"
                },
                "currentStudentsCount": {
                    "type": "integer"
                },
                "createDate": {
                    "type": "string",
                    "format": "date-time"
                },
                "updateDate": {
                    "type": "string",
                    "format": "date-time"
                },
                "schoolId": {
                    "type": "string",
                    "format": "uuid"
                },
                "stopRegisterDate": {
                    "type": "string",
                    "format": "date-time"
                },
                "isRegistered": {
                    "type": "boolean"
                },
                "activityType": {
                    "type": "string"
                },
                "eventType": {
                    "type": "string"
                },
                "isMandatory": {
                    "type": "boolean"
                },
                "status": {
                    "type": "string"
                },
                "organizers": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/Organizer"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "activityEventId",
                "activityType",
                "beginDate",
                "createDate",
                "currentStudentsCount",
                "description",
                "endDate",
                "eventId",
                "eventType",
                "isInWaitList",
                "isMandatory",
                "isRegistered",
                "isVisible",
                "isWaitListActive",
                "location",
                "maxStudentCount",
                "name",
                "organizers",
                "schoolId",
                "status",
                "stopRegisterDate",
                "updateDate"
            ],
            "title": "Activity"
        },
        "Organizer": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "login": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "login"
            ],
            "title": "Organizer"
        }
    }
}

```

</details>

[[Index](#index)]

### unsubscribeFromEvent

<details>
<summary> Query </summary>

```
mutation unsubscribeFromEvent($eventId: ID!) {
  student {
    unsubscribeFromEvent(eventId: $eventId) {
      ...UpcomingEvent
      __typename
    }
    __typename
  }
}

fragment UpcomingEvent on CalendarEvent {
  id
  start
  end
  bookings {
    id
    task {
      id
      goalName
      __typename
    }
    __typename
  }
  eventSlots {
    id
    eventId
    type
    start
    end
    __typename
  }
  maxStudentCount
  location
  ipRange
  eventType
  eventCode
  description
  externalId
  currentStudentsCount
  exam {
    examId
    eventId
    beginDate
    endDate
    location
    ip
    maxStudentCount
    isVisible
    name
    goalId
    isWaitListActive
    isInWaitList
    currentStudentsCount
    createDate
    updateDate
    schoolId
    stopRegisterDate
    isRegistered
    goalName
    eventType
    registrationAccessStatus
    __typename
  }
  studentCodeReview {
    studentGoalId
    __typename
  }
  activity {
    activityEventId
    eventId
    beginDate
    endDate
    location
    description
    maxStudentCount
    isVisible
    name
    isWaitListActive
    isInWaitList
    currentStudentsCount
    createDate
    updateDate
    schoolId
    stopRegisterDate
    isRegistered
    activityType
    eventType
    isMandatory
    status
    organizers {
      id
      login
      __typename
    }
    __typename
  }
  penalty {
    ...Penalty
    __typename
  }
  __typename
}

fragment Penalty on Penalty {
  comment
  id
  duration
  status
  startTime
  createTime
  penaltySlot {
    currentStudentsCount
    description
    duration
    startTime
    id
    endTime
    __typename
  }
  reasonId
  __typename
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "eventId": {
                    "type": "string",
                    "format": "integer"
                }
            },
            "required": [
                "eventId"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "unsubscribeFromEvent": {
                    "$ref": "#/definitions/UnsubscribeFromEvent"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "unsubscribeFromEvent"
            ],
            "title": "Student"
        },
        "UnsubscribeFromEvent": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "start": {
                    "type": "string",
                    "format": "date-time"
                },
                "end": {
                    "type": "string",
                    "format": "date-time"
                },
                "bookings": {
                    "type": "array",
                    "items": {}
                },
                "eventSlots": {
                    "type": "array",
                    "items": {}
                },
                "maxStudentCount": {
                    "type": "integer"
                },
                "location": {
                    "type": "string"
                },
                "ipRange": {
                    "type": "string"
                },
                "eventType": {
                    "type": "string"
                },
                "eventCode": {
                    "type": "string"
                },
                "description": {
                    "type": "string"
                },
                "externalId": {
                    "type": "integer"
                },
                "currentStudentsCount": {
                    "type": "integer"
                },
                "exam": {
                    "type": "null"
                },
                "studentCodeReview": {
                    "type": "null"
                },
                "activity": {
                    "$ref": "#/definitions/Activity"
                },
                "penalty": {
                    "type": "null"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "activity",
                "bookings",
                "currentStudentsCount",
                "description",
                "end",
                "eventCode",
                "eventSlots",
                "eventType",
                "exam",
                "externalId",
                "id",
                "ipRange",
                "location",
                "maxStudentCount",
                "penalty",
                "start",
                "studentCodeReview"
            ],
            "title": "UnsubscribeFromEvent"
        },
        "Activity": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "activityEventId": {
                    "type": "string",
                    "format": "integer"
                },
                "eventId": {
                    "type": "string",
                    "format": "integer"
                },
                "beginDate": {
                    "type": "string",
                    "format": "date-time"
                },
                "endDate": {
                    "type": "string",
                    "format": "date-time"
                },
                "location": {
                    "type": "string"
                },
                "description": {
                    "type": "string"
                },
                "maxStudentCount": {
                    "type": "integer"
                },
                "isVisible": {
                    "type": "boolean"
                },
                "name": {
                    "type": "string"
                },
                "isWaitListActive": {
                    "type": "boolean"
                },
                "isInWaitList": {
                    "type": "boolean"
                },
                "currentStudentsCount": {
                    "type": "integer"
                },
                "createDate": {
                    "type": "string",
                    "format": "date-time"
                },
                "updateDate": {
                    "type": "string",
                    "format": "date-time"
                },
                "schoolId": {
                    "type": "string",
                    "format": "uuid"
                },
                "stopRegisterDate": {
                    "type": "string",
                    "format": "date-time"
                },
                "isRegistered": {
                    "type": "boolean"
                },
                "activityType": {
                    "type": "string"
                },
                "eventType": {
                    "type": "string"
                },
                "isMandatory": {
                    "type": "boolean"
                },
                "status": {
                    "type": "string"
                },
                "organizers": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/Organizer"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "activityEventId",
                "activityType",
                "beginDate",
                "createDate",
                "currentStudentsCount",
                "description",
                "endDate",
                "eventId",
                "eventType",
                "isInWaitList",
                "isMandatory",
                "isRegistered",
                "isVisible",
                "isWaitListActive",
                "location",
                "maxStudentCount",
                "name",
                "organizers",
                "schoolId",
                "status",
                "stopRegisterDate",
                "updateDate"
            ],
            "title": "Activity"
        },
        "Organizer": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "login": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "login"
            ],
            "title": "Organizer"
        }
    }
}

```

</details>

[[Index](#index)]

### publicProfileGetProjects

<details>
<summary> Query </summary>

```
query publicProfileGetProjects($studentId: UUID!, $stageGroupId: ID!) {
  school21 {
    getStudentProjectsForPublicProfileByStageGroup(
      studentId: $studentId
      stageGroupId: $stageGroupId
    ) {
      groupName
      name
      experience
      finalPercentage
      goalId
      goalStatus
      amountAnswers
      amountReviewedAnswers
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "studentId": {
                    "type": "string",
                    "format": "uuid"
                },
                "stageGroupId": {
                    "type": "string",
                    "format": "integer"
                }
            },
            "required": [
                "stageGroupId",
                "studentId"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "school21": {
                    "$ref": "#/definitions/School21"
                }
            },
            "required": [
                "school21"
            ],
            "title": "Data"
        },
        "School21": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getStudentProjectsForPublicProfileByStageGroup": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/GetStudentProjectsForPublicProfileByStageGroup"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getStudentProjectsForPublicProfileByStageGroup"
            ],
            "title": "School21"
        },
        "GetStudentProjectsForPublicProfileByStageGroup": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "groupName": {
                    "type": "string"
                },
                "name": {
                    "type": "string"
                },
                "experience": {
                    "type": "integer"
                },
                "finalPercentage": {
                    "anyOf": [
                        {
                            "type": "integer"
                        },
                        {
                            "type": "null"
                        }
                    ]
                },
                "goalId": {
                    "type": "integer"
                },
                "goalStatus": {
                    "type": "string"
                },
                "amountAnswers": {
                    "type": "null"
                },
                "amountReviewedAnswers": {
                    "type": "null"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "amountAnswers",
                "amountReviewedAnswers",
                "experience",
                "finalPercentage",
                "goalId",
                "goalStatus",
                "groupName",
                "name"
            ],
            "title": "GetStudentProjectsForPublicProfileByStageGroup"
        }
    }
}

```

</details>

[[Index](#index)]

### publicProfileGetCredentialsByLogin

<details>
<summary> Query </summary>

```
query publicProfileGetCredentialsByLogin($login: String!) {
  school21 {
    getStudentByLogin(login: $login) {
      studentId
      userId
      schoolId
      isActive
      isGraduate
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "login": {
                    "type": "string"
                }
            },
            "required": [
                "login"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "school21": {
                    "$ref": "#/definitions/School21"
                }
            },
            "required": [
                "school21"
            ],
            "title": "Data"
        },
        "School21": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getStudentByLogin": {
                    "$ref": "#/definitions/GetStudentByLogin"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getStudentByLogin"
            ],
            "title": "School21"
        },
        "GetStudentByLogin": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "studentId": {
                    "type": "string",
                    "format": "uuid"
                },
                "userId": {
                    "type": "string",
                    "format": "uuid"
                },
                "schoolId": {
                    "type": "string",
                    "format": "uuid"
                },
                "isActive": {
                    "type": "boolean"
                },
                "isGraduate": {
                    "type": "boolean"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "isActive",
                "isGraduate",
                "schoolId",
                "studentId",
                "userId"
            ],
            "title": "GetStudentByLogin"
        }
    }
}

```

</details>

[[Index](#index)]

### bonusesGetUserIdByLogin

<details>
<summary> Query </summary>

```
query bonusesGetUserIdByLogin($login: String!) {
  student {
    getUserIdByLogin(login: $login)
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "login": {
                    "type": "string"
                }
            },
            "required": [
                "login"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getUserIdByLogin": {
                    "type": "string",
                    "format": "uuid"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getUserIdByLogin"
            ],
            "title": "Student"
        }
    }
}

```

</details>

[[Index](#index)]

### competitionCoalitionGetUserTournament

<details>
<summary> Query </summary>

```
query competitionCoalitionGetUserTournament {
  student {
    getUserTournamentWidget {
      coalitionMember {
        coalition {
          ...CompetitionCurrentCoalition
          __typename
        }
        __typename
      }
      lastTournamentResult {
        id
        __typename
      }
      __typename
    }
    __typename
  }
}

fragment CompetitionCurrentCoalition on GameCoalition {
  id
  name
  avatarUrl
  backgroundUrl
  backgroundUrlBig
  memberCount
  color
  currentTournament {
    points
    tournament {
      name
      timeStart
      timeEnd
      __typename
    }
    __typename
  }
  masterUser {
    login
    avatarUrl
    __typename
  }
  __typename
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getUserTournamentWidget": {
                    "$ref": "#/definitions/GetUserTournamentWidget"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getUserTournamentWidget"
            ],
            "title": "Student"
        },
        "GetUserTournamentWidget": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "coalitionMember": {
                    "$ref": "#/definitions/CoalitionMember"
                },
                "lastTournamentResult": {
                    "$ref": "#/definitions/LastTournamentResult"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "coalitionMember",
                "lastTournamentResult"
            ],
            "title": "GetUserTournamentWidget"
        },
        "CoalitionMember": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "coalition": {
                    "$ref": "#/definitions/Coalition"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "coalition"
            ],
            "title": "CoalitionMember"
        },
        "Coalition": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "name": {
                    "type": "string"
                },
                "avatarUrl": {
                    "type": "string"
                },
                "backgroundUrl": {
                    "type": "string"
                },
                "backgroundUrlBig": {
                    "type": "string"
                },
                "memberCount": {
                    "type": "integer"
                },
                "color": {
                    "type": "string"
                },
                "currentTournament": {
                    "$ref": "#/definitions/CurrentTournament"
                },
                "masterUser": {
                    "$ref": "#/definitions/MasterUser"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "avatarUrl",
                "backgroundUrl",
                "backgroundUrlBig",
                "color",
                "currentTournament",
                "id",
                "masterUser",
                "memberCount",
                "name"
            ],
            "title": "Coalition"
        },
        "CurrentTournament": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "points": {
                    "type": "integer"
                },
                "tournament": {
                    "$ref": "#/definitions/Tournament"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "points",
                "tournament"
            ],
            "title": "CurrentTournament"
        },
        "Tournament": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "name": {
                    "type": "string"
                },
                "timeStart": {
                    "type": "string",
                    "format": "date-time"
                },
                "timeEnd": {
                    "type": "string",
                    "format": "date-time"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "name",
                "timeEnd",
                "timeStart"
            ],
            "title": "Tournament"
        },
        "MasterUser": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "login": {
                    "type": "string"
                },
                "avatarUrl": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "avatarUrl",
                "login"
            ],
            "title": "MasterUser"
        },
        "LastTournamentResult": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id"
            ],
            "title": "LastTournamentResult"
        }
    }
}

```

</details>

[[Index](#index)]

### competitionCoalitionGetMyCoalitionMembers

<details>
<summary> Query </summary>

```
query competitionCoalitionGetMyCoalitionMembers($page: PagingInput) {
  student {
    getUserTournamentWidget {
      getMyCoalitionMembers(page: $page) {
        user {
          id
          login
          avatarUrl
          userExperience {
            level {
              id
              levelCode
              __typename
            }
            __typename
          }
          __typename
        }
        __typename
      }
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "page": {
                    "$ref": "#/definitions/Page"
                }
            },
            "required": [
                "page"
            ],
            "title": "Variables"
        },
        "Page": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "offset": {
                    "type": "integer"
                },
                "limit": {
                    "type": "integer"
                }
            },
            "required": [
                "limit",
                "offset"
            ],
            "title": "Page"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getUserTournamentWidget": {
                    "$ref": "#/definitions/GetUserTournamentWidget"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getUserTournamentWidget"
            ],
            "title": "Student"
        },
        "GetUserTournamentWidget": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getMyCoalitionMembers": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/GetMyCoalitionMember"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getMyCoalitionMembers"
            ],
            "title": "GetUserTournamentWidget"
        },
        "GetMyCoalitionMember": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "user": {
                    "$ref": "#/definitions/User"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "user"
            ],
            "title": "GetMyCoalitionMember"
        },
        "User": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "login": {
                    "type": "string"
                },
                "avatarUrl": {
                    "type": "string"
                },
                "userExperience": {
                    "$ref": "#/definitions/UserExperience"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "avatarUrl",
                "id",
                "login",
                "userExperience"
            ],
            "title": "User"
        },
        "UserExperience": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "level": {
                    "$ref": "#/definitions/Level"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "level"
            ],
            "title": "UserExperience"
        },
        "Level": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "integer"
                },
                "levelCode": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "levelCode"
            ],
            "title": "Level"
        }
    }
}

```

</details>

[[Index](#index)]

### getPenaltyList

<details>
<summary> Query </summary>

```
query getPenaltyList($statuses: [String]!, $from: DateTime, $to: DateTime, $sorting: SortingField, $page: PagingInput!) {
  school21 {
    getMyPenalties(
      statuses: $statuses
      from: $from
      to: $to
      sorting: $sorting
      page: $page
    ) {
      ...Penalty
      __typename
    }
    getPenaltyReasons {
      id
      name
      __typename
    }
    countMyPenalties(statuses: $statuses)
    __typename
  }
}

fragment Penalty on Penalty {
  comment
  id
  duration
  status
  startTime
  createTime
  penaltySlot {
    currentStudentsCount
    description
    duration
    startTime
    id
    endTime
    __typename
  }
  reasonId
  __typename
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "page": {
                    "$ref": "#/definitions/Page"
                },
                "statuses": {
                    "type": "array",
                    "items": {
                        "type": "string"
                    }
                }
            },
            "required": [
                "page",
                "statuses"
            ],
            "title": "Variables"
        },
        "Page": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "offset": {
                    "type": "integer"
                },
                "limit": {
                    "type": "integer"
                }
            },
            "required": [
                "limit",
                "offset"
            ],
            "title": "Page"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "school21": {
                    "$ref": "#/definitions/School21"
                }
            },
            "required": [
                "school21"
            ],
            "title": "Data"
        },
        "School21": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getMyPenalties": {
                    "type": "array",
                    "items": {}
                },
                "getPenaltyReasons": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/GetPenaltyReason"
                    }
                },
                "countMyPenalties": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "countMyPenalties",
                "getMyPenalties",
                "getPenaltyReasons"
            ],
            "title": "School21"
        },
        "GetPenaltyReason": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "name": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "name"
            ],
            "title": "GetPenaltyReason"
        }
    }
}

```

</details>

[[Index](#index)]

### getPenaltiesCount

<details>
<summary> Query </summary>

```
query getPenaltiesCount($statuses: [String]!) {
  school21 {
    countMyPenalties(statuses: $statuses)
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "statuses": {
                    "type": "array",
                    "items": {
                        "type": "string"
                    }
                }
            },
            "required": [
                "statuses"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "school21": {
                    "$ref": "#/definitions/School21"
                }
            },
            "required": [
                "school21"
            ],
            "title": "Data"
        },
        "School21": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "countMyPenalties": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "countMyPenalties"
            ],
            "title": "School21"
        }
    }
}

```

</details>

[[Index](#index)]

### getGraphCurrentType

<details>
<summary> Query </summary>

```
query getGraphCurrentType($userId: ID!, $schoolId: ID!) {
  student {
    getStudentCurrentStageWithGraphType(userId: $userId, schoolId: $schoolId) {
      id
      graphType
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "userId": {
                    "type": "string",
                    "format": "uuid"
                },
                "schoolId": {
                    "type": "string",
                    "format": "uuid"
                }
            },
            "required": [
                "schoolId",
                "userId"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getStudentCurrentStageWithGraphType": {
                    "$ref": "#/definitions/GetStudentCurrentStageWithGraphType"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getStudentCurrentStageWithGraphType"
            ],
            "title": "Student"
        },
        "GetStudentCurrentStageWithGraphType": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "graphType": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "graphType",
                "id"
            ],
            "title": "GetStudentCurrentStageWithGraphType"
        }
    }
}

```

</details>

[[Index](#index)]

### getGraphBasisGoals

<details>
<summary> Query </summary>

```
query getGraphBasisGoals($studentId: UUID!) {
  student {
    getBasisGraph(studentId: $studentId) {
      isIntensiveGraphAvailable
      graphNodes {
        ...BasisGraphNode
        __typename
      }
      __typename
    }
    __typename
  }
}

fragment BasisGraphNode on GraphNode {
  graphNodeId
  nodeCode
  studyDirections {
    id
    name
    color
    textColor
    __typename
  }
  entityType
  entityId
  goal {
    goalExecutionType
    projectState
    projectName
    projectDescription
    projectPoints
    projectDate
    duration
    isMandatory
    __typename
  }
  course {
    courseType
    projectState
    projectName
    projectDescription
    projectPoints
    projectDate
    duration
    localCourseId
    __typename
  }
  parentNodeCodes
  __typename
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "studentId": {
                    "type": "string",
                    "format": "uuid"
                }
            },
            "required": [
                "studentId"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getBasisGraph": {
                    "$ref": "#/definitions/GetBasisGraph"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getBasisGraph"
            ],
            "title": "Student"
        },
        "GetBasisGraph": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "isIntensiveGraphAvailable": {
                    "type": "boolean"
                },
                "graphNodes": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/GraphNode"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "graphNodes",
                "isIntensiveGraphAvailable"
            ],
            "title": "GetBasisGraph"
        },
        "GraphNode": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "graphNodeId": {
                    "type": "string",
                    "format": "integer"
                },
                "nodeCode": {
                    "type": "string"
                },
                "studyDirections": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/StudyDirection"
                    }
                },
                "entityType": {
                    "type": "string"
                },
                "entityId": {
                    "type": "string",
                    "format": "integer"
                },
                "goal": {
                    "anyOf": [
                        {
                            "$ref": "#/definitions/Course"
                        },
                        {
                            "type": "null"
                        }
                    ]
                },
                "course": {
                    "anyOf": [
                        {
                            "$ref": "#/definitions/Course"
                        },
                        {
                            "type": "null"
                        }
                    ]
                },
                "parentNodeCodes": {
                    "type": "array",
                    "items": {
                        "type": "string"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "course",
                "entityId",
                "entityType",
                "goal",
                "graphNodeId",
                "nodeCode",
                "parentNodeCodes",
                "studyDirections"
            ],
            "title": "GraphNode"
        },
        "Course": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "courseType": {
                    "type": "string"
                },
                "projectState": {
                    "type": "string"
                },
                "projectName": {
                    "type": "string"
                },
                "projectDescription": {
                    "type": "string"
                },
                "projectPoints": {
                    "type": "integer"
                },
                "projectDate": {
                    "type": "null"
                },
                "duration": {
                    "type": "integer"
                },
                "localCourseId": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                },
                "goalExecutionType": {
                    "type": "string"
                },
                "isMandatory": {
                    "type": "boolean"
                }
            },
            "required": [
                "__typename",
                "duration",
                "projectDate",
                "projectDescription",
                "projectName",
                "projectPoints",
                "projectState"
            ],
            "title": "Course"
        },
        "StudyDirection": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "name": {
                    "type": "string"
                },
                "color": {
                    "type": "string"
                },
                "textColor": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "color",
                "id",
                "name",
                "textColor"
            ],
            "title": "StudyDirection"
        }
    }
}

```

</details>

[[Index](#index)]

### getTasks

<details>
<summary> Query </summary>

```
query getTasks($ids: [ID!]!) {
  student {
    getTasksByIds(ids: $ids) {
      ...StudentTaskInProject
      __typename
    }
    __typename
  }
}

fragment StudentTaskInProject on StudentTask {
  id
  task {
    id
    content {
      id
      body
      __typename
    }
    __typename
  }
  __typename
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "ids": {
                    "type": "array",
                    "items": {
                        "type": "string",
                        "format": "integer"
                    }
                }
            },
            "required": [
                "ids"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getTasksByIds": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/GetTasksByID"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getTasksByIds"
            ],
            "title": "Student"
        },
        "GetTasksByID": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "task": {
                    "$ref": "#/definitions/Task"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "task"
            ],
            "title": "GetTasksByID"
        },
        "Task": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "content": {
                    "$ref": "#/definitions/Content"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "content",
                "id"
            ],
            "title": "Task"
        },
        "Content": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string"
                },
                "body": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "body",
                "id"
            ],
            "title": "Content"
        }
    }
}

```

</details>

[[Index](#index)]

### getGitlabLink

<details>
<summary> Query </summary>

```
query getGitlabLink($taskId: ID!) {
  student {
    getLinkToPrivateStudentGitlabProjectByTaskId(taskId: $taskId) {
      sshLink
      hasOpenedMR
      httpsLink
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "taskId": {
                    "type": "string",
                    "format": "integer"
                }
            },
            "required": [
                "taskId"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getLinkToPrivateStudentGitlabProjectByTaskId": {
                    "$ref": "#/definitions/GetLinkToPrivateStudentGitlabProjectByTaskID"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getLinkToPrivateStudentGitlabProjectByTaskId"
            ],
            "title": "Student"
        },
        "GetLinkToPrivateStudentGitlabProjectByTaskID": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "sshLink": {
                    "type": "string"
                },
                "hasOpenedMR": {
                    "type": "boolean"
                },
                "httpsLink": {
                    "type": "string",
                    "format": "uri",
                    "qt-uri-protocols": [
                        "https"
                    ],
                    "qt-uri-extensions": [
                        ".git"
                    ]
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "hasOpenedMR",
                "httpsLink",
                "sshLink"
            ],
            "title": "GetLinkToPrivateStudentGitlabProjectByTaskID"
        }
    }
}

```

</details>

[[Index](#index)]

### createFeedbackOnEvaluation

<details>
<summary> Query </summary>

```
mutation createFeedbackOnEvaluation($reviewFeedbackInput: ReviewFeedbackInput!) {
  student {
    createReviewFeedback(reviewFeedbackInput: $reviewFeedbackInput) {
      ...EvaluationFeedback
      __typename
    }
    __typename
  }
}

fragment EvaluationFeedback on ReviewFeedback {
  id
  comment
  filledChecklist {
    id
    __typename
  }
  reviewFeedbackCategoryValues {
    feedbackCategory
    feedbackValue
    id
    __typename
  }
  __typename
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "reviewFeedbackInput": {
                    "$ref": "#/definitions/ReviewFeedbackInput"
                }
            },
            "required": [
                "reviewFeedbackInput"
            ],
            "title": "Variables"
        },
        "ReviewFeedbackInput": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "filledChecklistId": {
                    "type": "string",
                    "format": "integer"
                },
                "comment": {
                    "type": "string"
                },
                "reviewFeedbackCategoryValues": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/ReviewFeedbackCategoryValue"
                    }
                }
            },
            "required": [
                "comment",
                "filledChecklistId",
                "reviewFeedbackCategoryValues"
            ],
            "title": "ReviewFeedbackInput"
        },
        "ReviewFeedbackCategoryValue": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "feedbackCategory": {
                    "type": "string"
                },
                "feedbackCategoryValue": {
                    "type": "string"
                }
            },
            "required": [
                "feedbackCategory",
                "feedbackCategoryValue"
            ],
            "title": "ReviewFeedbackCategoryValue"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "createReviewFeedback": {
                    "$ref": "#/definitions/CreateReviewFeedback"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "createReviewFeedback"
            ],
            "title": "Student"
        },
        "CreateReviewFeedback": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "comment": {
                    "type": "string"
                },
                "filledChecklist": {
                    "$ref": "#/definitions/FilledChecklist"
                },
                "reviewFeedbackCategoryValues": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/ReviewFeedbackCategoryValue"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "comment",
                "filledChecklist",
                "id",
                "reviewFeedbackCategoryValues"
            ],
            "title": "CreateReviewFeedback"
        },
        "FilledChecklist": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id"
            ],
            "title": "FilledChecklist"
        },
        "ReviewFeedbackCategoryValue": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "feedbackCategory": {
                    "type": "string"
                },
                "feedbackValue": {
                    "type": "string"
                },
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "feedbackCategory",
                "feedbackValue",
                "id"
            ],
            "title": "ReviewFeedbackCategoryValue"
        }
    }
}

```

</details>

[[Index](#index)]

### getProjectTeamWithMembers

<details>
<summary> Query </summary>

```
query getProjectTeamWithMembers($goalId: ID!) {
  student {
    getProjectTeamWithMembers(goalId: $goalId) {
      ...TeamWithMembers
      __typename
    }
    __typename
  }
}

fragment TeamWithMembers on ProjectTeamWithMembers {
  teamWithMembers {
    team {
      id
      name
      status
      minTeamMemberCount
      maxTeamMemberCount
      __typename
    }
    members {
      ...TeamMemberWithRole
      __typename
    }
    __typename
  }
  invitedStudents {
    student {
      user {
        ...ProjectTeamMember
        __typename
      }
      __typename
    }
    __typename
  }
  __typename
}

fragment TeamMemberWithRole on TeamMember {
  role
  user {
    ...ProjectTeamMember
    __typename
  }
  __typename
}

fragment ProjectTeamMember on User {
  id
  avatarUrl
  login
  userExperience {
    level {
      id
      range {
        levelCode
        __typename
      }
      __typename
    }
    cookiesCount
    codeReviewPoints
    __typename
  }
  __typename
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "goalId": {
                    "type": "string",
                    "format": "integer"
                }
            },
            "required": [
                "goalId"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/DataStudent"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "DataStudent": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getProjectTeamWithMembers": {
                    "$ref": "#/definitions/GetProjectTeamWithMembers"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getProjectTeamWithMembers"
            ],
            "title": "DataStudent"
        },
        "GetProjectTeamWithMembers": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "teamWithMembers": {
                    "$ref": "#/definitions/TeamWithMembers"
                },
                "invitedStudents": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/InvitedStudent"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "invitedStudents",
                "teamWithMembers"
            ],
            "title": "GetProjectTeamWithMembers"
        },
        "InvitedStudent": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/InvitedStudentStudent"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "student"
            ],
            "title": "InvitedStudent"
        },
        "InvitedStudentStudent": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "user": {
                    "$ref": "#/definitions/User"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "user"
            ],
            "title": "InvitedStudentStudent"
        },
        "User": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "avatarUrl": {
                    "type": "string"
                },
                "login": {
                    "type": "string"
                },
                "userExperience": {
                    "$ref": "#/definitions/UserExperience"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "avatarUrl",
                "id",
                "login",
                "userExperience"
            ],
            "title": "User"
        },
        "UserExperience": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "level": {
                    "$ref": "#/definitions/Level"
                },
                "cookiesCount": {
                    "type": "integer"
                },
                "codeReviewPoints": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "codeReviewPoints",
                "cookiesCount",
                "level"
            ],
            "title": "UserExperience"
        },
        "Level": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "integer"
                },
                "range": {
                    "$ref": "#/definitions/Range"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "range"
            ],
            "title": "Level"
        },
        "Range": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "levelCode": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "levelCode"
            ],
            "title": "Range"
        },
        "TeamWithMembers": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "team": {
                    "$ref": "#/definitions/Team"
                },
                "members": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/Member"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "members",
                "team"
            ],
            "title": "TeamWithMembers"
        },
        "Member": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "role": {
                    "type": "string"
                },
                "user": {
                    "$ref": "#/definitions/User"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "role",
                "user"
            ],
            "title": "Member"
        },
        "Team": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "name": {
                    "type": "string"
                },
                "status": {
                    "type": "string"
                },
                "minTeamMemberCount": {
                    "type": "integer"
                },
                "maxTeamMemberCount": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "maxTeamMemberCount",
                "minTeamMemberCount",
                "name",
                "status"
            ],
            "title": "Team"
        }
    }
}

```

</details>

[[Index](#index)]

### getIsDisbandRequestAlreadySent

<details>
<summary> Query </summary>

```
query getIsDisbandRequestAlreadySent($teamId: UUID!) {
  student {
    isRequestBeenSentToTeamDisband(teamId: $teamId)
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "teamId": {
                    "type": "string",
                    "format": "uuid"
                }
            },
            "required": [
                "teamId"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "isRequestBeenSentToTeamDisband": {
                    "type": "boolean"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "isRequestBeenSentToTeamDisband"
            ],
            "title": "Student"
        }
    }
}

```

</details>

[[Index](#index)]

### getGitlabSettingsToken

<details>
<summary> Query </summary>

```
query getGitlabSettingsToken($taskId: ID!) {
  student {
    getLinkToPrivateStudentGitlabProjectByTaskId(taskId: $taskId) {
      runnersToken
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "taskId": {
                    "type": "string",
                    "format": "integer"
                }
            },
            "required": [
                "taskId"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "type": "null"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        }
    }
}

```

</details>

[[Index](#index)]

### cancelInvitation

<details>
<summary> Query </summary>

```
mutation cancelInvitation($teamId: UUID!, $userId: ID!) {
  student {
    cancelInvitation(teamId: $teamId, userId: $userId) {
      ...StudentInvitationInfo
      __typename
    }
    __typename
  }
}

fragment StudentInvitationInfo on StudentInvitationInfo {
  student {
    ...AvailableStudentForTeam
    __typename
  }
  invitationStatus
  __typename
}

fragment AvailableStudentForTeam on Student {
  id
  user {
    id
    login
    avatarUrl
    userExperience {
      ...CurrentUserExperience
      __typename
    }
    __typename
  }
  __typename
}

fragment CurrentUserExperience on UserExperience {
  id
  cookiesCount
  codeReviewPoints
  coinsCount
  level {
    id
    range {
      id
      levelCode
      __typename
    }
    __typename
  }
  __typename
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "userId": {
                    "type": "string",
                    "format": "uuid"
                },
                "teamId": {
                    "type": "string",
                    "format": "uuid"
                }
            },
            "required": [
                "teamId",
                "userId"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/DataStudent"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "DataStudent": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "cancelInvitation": {
                    "$ref": "#/definitions/CancelInvitation"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "cancelInvitation"
            ],
            "title": "DataStudent"
        },
        "CancelInvitation": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/CancelInvitationStudent"
                },
                "invitationStatus": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "invitationStatus",
                "student"
            ],
            "title": "CancelInvitation"
        },
        "CancelInvitationStudent": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "user": {
                    "$ref": "#/definitions/User"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "user"
            ],
            "title": "CancelInvitationStudent"
        },
        "User": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "login": {
                    "type": "string"
                },
                "avatarUrl": {
                    "type": "string"
                },
                "userExperience": {
                    "$ref": "#/definitions/UserExperience"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "avatarUrl",
                "id",
                "login",
                "userExperience"
            ],
            "title": "User"
        },
        "UserExperience": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "cookiesCount": {
                    "type": "integer"
                },
                "codeReviewPoints": {
                    "type": "integer"
                },
                "coinsCount": {
                    "type": "integer"
                },
                "level": {
                    "$ref": "#/definitions/Level"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "codeReviewPoints",
                "coinsCount",
                "cookiesCount",
                "id",
                "level"
            ],
            "title": "UserExperience"
        },
        "Level": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "integer"
                },
                "range": {
                    "$ref": "#/definitions/Range"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "range"
            ],
            "title": "Level"
        },
        "Range": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "levelCode": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "levelCode"
            ],
            "title": "Range"
        }
    }
}

```

</details>

[[Index](#index)]

### getAvailableStudentsForTeams

<details>
<summary> Query </summary>

```
query getAvailableStudentsForTeams($goalId: ID!) {
  student {
    getAvailableStudentsForTeam(goalId: $goalId) {
      ...StudentInvitationInfo
      __typename
    }
    __typename
  }
}

fragment StudentInvitationInfo on StudentInvitationInfo {
  student {
    ...AvailableStudentForTeam
    __typename
  }
  invitationStatus
  __typename
}

fragment AvailableStudentForTeam on Student {
  id
  user {
    id
    login
    avatarUrl
    userExperience {
      ...CurrentUserExperience
      __typename
    }
    __typename
  }
  __typename
}

fragment CurrentUserExperience on UserExperience {
  id
  cookiesCount
  codeReviewPoints
  coinsCount
  level {
    id
    range {
      id
      levelCode
      __typename
    }
    __typename
  }
  __typename
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "goalId": {
                    "type": "string",
                    "format": "integer"
                }
            },
            "required": [
                "goalId"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/DataStudent"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "DataStudent": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getAvailableStudentsForTeam": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/GetAvailableStudentsForTeam"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getAvailableStudentsForTeam"
            ],
            "title": "DataStudent"
        },
        "GetAvailableStudentsForTeam": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/GetAvailableStudentsForTeamStudent"
                },
                "invitationStatus": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "invitationStatus",
                "student"
            ],
            "title": "GetAvailableStudentsForTeam"
        },
        "GetAvailableStudentsForTeamStudent": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "user": {
                    "$ref": "#/definitions/User"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "user"
            ],
            "title": "GetAvailableStudentsForTeamStudent"
        },
        "User": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "login": {
                    "type": "string"
                },
                "avatarUrl": {
                    "type": "string",
                    "qt-uri-protocols": [
                        "https"
                    ]
                },
                "userExperience": {
                    "$ref": "#/definitions/UserExperience"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "avatarUrl",
                "id",
                "login",
                "userExperience"
            ],
            "title": "User"
        },
        "UserExperience": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "cookiesCount": {
                    "type": "integer"
                },
                "codeReviewPoints": {
                    "type": "integer"
                },
                "coinsCount": {
                    "type": "integer"
                },
                "level": {
                    "$ref": "#/definitions/Level"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "codeReviewPoints",
                "coinsCount",
                "cookiesCount",
                "id",
                "level"
            ],
            "title": "UserExperience"
        },
        "Level": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "integer"
                },
                "range": {
                    "$ref": "#/definitions/Range"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "range"
            ],
            "title": "Level"
        },
        "Range": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "levelCode": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "levelCode"
            ],
            "title": "Range"
        }
    }
}

```

</details>

[[Index](#index)]

### sendInvitation

<details>
<summary> Query </summary>

```
mutation sendInvitation($teamId: UUID!, $userId: ID!) {
  student {
    sendInvitation(teamId: $teamId, userId: $userId) {
      ...StudentInvitationInfo
      __typename
    }
    __typename
  }
}

fragment StudentInvitationInfo on StudentInvitationInfo {
  student {
    ...AvailableStudentForTeam
    __typename
  }
  invitationStatus
  __typename
}

fragment AvailableStudentForTeam on Student {
  id
  user {
    id
    login
    avatarUrl
    userExperience {
      ...CurrentUserExperience
      __typename
    }
    __typename
  }
  __typename
}

fragment CurrentUserExperience on UserExperience {
  id
  cookiesCount
  codeReviewPoints
  coinsCount
  level {
    id
    range {
      id
      levelCode
      __typename
    }
    __typename
  }
  __typename
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "userId": {
                    "type": "string",
                    "format": "uuid"
                },
                "teamId": {
                    "type": "string",
                    "format": "uuid"
                }
            },
            "required": [
                "teamId",
                "userId"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/DataStudent"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "DataStudent": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "sendInvitation": {
                    "$ref": "#/definitions/SendInvitation"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "sendInvitation"
            ],
            "title": "DataStudent"
        },
        "SendInvitation": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/SendInvitationStudent"
                },
                "invitationStatus": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "invitationStatus",
                "student"
            ],
            "title": "SendInvitation"
        },
        "SendInvitationStudent": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "user": {
                    "$ref": "#/definitions/User"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "user"
            ],
            "title": "SendInvitationStudent"
        },
        "User": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "login": {
                    "type": "string"
                },
                "avatarUrl": {
                    "type": "string"
                },
                "userExperience": {
                    "$ref": "#/definitions/UserExperience"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "avatarUrl",
                "id",
                "login",
                "userExperience"
            ],
            "title": "User"
        },
        "UserExperience": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "cookiesCount": {
                    "type": "integer"
                },
                "codeReviewPoints": {
                    "type": "integer"
                },
                "coinsCount": {
                    "type": "integer"
                },
                "level": {
                    "$ref": "#/definitions/Level"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "codeReviewPoints",
                "coinsCount",
                "cookiesCount",
                "id",
                "level"
            ],
            "title": "UserExperience"
        },
        "Level": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "integer"
                },
                "range": {
                    "$ref": "#/definitions/Range"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "range"
            ],
            "title": "Level"
        },
        "Range": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "levelCode": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "levelCode"
            ],
            "title": "Range"
        }
    }
}

```

</details>

[[Index](#index)]

### removeP2P

<details>
<summary> Query </summary>

```
mutation removeP2P($bookingId: ID!) {
  student {
    removeBookingFromEventSlot(bookingId: $bookingId)
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "bookingId": {
                    "type": "string",
                    "format": "integer"
                }
            },
            "required": [
                "bookingId"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "removeBookingFromEventSlot": {
                    "type": "boolean"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "removeBookingFromEventSlot"
            ],
            "title": "Student"
        }
    }
}

```

</details>

[[Index](#index)]

### calendarGetExams

<details>
<summary> Query </summary>

```
query calendarGetExams($from: DateTime!, $to: DateTime!) {
  student {
    getExams(from: $from, to: $to) {
      ...CalendarExam
      __typename
    }
    __typename
  }
}

fragment CalendarExam on Exam {
  examId
  eventId
  beginDate
  endDate
  name
  location
  maxStudentCount
  currentStudentsCount
  updateDate
  goalId
  goalName
  isWaitListActive
  isInWaitList
  stopRegisterDate
  __typename
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "from": {
                    "type": "string",
                    "format": "date-time"
                },
                "to": {
                    "type": "string",
                    "format": "date-time"
                }
            },
            "required": [
                "from",
                "to"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "student": {
                    "$ref": "#/definitions/Student"
                }
            },
            "required": [
                "student"
            ],
            "title": "Data"
        },
        "Student": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getExams": {
                    "type": "array",
                    "items": {}
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getExams"
            ],
            "title": "Student"
        }
    }
}

```

</details>

[[Index](#index)]

### userGetTheme

<details>
<summary> Query </summary>

```
query userGetTheme($userId: UUID!) {
  user {
    getUserViewSettings(userId: $userId) {
      isDarkThemeEnabled
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "userId": {
                    "type": "string",
                    "format": "uuid"
                }
            },
            "required": [
                "userId"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "user": {
                    "$ref": "#/definitions/User"
                }
            },
            "required": [
                "user"
            ],
            "title": "Data"
        },
        "User": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getUserViewSettings": {
                    "$ref": "#/definitions/GetUserViewSettings"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getUserViewSettings"
            ],
            "title": "User"
        },
        "GetUserViewSettings": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "isDarkThemeEnabled": {
                    "type": "boolean"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "isDarkThemeEnabled"
            ],
            "title": "GetUserViewSettings"
        }
    }
}

```

</details>

[[Index](#index)]

### getAllInCompletedStudentFeedbackPopup

<details>
<summary> Query </summary>

```
query getAllInCompletedStudentFeedbackPopup {
  sc21StudentTaskCheck {
    getAllInCompletedStudentFeedbackPopup {
      studentFeedbackId
      goalName
      resultAttemptDate
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "sc21StudentTaskCheck": {
                    "$ref": "#/definitions/Sc21StudentTaskCheck"
                }
            },
            "required": [
                "sc21StudentTaskCheck"
            ],
            "title": "Data"
        },
        "Sc21StudentTaskCheck": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getAllInCompletedStudentFeedbackPopup": {
                    "type": "array",
                    "items": {}
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getAllInCompletedStudentFeedbackPopup"
            ],
            "title": "Sc21StudentTaskCheck"
        }
    }
}

```

</details>

[[Index](#index)]

### getIsHonorRatingNeeded

<details>
<summary> Query </summary>

```
query getIsHonorRatingNeeded {
  honorRating {
    isHonorRatingNeeded
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "honorRating": {
                    "$ref": "#/definitions/HonorRating"
                }
            },
            "required": [
                "honorRating"
            ],
            "title": "Data"
        },
        "HonorRating": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "isHonorRatingNeeded": {
                    "type": "boolean"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "isHonorRatingNeeded"
            ],
            "title": "HonorRating"
        }
    }
}

```

</details>

[[Index](#index)]

### getSearchHistory

<details>
<summary> Query </summary>

```
query getSearchHistory {
  globalSearch {
    getSearchHistoryTooltips {
      tooltipText
      tooltipCategory
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "globalSearch": {
                    "$ref": "#/definitions/GlobalSearch"
                }
            },
            "required": [
                "globalSearch"
            ],
            "title": "Data"
        },
        "GlobalSearch": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getSearchHistoryTooltips": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/GetSearchHistoryTooltip"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getSearchHistoryTooltips"
            ],
            "title": "GlobalSearch"
        },
        "GetSearchHistoryTooltip": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "tooltipText": {
                    "type": "string"
                },
                "tooltipCategory": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "tooltipCategory",
                "tooltipText"
            ],
            "title": "GetSearchHistoryTooltip"
        }
    }
}

```

</details>

[[Index](#index)]

### getUpcomingEvents

<details>
<summary> Query </summary>

```
query getUpcomingEvents($eventCodes: [String!]!, $registrationAccessStatusFilter: RegistartionStatusEnum, $page: PagingInput) {
  calendarEventS21 {
    getUpcomingEventsForRegistration(
      eventCodes: $eventCodes
      registrationAccessStatusFilter: $registrationAccessStatusFilter
      page: $page
    ) {
      ...UpcomingEvent
      __typename
    }
    __typename
  }
}

fragment UpcomingEvent on CalendarEvent {
  id
  start
  end
  bookings {
    id
    task {
      id
      goalName
      __typename
    }
    __typename
  }
  eventSlots {
    id
    eventId
    type
    start
    end
    __typename
  }
  maxStudentCount
  location
  ipRange
  eventType
  eventCode
  description
  externalId
  currentStudentsCount
  exam {
    examId
    eventId
    beginDate
    endDate
    location
    ip
    maxStudentCount
    isVisible
    name
    goalId
    isWaitListActive
    isInWaitList
    currentStudentsCount
    createDate
    updateDate
    schoolId
    stopRegisterDate
    isRegistered
    goalName
    eventType
    registrationAccessStatus
    __typename
  }
  studentCodeReview {
    studentGoalId
    __typename
  }
  activity {
    activityEventId
    eventId
    beginDate
    endDate
    location
    description
    maxStudentCount
    isVisible
    name
    isWaitListActive
    isInWaitList
    currentStudentsCount
    createDate
    updateDate
    schoolId
    stopRegisterDate
    isRegistered
    activityType
    eventType
    isMandatory
    status
    organizers {
      id
      login
      __typename
    }
    __typename
  }
  penalty {
    ...Penalty
    __typename
  }
  __typename
}

fragment Penalty on Penalty {
  comment
  id
  duration
  status
  startTime
  createTime
  penaltySlot {
    currentStudentsCount
    description
    duration
    startTime
    id
    endTime
    __typename
  }
  reasonId
  __typename
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "eventCodes": {
                    "type": "array",
                    "items": {
                        "type": "string"
                    }
                },
                "registrationAccessStatusFilter": {
                    "type": "string"
                },
                "page": {
                    "$ref": "#/definitions/Page"
                }
            },
            "required": [
                "eventCodes",
                "page",
                "registrationAccessStatusFilter"
            ],
            "title": "Variables"
        },
        "Page": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "limit": {
                    "type": "integer"
                },
                "offset": {
                    "type": "integer"
                }
            },
            "required": [
                "limit",
                "offset"
            ],
            "title": "Page"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "calendarEventS21": {
                    "$ref": "#/definitions/CalendarEventS21"
                }
            },
            "required": [
                "calendarEventS21"
            ],
            "title": "Data"
        },
        "CalendarEventS21": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getUpcomingEventsForRegistration": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/GetUpcomingEventsForRegistration"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getUpcomingEventsForRegistration"
            ],
            "title": "CalendarEventS21"
        },
        "GetUpcomingEventsForRegistration": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "start": {
                    "type": "string",
                    "format": "date-time"
                },
                "end": {
                    "type": "string",
                    "format": "date-time"
                },
                "bookings": {
                    "type": "array",
                    "items": {}
                },
                "eventSlots": {
                    "type": "array",
                    "items": {}
                },
                "maxStudentCount": {
                    "type": "integer"
                },
                "location": {
                    "type": "string"
                },
                "ipRange": {
                    "type": "string"
                },
                "eventType": {
                    "type": "string"
                },
                "eventCode": {
                    "type": "string"
                },
                "description": {
                    "type": "string"
                },
                "externalId": {
                    "type": "integer"
                },
                "currentStudentsCount": {
                    "type": "integer"
                },
                "exam": {
                    "type": "null"
                },
                "studentCodeReview": {
                    "type": "null"
                },
                "activity": {
                    "$ref": "#/definitions/Activity"
                },
                "penalty": {
                    "type": "null"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "activity",
                "bookings",
                "currentStudentsCount",
                "description",
                "end",
                "eventCode",
                "eventSlots",
                "eventType",
                "exam",
                "externalId",
                "id",
                "ipRange",
                "location",
                "maxStudentCount",
                "penalty",
                "start",
                "studentCodeReview"
            ],
            "title": "GetUpcomingEventsForRegistration"
        },
        "Activity": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "activityEventId": {
                    "type": "string",
                    "format": "integer"
                },
                "eventId": {
                    "type": "string",
                    "format": "integer"
                },
                "beginDate": {
                    "type": "string",
                    "format": "date-time"
                },
                "endDate": {
                    "type": "string",
                    "format": "date-time"
                },
                "location": {
                    "type": "string"
                },
                "description": {
                    "type": "string"
                },
                "maxStudentCount": {
                    "type": "integer"
                },
                "isVisible": {
                    "type": "boolean"
                },
                "name": {
                    "type": "string"
                },
                "isWaitListActive": {
                    "type": "boolean"
                },
                "isInWaitList": {
                    "type": "boolean"
                },
                "currentStudentsCount": {
                    "type": "integer"
                },
                "createDate": {
                    "type": "string",
                    "format": "date-time"
                },
                "updateDate": {
                    "type": "string",
                    "format": "date-time"
                },
                "schoolId": {
                    "type": "string",
                    "format": "uuid"
                },
                "stopRegisterDate": {
                    "type": "string",
                    "format": "date-time"
                },
                "isRegistered": {
                    "type": "boolean"
                },
                "activityType": {
                    "type": "string"
                },
                "eventType": {
                    "type": "string"
                },
                "isMandatory": {
                    "type": "boolean"
                },
                "status": {
                    "type": "string"
                },
                "organizers": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/Organizer"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "activityEventId",
                "activityType",
                "beginDate",
                "createDate",
                "currentStudentsCount",
                "description",
                "endDate",
                "eventId",
                "eventType",
                "isInWaitList",
                "isMandatory",
                "isRegistered",
                "isVisible",
                "isWaitListActive",
                "location",
                "maxStudentCount",
                "name",
                "organizers",
                "schoolId",
                "status",
                "stopRegisterDate",
                "updateDate"
            ],
            "title": "Activity"
        },
        "Organizer": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "login": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "login"
            ],
            "title": "Organizer"
        }
    }
}

```

</details>

[[Index](#index)]

### getAgendaEvents

<details>
<summary> Query </summary>

```
query getAgendaEvents($from: DateTime!, $to: DateTime!, $limit: Int!) {
  calendarEventS21 {
    getMyAgendaEvents(from: $from, to: $to, limit: $limit) {
      agendaItemContext {
        entityId
        entityType
        __typename
      }
      start
      end
      label
      description
      agendaEventType
      additionalInfo {
        key
        value
        __typename
      }
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "from": {
                    "type": "string",
                    "format": "date-time"
                },
                "to": {
                    "type": "string",
                    "format": "date-time"
                },
                "limit": {
                    "type": "integer"
                }
            },
            "required": [
                "from",
                "limit",
                "to"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "calendarEventS21": {
                    "$ref": "#/definitions/CalendarEventS21"
                }
            },
            "required": [
                "calendarEventS21"
            ],
            "title": "Data"
        },
        "CalendarEventS21": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getMyAgendaEvents": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/GetMyAgendaEvent"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getMyAgendaEvents"
            ],
            "title": "CalendarEventS21"
        },
        "GetMyAgendaEvent": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "agendaItemContext": {
                    "$ref": "#/definitions/AgendaItemContext"
                },
                "start": {
                    "type": "string",
                    "format": "date-time"
                },
                "end": {
                    "type": "string",
                    "format": "date-time"
                },
                "label": {
                    "type": "string"
                },
                "description": {
                    "type": "string"
                },
                "agendaEventType": {
                    "type": "string"
                },
                "additionalInfo": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/AdditionalInfo"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "additionalInfo",
                "agendaEventType",
                "agendaItemContext",
                "description",
                "end",
                "label",
                "start"
            ],
            "title": "GetMyAgendaEvent"
        },
        "AdditionalInfo": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "key": {
                    "type": "string"
                },
                "value": {
                    "type": "string",
                    "format": "boolean"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "key",
                "value"
            ],
            "title": "AdditionalInfo"
        },
        "AgendaItemContext": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "entityId": {
                    "type": "string",
                    "format": "integer"
                },
                "entityType": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "entityId",
                "entityType"
            ],
            "title": "AgendaItemContext"
        }
    }
}

```

</details>

[[Index](#index)]

### getStudentStageGroupS21

<details>
<summary> Query </summary>

```
query getStudentStageGroupS21($studentId: UUID!) {
  school21 {
    getStageGroupS21PublicProfile(studentId: $studentId) {
      waveId
      waveName
      eduForm
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "studentId": {
                    "type": "string",
                    "format": "uuid"
                }
            },
            "required": [
                "studentId"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "school21": {
                    "$ref": "#/definitions/School21"
                }
            },
            "required": [
                "school21"
            ],
            "title": "Data"
        },
        "School21": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getStageGroupS21PublicProfile": {
                    "$ref": "#/definitions/GetStageGroupS21PublicProfile"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getStageGroupS21PublicProfile"
            ],
            "title": "School21"
        },
        "GetStageGroupS21PublicProfile": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "waveId": {
                    "type": "integer"
                },
                "waveName": {
                    "type": "string"
                },
                "eduForm": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "eduForm",
                "waveId",
                "waveName"
            ],
            "title": "GetStageGroupS21PublicProfile"
        }
    }
}

```

</details>

[[Index](#index)]

### calendarGetEvents

<details>
<summary> Query </summary>

```
query calendarGetEvents($from: DateTime!, $to: DateTime!) {
  calendarEventS21 {
    getMyCalendarEvents(from: $from, to: $to) {
      ...CalendarEvent
      __typename
    }
    __typename
  }
}

fragment CalendarEvent on CalendarEvent {
  id
  start
  end
  description
  eventType
  eventCode
  eventSlots {
    id
    type
    start
    end
    __typename
  }
  bookings {
    ...CalendarReviewBooking
    __typename
  }
  exam {
    ...CalendarEventExam
    __typename
  }
  studentCodeReview {
    studentGoalId
    __typename
  }
  activity {
    ...CalendarEventActivity
    studentFeedback {
      id
      rating
      comment
      __typename
    }
    status
    activityType
    isMandatory
    isWaitListActive
    isVisible
    comments {
      type
      createTs
      comment
      __typename
    }
    organizers {
      id
      login
      __typename
    }
    __typename
  }
  goals {
    goalId
    goalName
    __typename
  }
  penalty {
    ...Penalty
    __typename
  }
  __typename
}

fragment CalendarReviewBooking on CalendarBooking {
  id
  answerId
  eventSlotId
  task {
    id
    goalId
    goalName
    studentTaskAdditionalAttributes {
      cookiesCount
      __typename
    }
    assignmentType
    __typename
  }
  eventSlot {
    id
    start
    end
    event {
      eventUserRole
      __typename
    }
    __typename
  }
  verifierUser {
    ...CalendarReviewUser
    __typename
  }
  verifiableStudent {
    id
    user {
      ...CalendarReviewUser
      __typename
    }
    __typename
  }
  bookingStatus
  team {
    ...ProjectTeamMembers
    __typename
  }
  isOnline
  vcLinkUrl
  __typename
}

fragment CalendarReviewUser on User {
  id
  login
  __typename
}

fragment ProjectTeamMembers on ProjectTeamMembers {
  id
  teamLead {
    ...ProjectTeamMember
    __typename
  }
  members {
    ...ProjectTeamMember
    __typename
  }
  invitedUsers {
    ...ProjectTeamMember
    __typename
  }
  teamName
  teamStatus
  minTeamMemberCount
  maxTeamMemberCount
  __typename
}

fragment ProjectTeamMember on User {
  id
  avatarUrl
  login
  userExperience {
    level {
      id
      range {
        levelCode
        __typename
      }
      __typename
    }
    cookiesCount
    codeReviewPoints
    __typename
  }
  __typename
}

fragment CalendarEventExam on Exam {
  examId
  eventId
  beginDate
  endDate
  name
  location
  currentStudentsCount
  maxStudentCount
  updateDate
  goalId
  goalName
  isWaitListActive
  isInWaitList
  stopRegisterDate
  __typename
}

fragment CalendarEventActivity on ActivityEvent {
  activityEventId
  eventId
  name
  beginDate
  endDate
  isRegistered
  description
  currentStudentsCount
  maxStudentCount
  location
  updateDate
  isWaitListActive
  isInWaitList
  stopRegisterDate
  __typename
}

fragment Penalty on Penalty {
  comment
  id
  duration
  status
  startTime
  createTime
  penaltySlot {
    currentStudentsCount
    description
    duration
    startTime
    id
    endTime
    __typename
  }
  reasonId
  __typename
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "from": {
                    "type": "string",
                    "format": "date-time"
                },
                "to": {
                    "type": "string",
                    "format": "date-time"
                }
            },
            "required": [
                "from",
                "to"
            ],
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "calendarEventS21": {
                    "$ref": "#/definitions/CalendarEventS21"
                }
            },
            "required": [
                "calendarEventS21"
            ],
            "title": "Data"
        },
        "CalendarEventS21": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getMyCalendarEvents": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/GetMyCalendarEvent"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getMyCalendarEvents"
            ],
            "title": "CalendarEventS21"
        },
        "GetMyCalendarEvent": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "start": {
                    "type": "string",
                    "format": "date-time"
                },
                "end": {
                    "type": "string",
                    "format": "date-time"
                },
                "description": {
                    "type": "string"
                },
                "eventType": {
                    "type": "string"
                },
                "eventCode": {
                    "type": "string"
                },
                "eventSlots": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/EventSlot"
                    }
                },
                "bookings": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/Booking"
                    }
                },
                "exam": {
                    "type": "null"
                },
                "studentCodeReview": {
                    "type": "null"
                },
                "activity": {
                    "type": "null"
                },
                "goals": {
                    "type": "array",
                    "items": {}
                },
                "penalty": {
                    "type": "null"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "activity",
                "bookings",
                "description",
                "end",
                "eventCode",
                "eventSlots",
                "eventType",
                "exam",
                "goals",
                "id",
                "penalty",
                "start",
                "studentCodeReview"
            ],
            "title": "GetMyCalendarEvent"
        },
        "Booking": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "answerId": {
                    "type": "string",
                    "format": "integer"
                },
                "eventSlotId": {
                    "type": "string",
                    "format": "integer"
                },
                "task": {
                    "$ref": "#/definitions/Task"
                },
                "eventSlot": {
                    "$ref": "#/definitions/EventSlot"
                },
                "verifierUser": {
                    "$ref": "#/definitions/User"
                },
                "verifiableStudent": {
                    "$ref": "#/definitions/VerifiableStudent"
                },
                "bookingStatus": {
                    "type": "string"
                },
                "team": {
                    "anyOf": [
                        {
                            "$ref": "#/definitions/Team"
                        },
                        {
                            "type": "null"
                        }
                    ]
                },
                "isOnline": {
                    "type": "boolean"
                },
                "vcLinkUrl": {
                    "type": "null"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "answerId",
                "bookingStatus",
                "eventSlot",
                "eventSlotId",
                "id",
                "isOnline",
                "task",
                "team",
                "vcLinkUrl",
                "verifiableStudent",
                "verifierUser"
            ],
            "title": "Booking"
        },
        "Event": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "eventUserRole": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "eventUserRole"
            ],
            "title": "Event"
        },
        "Task": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "goalId": {
                    "type": "string",
                    "format": "integer"
                },
                "goalName": {
                    "type": "string"
                },
                "studentTaskAdditionalAttributes": {
                    "$ref": "#/definitions/StudentTaskAdditionalAttributes"
                },
                "assignmentType": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "assignmentType",
                "goalId",
                "goalName",
                "id",
                "studentTaskAdditionalAttributes"
            ],
            "title": "Task"
        },
        "StudentTaskAdditionalAttributes": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "cookiesCount": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "cookiesCount"
            ],
            "title": "StudentTaskAdditionalAttributes"
        },
        "Team": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "teamLead": {
                    "$ref": "#/definitions/TeamLead"
                },
                "members": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/TeamLead"
                    }
                },
                "invitedUsers": {
                    "type": "array",
                    "items": {}
                },
                "teamName": {
                    "type": "string"
                },
                "teamStatus": {
                    "type": "string"
                },
                "minTeamMemberCount": {
                    "type": "integer"
                },
                "maxTeamMemberCount": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "invitedUsers",
                "maxTeamMemberCount",
                "members",
                "minTeamMemberCount",
                "teamLead",
                "teamName",
                "teamStatus"
            ],
            "title": "Team"
        },
        "TeamLead": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "avatarUrl": {
                    "type": "string"
                },
                "login": {
                    "type": "string"
                },
                "userExperience": {
                    "$ref": "#/definitions/UserExperience"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "avatarUrl",
                "id",
                "login",
                "userExperience"
            ],
            "title": "TeamLead"
        },
        "UserExperience": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "level": {
                    "$ref": "#/definitions/Level"
                },
                "cookiesCount": {
                    "type": "integer"
                },
                "codeReviewPoints": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "codeReviewPoints",
                "cookiesCount",
                "level"
            ],
            "title": "UserExperience"
        },
        "Level": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "integer"
                },
                "range": {
                    "$ref": "#/definitions/Range"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "range"
            ],
            "title": "Level"
        },
        "Range": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "levelCode": {
                    "type": "integer"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "levelCode"
            ],
            "title": "Range"
        },
        "VerifiableStudent": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "user": {
                    "$ref": "#/definitions/User"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "user"
            ],
            "title": "VerifiableStudent"
        },
        "User": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "uuid"
                },
                "login": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "login"
            ],
            "title": "User"
        },
        "EventSlot": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "start": {
                    "type": "string",
                    "format": "date-time"
                },
                "end": {
                    "type": "string",
                    "format": "date-time"
                },
                "event": {
                    "$ref": "#/definitions/Event"
                },
                "__typename": {
                    "type": "string"
                },
                "type": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "end",
                "id",
                "start"
            ],
            "title": "EventSlot"
        }
    }
}

```

</details>

[[Index](#index)]

### getPenaltyReasons

<details>
<summary> Query </summary>

```
query getPenaltyReasons {
  penalty {
    getPenaltyReasons {
      id
      name
      __typename
    }
    __typename
  }
}

```

</details>

<details>
<summary> Variables </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Variables",
    "definitions": {
        "Variables": {
            "type": "object",
            "additionalProperties": false,
            "title": "Variables"
        }
    }
}

```

</details>

<details>
<summary> Data </summary>

```json
{
    "$schema": "http://json-schema.org/draft-06/schema#",
    "$ref": "#/definitions/Data",
    "definitions": {
        "Data": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "penalty": {
                    "$ref": "#/definitions/Penalty"
                }
            },
            "required": [
                "penalty"
            ],
            "title": "Data"
        },
        "Penalty": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "getPenaltyReasons": {
                    "type": "array",
                    "items": {
                        "$ref": "#/definitions/GetPenaltyReason"
                    }
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "getPenaltyReasons"
            ],
            "title": "Penalty"
        },
        "GetPenaltyReason": {
            "type": "object",
            "additionalProperties": false,
            "properties": {
                "id": {
                    "type": "string",
                    "format": "integer"
                },
                "name": {
                    "type": "string"
                },
                "__typename": {
                    "type": "string"
                }
            },
            "required": [
                "__typename",
                "id",
                "name"
            ],
            "title": "GetPenaltyReason"
        }
    }
}

```

</details>

[[Index](#index)]