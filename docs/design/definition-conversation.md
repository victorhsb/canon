# Consult, discuss, record

*DES-0001 · Draft design for Decision guidance (`SVC-0001`)*

Only the user can start this workflow. “Let’s use Canon to define how Canon
handles proposals” invokes it. “Let’s define how Canon handles proposals”
names Canon as the subject, not the tool: it does not invoke the workflow.
An agent may read definitions during ordinary work but must not start this
conversation or record decisions on its own.

1. **Consult.** Read the definitions that bear on the question. Code and tests
   can establish what happens today; neither proves the developer wants it to
   keep happening. If a definition already settles this case, explain how it
   applies and stop. There is nothing new to record.
2. **Discuss the difference that matters.** When precedent points one way,
   draft a proposal (`DM-0013`) and show the precedent
   so the developer can correct or veto it. When the evidence supports two
   materially different answers, ask the question that distinguishes them.
   If the request conflicts with a settled definition, show the consequence
   before changing anything. Leave unresolved proposals open.
3. **Record the understanding.** Update the definition that owns the answer;
   create one only if none fits. “Yes, use that for future reviews” is enough:
   show the resulting edit rather than asking the developer to approve the
   same standing decision (`DM-0014`) twice.
   If it is unclear whether the answer was just for this task, ask. Define
   terms by default when two plausible readings would lead to different work.
   Connect the definitions that use them; Domain supplies meaning, not a
   mandatory parent for every record.

**Canon designing itself:** After invoking Canon, a developer asks whether reading a service should
also show designs that refer to it. The agent drafts an example with a
“Referenced by” footer. “Show incoming references on reads” settles the
behavior in Reading a definition (`DES-0002`). It does not
settle the footer’s position, the CLI syntax, or how links are stored. A later
agent asked whether incoming references are visible should consult that design,
not pose the question again.
