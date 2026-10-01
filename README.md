# Python unittest walkthrough

A fork of the Code Institute solution repository showing three stages of the same even-number testing exercise.

[Português (Brasil)](README.pt-BR.md)

## Process record

Source reviewed on 2026-10-01. The repository records a learning exercise, not a shipped product. No dated planning notes, user research or wireframes were found in the reviewed files. The architecture below describes the code that exists; it does not invent a development diary.

## Idea, architecture and design

Each `testing_with_python_01/`, `_02/` and `_03/` folder contains its own evens.py and test_evens.py. Stage 01 is a stub returning None with an empty test class. Stage 02 implements counting with a loop; stage 03 uses a comprehension and sum. This sequence is present in the course material, not evidence of original product design or a personal development timeline. No UI, database or deployment exists in the reviewed root.

## Run and test

Run from one stage at a time so `from evens import ...` resolves to the matching module:

```bash
cd testing_with_python_03
python3 evens.py
python3 -m unittest -v test_evens
```

No third-party package is imported by these exercise files. Stages 02 and 03 each have two test methods covering a non-list error, empty list, two evens, one even and no evens. Stage 01 has no test methods. The stage 02 direct demo passes 5 and therefore raises the intended TypeError; use its test command to inspect behavior instead of expecting a successful demo. Tests were not rerun during this update.

## Limits and next checks

An empty list or zero even numbers returns False; a non-zero even count returns True. Elements are not validated before modulo. Check mixed types, negatives, zero and booleans before general reuse. This is course reference code, not a portfolio claim of original authorship.

## Snapshots

No application UI exists to capture. No screenshot was added. If terminal evidence is useful later, save a dated test-output capture under `docs/assets/`, showing the command and actual result without private paths or data. Do not invent a dashboard or claim tests passed.

## Credits and licensing

Forked from [Code-Institute-Solutions/unittest-python-testing](https://github.com/Code-Institute-Solutions/unittest-python-testing). Original source remains unchanged. No new license is applied to third-party course code.
