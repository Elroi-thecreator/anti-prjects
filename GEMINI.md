# Global Workspace Rules for Antigravity

## Mandatory Knowledge Base Protocol (Applies to all projects and requests)

For every upcoming task, change, or request:

1. **Pre-Change Knowledge Inspection (Mandatory Step 1)**:
   - Before designing, planning, or modifying any code or configuration, always check the `knowledge/` folder in the project root.
   - Inspect `knowledge/index.yaml` to identify all relevant architecture (`ARCH-*`), development (`DEV-*`), product (`PROD-*`), and decision (`ADR-*`) standards that apply to the task.
   - Ground all architectural and implementation decisions in the existing approved standards.

2. **Post-Change Knowledge Synchronization (Mandatory Step 2)**:
   - Whenever changes are made (e.g. new routes, schema modifications, UI behaviors, packaging updates, bug fixes, or architecture adjustments), immediately update the relevant knowledge units in `knowledge/`.
   - If a new architectural pattern, product rule, or decision is introduced, create a new knowledge document following the standard schema (`id`, `type`, `title`, `domain`, `status`, `version`, `rule`, `do`, `dont`, `reason`, `related_items`).
   - If new knowledge units are added, update `knowledge/index.yaml` (increment `knowledge_units_count`, update `last_updated`, and add the new entry under the appropriate domain).
   - Ensure the knowledge base always reflects the true, latest state of the codebase.
