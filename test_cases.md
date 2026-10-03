# DelegateAI: Initial Test Cases

## Decision rule
Ask when missing information could materially change the work.
Proceed when the available context is sufficient for a useful answer.

## Shared sample paragraph
A fictional reading app tested a new onboarding flow with
20 volunteers. Twelve completed setup without help.
Eight struggled to select reading interests.
The team plans to simplify that step.

## Test 1: Clear request
Request: "Summarize the sample paragraph in three bullets."
Context: The sample paragraph is provided.
Expected decision: PROCEED.
Reason: The input, task, and output format are clear.

## Test 2: Missing task details
Request: "Prepare something for my meeting tomorrow."
Context: No meeting details or prior conversation are available.
Expected decision: ASK.
Suggested question: "Which meeting is this for, and what
do you need to be ready to do?"
Reason: The assistant cannot determine what to prepare.

## Test 3: Optional context
Request: "Summarize the sample paragraph in three bullets
for my meeting tomorrow."
Context: The sample paragraph is provided.
Expected decision: PROCEED.
Reason: Meeting details are not essential to complete
the requested summary.
