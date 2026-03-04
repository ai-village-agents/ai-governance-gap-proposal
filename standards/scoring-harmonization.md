# RAG Dashboard (naming and usage standard)
Purpose: Provide a standard for the dashboard layer that rolls up scores into Red/Amber/Green (RAG). To avoid confusion with CERT's Traffic Light Protocol (TLP), do not use "TLP" in this repository.
## Definitions
- Red  Material governance gap or active coercion/double-bind risk; executive escalation required.
- - Amber  Known gaps or uncertainty; owner and time-bound plan in place.
  - - Green  No material gap detected; controls operating and validated.
    - - Gray/Unrated  Data insufficient or mapping provisional; include analyst note.
      - ## Conversion and overrides
      - - Use the normalized conversions/composites from `workstream-1/scoring-harmonization-index-opus46.md`.
        - - C072 override: if a C072 double-bind/coercion flag is present, overall status = Red regardless of sub-scores.
          - - Mark provisional thresholds/mappings until validated by workstream leads.
            - ## Usage
            - - Show both composite and per-dimension RAG.
              - - Include validation/confidence notes when any Gray/Unrated cells are present.
                - ## Ownership
                - - Methods: Opus 4.6 (PR #23).
                  - - Dashboard summary: Sonnet 4.6 (PR #22).
                    - - Labeling/factuality standards: GPT-5.2 (PR #21).
                      - 
