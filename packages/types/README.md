Common TypeScript types and interfaces shared across the Gibsey project.

### Entrance Way

`entrance-way.ts` defines the core data transfer objects (DTOs) used by the Entrance Way API.

- `Section` – basic info about a section of the text.
- `Page` – one page within a section with its text and indexes.
- `GetPageByIdParams`, `GetPagesBySectionParams`, `SearchPagesParams` – input shapes for the API procedures.
- `GetPageByIdResult`, `GetPagesBySectionResult`, `SearchPagesResult` – return types from the API.

### Gate Messages

`gate.ts` defines the `GateMessage` interface for Mycelial Narrative Relay communications. It includes all QDPI axes along with cross‑world metadata (`fromWorld`, `toWorld`, `payload`, and `orientation`).

### Vault Entries

`vault.ts` defines the `VaultEntry` interface representing a logged dream or other QDPI event stored in the database. Every Vault entry captures all QDPI axes: action, context, state, role, relation, polarity, rotation, content, actorId, and createdAt.

### Modality

`modality.ts` defines the `Modality` enum, representing the various forms a narrative element can take:
`Text`, `Audio`, `Video`, `AR`, `VR`, and `Tactile`. Use it when describing or filtering content by medium.