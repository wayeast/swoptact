Swoptact: a FOSS contact management system
==========================================

Swoptact is an [free & open source software](LICENSE.md) contact
management system for you and your organization.

# Overview

## Abstract

Swoptact is a list of contacts with a history of their event
attendance (making it also a list of events over time).  Use it to
keep track of people your organization comes into contact with over
time, and see how their engagement with your mission grows.


## User stories

These are stories about how various users make use of Swoptact.

Three kinds of users:
Sarah does data entry and is the most frequest user of Swoptact.
Colleen is an organizer and uses Swoptact to find information about
her contacts and occasionally update their information.
Michelle is a supervisor and runs reports from Swoptact.

### Why Sarah chose Swoptact

This is a high level overview of why Sarah thinks Swoptact will be
useful to her.

Swoptact has a simple interface that makes it fast and easy for Sarah
to enter her data.  It lets her keep track of the best way to contact
her constituents (used loosely) and to view their involvement over
time (meaning their event attendance over time).  She can search for
people when she only remembers a first or last name, and look for
people who live on a specific street when she wants to plan block-wide
events.

### Sarah's big event

This user story talks about Sarah, the event she ran, and what
information she kept after the event.

#### Before the conference

1. Sarah makes the conference, including its name and date, in
   Swoptact.
2. ?

#### Immediately after the conference

1. Sarah takes the paper sign-in sheet and enters the attendees into
   Swoptact. TBD: maybe some of them already have records and others
   don't?
   It is easy for Sarah to add conference attendance of a person who
   already has a Swoptact record and a person who does not.
2. Sarah realizes that one of the people she is entering has a new
   phone number, so she changes it to the new (correct) number.
3. Sarah sees that a person she added already had a record in
   Swoptact, so she merges the new record with the pre-existing one.
4. Sarah sees that that person doesn't exist in real life after all,
   so she deletes the record.
5. Sarah realizes that one person didn't come to the conference, so
   she removes him from the attendees list.

#### Later usage
1. Sarah looks at a list of conference participants.
2. Sarah finds the emails of all conference participants so she can
   send them a follow-up. TBD: does she send the email from Swoptact?
3. Sarah realizes the conference name has a typo, so she changes it.
4. Sarah reports on one person's attendance at events and conferences
   over time.
5. Sarah looks for people who went to both the conference and to
   another meeting.
6. Michelle reports to the board on attendance over time at conferences.
7. Colleen looks up a contact's phone number to schedule a one-on-one
   meeting.
8. Colleen looks up phone numbers for all the people who attended the
   conference, so she can invite them to another event.

## Interface
### Data Fields
Participants: first name, last name, phone number, address (street
number, street direction, street name, street type), email address
Events: name, date, location (site name and all address fields)

### Functionality
#### Participants:
search, create, modify, delete, merge, link to event, unlink from event
#### Events:
search, create, modify, delete, merge, link to participant, unlink from participant

## Database
### Participants
#### id
#### first name
#### last name
#### phone number
#### street number
#### street direction
#### street name
#### street type
#### email address
### Events
#### id
#### name
#### date
#### site name
#### street number
#### street direction
#### street name
#### street type


### Participants_Events
#### primary key...!
#### participant id
#### event id
#### date linked
#### date unlinked?

### Users and permissions

Making use of Django's builtins

### Contacts
### Events
# Installation
See (INSTALL.md)[INSTALL.md].
