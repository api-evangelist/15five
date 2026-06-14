# 15Five GraphQL Schema

This document describes a conceptual GraphQL schema for the 15Five continuous performance management platform. The schema is derived from the 15Five Public REST API and models the core domain objects available through the platform.

## Overview

15Five provides a REST API for managing continuous performance data including users, teams, check-ins, OKRs, 1-on-1 meetings, review cycles, pulse surveys, and recognition. This GraphQL schema represents those capabilities in a typed graph model.

- Base API: https://my.15five.com/api/public/
- Documentation: https://success.15five.com/hc/en-us/articles/360002699631-API
- Authentication: API key via HTTP Basic Auth
- Rate Limit: 5 requests per second per IP

## Schema File

See [15five-schema.graphql](15five-schema.graphql) for the full schema definition.

## Core Types

### Identity and Access

- `User` — A 15Five platform user (employee or manager)
- `UserDetails` — Extended profile information for a user
- `UserRole` — Role assignment for a user within the platform
- `Manager` — A user designated as a people manager
- `DirectReport` — A user who reports to a manager
- `APIKey` — An API key used to authenticate with the 15Five API
- `Token` — An authentication token

### Teams and Groups

- `Team` — An organizational team within 15Five
- `TeamDetails` — Extended attributes of a team
- `Group` — A logical grouping of users
- `GroupDetails` — Extended attributes of a group

### Check-Ins

- `CheckIn` — A weekly check-in record submitted by a user
- `CheckInDetails` — Extended content of a check-in
- `CheckInResponse` — Manager or peer response to a check-in
- `Response` — A general response object
- `ResponseItem` — An individual item within a response

### Goals and OKRs

- `Goal` — A goal set by a user or team
- `GoalDetails` — Extended details of a goal
- `GoalStatus` — Current status of a goal
- `GoalType` — Classification of a goal
- `GoalProgress` — Progress tracking record for a goal
- `KeyResult` — A measurable key result tied to an objective
- `KeyResultDetails` — Extended details of a key result
- `OKR` — An Objective and Key Result
- `OKRDetails` — Extended details of an OKR
- `OKRCycle` — A time-boxed period for OKR tracking

### 1-on-1 Meetings

- `OneOnOne` — A 1-on-1 meeting record between manager and report
- `OneOnOneDetails` — Extended details of a 1-on-1 meeting
- `OneOnOneNote` — A note attached to a 1-on-1 meeting
- `OneOnOneAgenda` — The agenda for a 1-on-1 meeting
- `AgendaItem` — An individual item on a 1-on-1 agenda
- `AgendaItemStatus` — Status of an agenda item

### Reviews

- `Review` — A performance review record
- `ReviewDetails` — Extended content of a performance review
- `ReviewType` — Classification of a review (self, peer, manager)
- `ReviewCycle` — A time-boxed review cycle period
- `ReviewQuestion` — A question included in a review
- `ReviewResponse` — A response to a review question

### Ratings

- `Rating` — A rating assigned during a review or pulse
- `RatingDetails` — Extended details of a rating

### Surveys and Engagement

- `Survey` — A survey distributed to users
- `SurveyDetails` — Extended content of a survey
- `SurveyQuestion` — A question within a survey
- `SurveyResponse` — A user's response to a survey
- `Engagement` — An engagement measurement record
- `EngagementScore` — A computed engagement score for a user or team
- `Pulse` — A pulse survey record
- `PulseDetails` — Extended details of a pulse survey

### Recognition

- `Recognition` — A recognition event given to a user
- `RecognitionDetails` — Extended details of a recognition event
- `Badge` — A badge that can be awarded for recognition
- `BadgeDetails` — Extended details of a badge
- `Shoutout` — A public shoutout given to a user
- `ShoutoutDetails` — Extended details of a shoutout

### Webhooks

- `Webhook` — A registered webhook endpoint
- `WebhookEvent` — An event payload delivered to a webhook
