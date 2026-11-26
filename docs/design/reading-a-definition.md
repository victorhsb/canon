# Reading a definition

*DES-0002 · Draft design for Decision guidance (`SVC-0001`)*

When an agent fetches a definition, it gets the definition and enough context
to navigate one step in either direction: which domain terms it uses, and
which other records refer to it. A disambiguation link answers a different
question: “Which of these meanings fits here?” It explains the distinction,
not just the title of a neighboring record.

For example, a fetch of **Proposal** in this draft could include the following
note after its definition:

| Relationship | Related definition | Why it is here |
| --- | --- | --- |
| Distinguish from | Standing decision (`DM-0014`) | Proposed answers can be vetoed; settled answers guide later work. |
| Referenced by | Decision guidance (`SVC-0001`) | The service promises that precedent alone will not become a rule. |
| Referenced by | Consult, discuss, record (`DES-0001`) | The workflow shows when to offer a proposal rather than ask an open question. |

Conversely, a fetch of **Decision guidance** shows **Proposal** and **Standing
decision** under “Uses.” The reader can follow either term to its meaning.
The service author does not maintain a second list on each term. A passing use
of the same word in an unrelated sense does not create a domain link.

These are illustrative excerpts of a V2 read, not output from today’s CLI or
a proposed wire format. The design concerns the relationships visible to the
reader, not whether they are stored in Markdown or a database.
