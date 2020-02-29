# Mentorioum Glossary

## Who

* Mentor
* Trainee
* Assistant

## What

* Learning Session (Flow)
* Learning Content Preparation
* Cources register

## How

* Procceed with Learning Session
* Search for particular events in other systems
* Verification of trainees knoweledges (such as manual it's only particular use case)

## Where

* Various other systems like Github, Gitlab, etc
* Cloud

## Volatilities List

### Mentoring Session

It looks like a core functionality of the system, so Mentors can cooperate to
create a complex sessions, or Mentor can extend session as it needs. There are a lot of ways on how learning material could be
transformed to mentoring flow like (tasks), how participants of flow would see new tasks (immediately or get them one by one as they proceed with them),
As users would move from one tasks to another we have to keep state of that session, because it may take a long time while users finish it.
That part of the system should't know about particular ticket system or how to verify task, however it should know on whom can
do verification.

```
EducationManager
SessionGenerationEngine
SessionAccess

```

### Learning Content and Verification

Even if system supports it's own format for defining content for learning, it's not enough and it should support
various LMS types. So content would wary from system to system. Another volatility area is a way on how verification
is done, it's could be a `manual` verification, when mentor just have a task to verify a trainee's knoweledge, or
it can be an automated verification (test forms, automatic code verification).
Learning content could be stored in it's own LMS system, so sometimes it may appear that we need to integrate
with their API to do read/verify learning steps. However, if standalone system has it's own learning flow,
we no need to burden our learning session with it's internals and just have an ability to report about trainees
verifications/scores.

Mentors can register their cources to system. Also mentors can prepare cource as adapter to thirdparty LMS to integrate with
system
