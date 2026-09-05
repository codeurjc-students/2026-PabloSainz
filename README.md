# TrainFyre: Incident Management System for Multimodal Transport Networks

## Description

A system capable of collecting data from various transport sources. 
This data will be used and processed to provide various functionalities, 
such as allowing users to receive notifications regarding lines of interest
and statistics related to those lines.

[TODO example screens]

## Objectives

The objectives of this project center on the ability to collect and process
alerts from various sources in order to offer a range of services to users similar
to those provided by official websites like [Metro Madrid](https://www.metromadrid.es/es) 
and [Renfe](https://www.adif.es/viajeros/estado-de-la-red), or apps like [Moovit](https://moovitapp.com/es).

> [!WARNING]
> Only the objectives will be defined below; however, their implementation has not yet begun.

### Functional objectives

The functional objectives will be delivered in a phased manner across iterations.
Some functional objectives may change in the future.

These functional objectives/features will be accessible based on user roles:
anonymous, registered, and administrator. These are listed in order of privilege,
with the administrator having access to all features offered by the software.

The project's functional objectives are listed below, indicating the minimum
privilege level (role) required for access:

* Register in the system (anonymous).
* View general statistics for the lines or their status (anonymous).
* Create alert subscriptions to subsequently receive notifications (registered).
* Log in and log out (registered).
* CRUD operations on entities other than the user (admin).
* View or collect audit information and statistics on the system and/or lines (admin).

As the project progresses and it becomes apparent which features could offer more value, 
they will be added to this list.

### Technical objectives

* Hexagonal Architecture.
* Security via roles and JWT.
* Management and sending of alerts/notifications (email).
* Expose the data using a REST API.
* Static code analysis (Sonar qube).
* Consume Various data sources.

## Methodology

Work will be carried out in iterations, meeting objectives in a phased manner
that allows for changes. Similarly, only dates for key milestones will be scheduled,
and work completed for each delivery (one delivery per milestone) will be recorded,
capturing the start and end dates of tasks performed during the iteration.

Given the complexity and difficulty of the project's objective,
sound software design principles, patterns, and practices will be followed
to the extent possible; these are:

* Hexagonal architecture: It is useful, as it will receive data from various sources.
  Furthermore, its modularity will facilitate testing and maintenance.
* DDD (domain driven design): improving communication and maintainability
  (ubiquitous language), enabling the creation of a more modular and maintainable system
* EDA (Event driven architecture): Enabling the reduction of dependencies between
  services and their subsequent division into microservices (monolith-first approach).
* TDD (test driven development): improving software design,
  drastically reducing errors, and enabling code modification without fear,
  thanks to a safety net of automated tests created before the source code

The gantt will be added [HERE] when it is created.
You can see the current project status on it's related github project on: "See also"

## Detailed features

|              | anonymous | registered | admin |
| ------------ |-----------|------------|-------|
| basic        |Register in the system           |Log in and log out            |CRUD operations on entities other than the user       |
| intermediate |View general statistics for the lines or their status           |Create alert subscriptions to subsequently receive notifications            |View or collect audit information and statistics on the system and/or lines       |
| advanced     | TODO      | TODO       | TODO  |


## Analysis

TODO (As the project progresses)

[Website layout](https://www.figma.com/design/4TL76NTkyb7FL6PTQH29iN/Trainfyre-maquetaci%C3%B3n?node-id=305-5749&t=TcFFmUE4bhh7lFds-1). Please note that this layout is only a prototype and may change during future development and implementation.

## Follow-up

GitHub project used to track this project: [link](https://github.com/orgs/codeurjc-students/projects/52)

You can also visit: [Project blog]()

## Author

This application is being developed as part of the Bachelor's Thesis of 
Pablo Sainz López, who is pursuing a double degree in Computer Engineering
and Computer Systems Engineering at the ETSII of the URJC.

## See also

* [Changelog](https://github.com/codeurjc-students/2026-PabloSainz/blob/main/CHANGELOG.md)
* [Ai_usage](https://github.com/codeurjc-students/2026-PabloSainz/blob/main/AI_USAGE.md)
