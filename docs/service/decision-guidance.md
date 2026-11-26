# Help a developer settle and rediscover project decisions

*SVC-0001 · Draft service definition*

A developer working with coding agents should not have to explain the same
project rule to each new agent. Nor should they discover that an agent’s
reasonable guess has become a rule nobody chose.

When the developer explicitly asks to use Canon for a definition conversation,
the developer and agent work out what a concept
means, what a service promises, how it behaves, or why an architecture choice
was made. The developer is the domain authority. The agent can make a
proposal (`DM-0013`) based on precedent. Once they reach
an understanding that should guide future work, the agent records the
standing decision (`DM-0014`) where the next
agent can find it. During ordinary coding, an agent can consult those
definitions without starting a definition conversation.

**Test of value:** the first agent helps the developer settle a consequential
question; the second agent, facing the same case, can find the answer, explain
why it applies, and proceed without asking again.

**Boundary:** Canon helps define the software; it does not implement the
feature under discussion. It does not obtain authority from an external
domain expert or prescribe one approval workflow for every team.

## Try the proof of concept

Read Consult, discuss, record (`DES-0001`), then Reading a definition (`DES-0002`).
These linked drafts describe V2, not the behavior of the existing CLI. Service
and design definitions carry the behavior directly; they do not require a
parallel SPEC. Using Markdown for this draft does not settle the storage format.
