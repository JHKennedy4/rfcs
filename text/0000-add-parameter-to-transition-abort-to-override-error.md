- Start Date: 2017-10-12
- RFC PR: (leave this empty)
- Ember Issue: (leave this empty)

# Summary

Aborting a transition causes the promise returned by transitionTo to resolve
with a TransitionError. This feature would allow the user to provide an argument
to transition.abort() that will replace TransitionError as the resolved value.

# Motivation

A common reason to abort a transition is an error occurring in the course of the
transition. Currently, information about the failure is lost to the caller.

# Detailed design

This is the bulk of the RFC. Explain the design in enough detail for somebody
familiar with the framework to understand, and for somebody familiar with the
implementation to implement. This should get into specifics and corner-cases,
and include examples of how the feature is used. Any new terminology should be
defined here.

# How We Teach This

What names and terminology work best for these concepts and why? How is this
idea best presented? As a continuation of existing Ember patterns, or as a
wholly new one?

Would the acceptance of this proposal mean the Ember guides must be
re-organized or altered? Does it change how Ember is taught to new users
at any level?

How should this feature be introduced and taught to existing Ember
users?

# Drawbacks

Why should we *not* do this? Please consider the impact on teaching Ember,
on the integration of this feature with other existing and planned features,
on the impact of the API churn on existing apps, etc.

There are tradeoffs to choosing any path, please attempt to identify them here.

# Alternatives

What other designs have been considered? What is the impact of not doing this?

This section could also include prior art, that is, how other frameworks in the same domain have solved this problem.

# Unresolved questions

Optional, but suggested for first drafts. What parts of the design are still
TBD?
