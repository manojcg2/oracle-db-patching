## Operating Assumptions

- Oracle Home is **patched once per host**
- Databases (SIDs) are discovered dynamically via PMON
- oratab is **not** used for SID discovery
- Multiple databases may share the same Oracle Home
- Oracle environment is injected per task using Ansible `environment`
- RMAN backups are assumed to exist (read-only validation only)

This role does not create or alter databases.
It only orchestrates patch activities defined in the official SOP.