# Nielsen's 10 Usability Heuristics

Reference definitions and scoring criteria for proactive heuristic application during UX research. Based on Jakob Nielsen's heuristics (Nielsen Norman Group, 1994).

Source: https://www.nngroup.com/articles/ten-usability-heuristics/

---

## H1: Visibility of System Status

The design should always keep users informed about what is going on, through appropriate feedback within a reasonable amount of time.

**Apply when:** The feature involves loading, processing, state changes, or multi-step flows where the user might lose track of progress or status.

---

## H2: Match Between System and Real World

The design should speak the users' language. Use words, phrases, and concepts familiar to the user, rather than internal jargon. Follow real-world conventions, making information appear in a natural and logical order.

**Apply when:** The feature uses domain-specific terminology, icons, or metaphors that may not match user mental models.

---

## H3: User Control and Freedom

Users often perform actions by mistake. They need a clearly marked "emergency exit" to leave the unwanted action without having to go through an extended process.

**Apply when:** The feature involves destructive actions, commitments, navigation dead-ends, or flows where users might want to backtrack.

---

## H4: Consistency and Standards

Users should not have to wonder whether different words, situations, or actions mean the same thing. Follow platform and industry conventions.

**Apply when:** The feature introduces new patterns, terminology, or interactions that may conflict with established conventions in the product or industry.

---

## H5: Error Prevention

Good error messages are important, but the best designs carefully prevent problems from occurring in the first place. Either eliminate error-prone conditions, or check for them and present users with a confirmation option before they commit to the action.

**Apply when:** The feature involves form input, configuration, data entry, or any action where users can easily make mistakes.

---

## H6: Recognition Rather Than Recall

Minimize the user's memory load by making elements, actions, and options visible. The user should not have to remember information from one part of the interface to another.

**Apply when:** The feature requires users to reference previous information, remember codes/IDs, or navigate between views to complete a task.

---

## H7: Flexibility and Efficiency of Use

Shortcuts -- hidden from novice users -- can speed up the interaction for the expert user so that the design can cater to both inexperienced and experienced users. Allow users to tailor frequent actions.

**Apply when:** The feature will be used repeatedly by power users, or the workflow has steps that could be accelerated or bypassed.

---

## H8: Aesthetic and Minimalist Design

Interfaces should not contain information that is irrelevant or rarely needed. Every extra unit of information in an interface competes with the relevant units of information and diminishes their relative visibility.

**Apply when:** The feature risks information overload, or the design challenge involves presenting dense data, many options, or complex configurations.

---

## H9: Help Users Recognize, Diagnose, and Recover from Errors

Error messages should be expressed in plain language (no error codes), precisely indicate the problem, and constructively suggest a solution.

**Apply when:** The feature involves validation, API calls, permissions, or any interaction where things can go wrong.

---

## H10: Help and Documentation

It may be necessary to provide documentation to help users understand how to complete their tasks. Any such information should be easy to search, focused on the user's task, list concrete steps to be carried out, and not be too large.

**Apply when:** The feature introduces new concepts, has non-obvious functionality, or targets users who may need onboarding or guidance.

---

## Severity Rating Scale

When evaluating heuristic relevance to a design problem, use this scale:

| Rating | Label | Description |
|--------|-------|-------------|
| 0 | Not relevant | This heuristic does not apply to the design problem |
| 1 | Low relevance | Minor consideration, unlikely to cause usability issues |
| 2 | Medium relevance | Moderate consideration, could cause friction if ignored |
| 3 | High relevance | Critical consideration, likely to cause significant usability issues if ignored |
