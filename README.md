# Copilot Agents Demo

Use the following 3 files to setup your Copilot Agents demo. 
Create a repo with the same README file as this one.
Paste the ISSUE.md file into a new issue in that repository. 
Assign Copilot to the new Issue in the new repository.
Use the STEER.md file to course correct the agent mid session. 

## What this demo shows
- Assign an issue to Copilot to start an agent task
- Monitor progress in AgentHQ
- Re-steer mid-session with a new requirement
- Review the resulting PR like a teammate’s work

## Demo files
- `ISSUE.md` contains the exact issue text to copy/paste into GitHub
- `STEER.md` contains the mid-session requirement change to paste while the agent is working

## Quick demo steps
1. Create a new GitHub Issue by copying the Title and Body from `ISSUE.md`
2. Assign the issue to Copilot to start the agent task
3. Open AgentHQ to monitor progress
4. Paste `STEER.md` into the agent session to re-steer the work
5. Review the PR diff for clarity, completeness, and constraints.
6. Verify the PR edited the README.md file by adding priority levels plus the steered examples. 

---

## Ticket Triage Policy

We triage support tickets using Severity (how bad the impact is) and Priority (how soon we act).

### Severity levels
- Low means minor annoyance with an easy workaround
- Medium means a meaningful user impact but workarounds exist
- High means blocks key workflows or causes data loss

### Priority levels
- P0 Critical: widespread outage or data loss. Drop other work, respond now, fix within 24 hours
- P1 High: key workflow blocked for many users, no reasonable workaround. Fix in the current sprint
- P2 Medium: meaningful impact with a workaround. Schedule in an upcoming sprint
- P3 Low: minor or cosmetic. Fix opportunistically or backlog it

### Severity to default Priority

| Severity | Scope | Default Priority |
| --- | --- | --- |
| High | Many users or data loss | P0 |
| High | Single user or team | P1 |
| Medium | Any | P2 |
| Low | Any | P3 |

Raise or lower one level when there is a security risk, a customer commitment, or a solid workaround. Record the reason on the ticket.

### How to triage in 60 seconds
1. Reproduce or confirm the report
2. Pick the Severity
3. Check the scope, how many users are affected
4. Apply the default Priority from the table, adjust one level if needed and note why
5. Assign an owner and label the ticket

### Example tickets
- Checkout fails for all users after deploy, no workaround. High severity, many users, so P0
- Admin cannot export the monthly report, other admins are unaffected and export works via API. High severity, single user, but a workaround exists, so lower one level to P2 and note the workaround
- Dashboard chart legend overlaps on small screens. Low severity, cosmetic, so P3

### Current rules
- Triage happens daily
- P0 tickets page the on call owner immediately
- Every ticket gets a Severity, a Priority, and an owner at triage time
