# DelegateAI

Helping AI assistants understand what users mean before doing the work.

## The problem
People express requests naturally, through voice or text.
Their requests may include corrections, several intentions,
or missing context.

An assistant may act on the wrong interpretation.
Asking unnecessary questions can also waste the user's time.

## The idea
DelegateAI is an experimental interaction layer that:
- Identifies the user's intended task.
- Preserves corrections, constraints, and important context.
- Proceeds when the request is sufficiently clear.
- Asks a targeted question when missing information
  could materially change the result.

It is designed to explore a capability that could fit
inside a general-purpose AI assistant.

## Example
"Prepare slides for Friday—actually Thursday.
First explain why sales dropped. Don't send anything."

The assistant should preserve Thursday as the date,
analyze the decline before preparing slides, and avoid sending.
If the necessary sales data is missing, it should ask for it.

## First prototype
A simple interface accepting typed requests or pasted
voice transcripts. It will clarify when needed, then
complete the task using the available information.

Live voice input and automatic model selection are
possible future extensions.

## How I will evaluate it
Compare DelegateAI with the same model handling requests
normally, using the same context and tools.

Measure:
- Correct understanding and task completion
- Unnecessary clarification questions
- User time spent clarifying and correcting
- Total response time
- AI cost per successful task

## Data
Initial tests will use fictional requests and synthetic data.
No employer, customer, or confidential business data will be used.

## Status
Early prototype planning. No performance results yet.

## Next steps
1. Create clear and ambiguous test requests.
2. Define when clarification is useful.
3. Build the first working version.
4. Compare results and document failures.