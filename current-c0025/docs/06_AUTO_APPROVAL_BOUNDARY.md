# C0025 AUTO-APPROVAL BOUNDARY

The C0024 visual direction is approved for continued reversible design work.

Automatic approval may advance to the next review Candidate only when:

- the direct parent and rollback reference are locked,
- static and scope-specific visual tests pass,
- prices, service IDs, product scope, policy and payment behavior do not change,
- no new regression is found,
- the change remains reversible,
- all unexecuted Runtime and user tests remain explicitly UNVERIFIED.

Automatic approval does not promote a Candidate to Active Control, deploy, commit, push, delete files, or change pricing, policy, payment or business identity. Those actions retain their existing explicit gates.
