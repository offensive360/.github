# Application security evaluation worksheet

Author: The Offensive360 Team

Updated: 2026-09-13 · Version 1.0

Application security resources: https://offensive360.com/resources/

Use this vendor-neutral worksheet to compare a tool or service against your team's actual requirements. It covers source analysis, web and API testing, mobile analysis, asset discovery, governance workflows, and optional AI-assisted testing. Complete only the sections that apply to your evaluation.

This is an evidence record, not a certification checklist or a universal scanner benchmark. A completed worksheet does not establish that an application is secure.

## How to use it

1. Agree the scope, representative inputs, and acceptance criteria before testing.
2. Record the exact tool version, application revision, configuration, and environment.
3. Include both known weaknesses and equivalent safe controls where detection is being evaluated.
4. Record actual results and evidence; leave unexecuted checks as **Not tested**.
5. Assign an owner and next step to every failed, partial, or unresolved requirement.
6. Repeat relevant checks after a fix or material configuration change.

Use evidence IDs or access-controlled links. Do not paste credentials, personal data, or production source code into a worksheet that will be shared externally.

## 1. Evaluation brief

| Field | Your record |
| --- | --- |
| Evaluation name / ID | |
| Decision to make | |
| Evaluation owner and participating teams | |
| Vendor / tool / service being evaluated | |
| Product, edition, version, and enabled features | |
| Application or project and exact revision | |
| Languages, frameworks, package formats, and runtime versions | |
| Deployment model and environment | |
| Required identity, pipeline, ticketing, and reporting integrations | |
| Data handling, residency, retention, or offline requirements | |
| Agreed test dates and decision date | |
| Written scope / authorization reference | |
| Included assets, repositories, routes, and test roles | |
| Excluded systems, actions, data, and known coverage limits | |
| Stop conditions and responsible contact | |

## 2. Result definitions

| Result | Meaning |
| --- | --- |
| Pass | The agreed criterion was exercised and supporting evidence demonstrates the expected result. |
| Partial | A defined part worked, but a required part remains unmet or unverified. Describe both. |
| Fail | The check ran and evidence shows that the agreed criterion was not met. |
| Not tested | The check did not run, could not complete, or has insufficient evidence to decide. Record why. |
| Not applicable | The criterion is outside the agreed scope. Record the reason and the scope owner's agreement. |

Do not count **Not tested** or **Not applicable** as a pass. Do not turn a partial result into a single favorable score. A check that failed to run is different from a completed check that found no issue.

## 3. Acceptance criteria

Adapt the starting criteria below before testing. Define any required thresholds, expected outputs, and acceptable limitations in the acceptance-condition column. These are questions to verify, not claims about any vendor.

| ID | Criterion | Your acceptance condition | Result | Evidence / unresolved point |
| --- | --- | --- | --- | --- |
| E01 | Required languages, frameworks, package formats, or asset types are demonstrated with representative inputs. | | | |
| E02 | The actual analyzed scope, omissions, errors, and skipped checks are visible. | | | |
| E03 | Known weaknesses and safe controls are assessed under the same recorded configuration. | | | |
| E04 | A sample finding has inspectable location, rationale, and supporting evidence. | | | |
| E05 | A developer can investigate, remediate, and retest a representative finding. | | | |
| E06 | Required authentication, permissions, and role boundaries work for the intended workflow. | | | |
| E07 | A representative pipeline or scheduling workflow completes with understandable failure behavior. | | | |
| E08 | Required exports and integrations preserve the information needed for triage and ownership. | | | |
| E09 | Data handling, access controls, retention, and deployment requirements are confirmed. | | | |
| E10 | Offline workflows, updates, licensing, and export are demonstrated if disconnected operation is required. | | | |
| E11 | Workload, resource use, scan time, and investigation effort are measured for the agreed test scope. | | | |
| E12 | Product scope, capacity, support, maintenance ownership, expansion, and renewal terms are clear. | | | |

### Additional questions by evaluation type

Choose the relevant rows and turn each into a concrete acceptance criterion above. A feature name or a successful login alone is not evidence that the full workflow was exercised.

| Evaluation type | Evidence to request or produce |
| --- | --- |
| Source analysis | Representative language/framework handling; affected code; rule rationale; available data flow; unsupported constructs and analysis failures. |
| Web / API testing | Authenticated reachability for each required role; route/API scope; excluded state-changing actions; request/response evidence; distinction between confirmed and potential findings. |
| Mobile analysis | Exact Android/iOS package and version; analysis mode; packaging/obfuscation limits; explicit separation of source, binary, and runtime observations. |
| Asset discovery | Ownership attribution; discovery sources; freshness; exposure observations; false associations; change history. |
| Governance, risk, and compliance | One representative control, risk, evidence item, approval, and report moving through the required owners and permissions. |
| AI-assisted testing | Written scope; tool permissions; approval checkpoints; excluded actions; stop controls; evidence beyond a generated narrative. |

## 4. Test-case record

Copy this block for each important positive case, safe control, or operational workflow.

- Case ID and linked acceptance criterion:
- Question this case answers:
- Input or fixture ID and exact version:
- Case type: known weakness / safe control / operational workflow
- Preconditions, role, and relevant configuration:
- Expected result agreed before the run:
- Steps performed and run ID:
- Actual result: Pass / Partial / Fail / Not tested / Not applicable
- Evidence reference:
- Scope actually exercised and any skipped work:
- Reviewer, review date, and limitations:
- Next action and owner:

### Detection comparison record, where applicable

| Case ID | Expected weak or safe behavior | Tool observation | Reviewer-confirmed outcome | Evidence / scope limits |
| --- | --- | --- | --- | --- |
| | | | | |
| | | | | |
| | | | | |

Keep missed issues and unexpected safe-control findings visible. Use a consistent unit when counting findings, and record the denominator and scope for any detection or false-positive rate. Counts from different scopes or different finding-grouping rules are not directly comparable.

## 5. Remediation and retest

| Field | Your record |
| --- | --- |
| Finding / test-case ID | |
| Developer or remediation owner | |
| Time spent understanding and investigating the finding | |
| Fix or configuration change and revision | |
| Behavior that must remain intact | |
| Retest steps, run ID, and result | |
| Evidence that the intended behavior still works | |
| Remaining limitation or accepted exception | |

Keep investigation effort separate from automated run time. A result that disappears after a configuration change may reflect lost coverage; confirm that the relevant check still ran.

## 6. Unresolved items and decision

| Criterion / case | Unresolved requirement or limitation | Owner | Next action | Due date | Decision impact |
| --- | --- | --- | --- | --- | --- |
| | | | | | |
| | | | | | |
| | | | | | |

- Requirements demonstrated with evidence:
- Requirements only partially demonstrated:
- Failed requirements:
- Untested or unavailable requirements:
- Out-of-scope requirements and rationale:
- Blocking issues:
- Proposed decision and evidence supporting it:
- Conditions that must be met before rollout:
- Decision owner and date:
- Date or event that triggers reevaluation:

Keep the completed record with the evaluated configuration and supporting evidence. Revisit the decision when the application, deployment model, enabled features, or requirements materially change.

---

Maintained by The Offensive360 Team. Explore the related resources: https://offensive360.com/resources/
