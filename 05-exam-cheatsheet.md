# PL-300 Exam Cheatsheet

Quick-reference highlights. Skim before the exam.

- Storage modes: Import (in-memory) / DirectQuery (live to source) / Dual / Live (semantic model).
- Query folding = push transforms to source as SQL (preserve at all costs).
- Star schema = facts in middle, dimensions radiating. Best perf + compression.
- Cross-filter direction default = Single (dim -> fact). Both only for many-to-many.
- Calc column = per row + stored. Measure = dynamic aggregation by filter context.
- Need a marked Date table for time intelligence (DATEADD, TOTALYTD).
- VAR = compute once, reuse - readability and perf.
- RLS = rows by role. OLS = columns/tables by role.
- Performance Analyzer reveals slow visuals + DAX timing.
- Visual choice: line=trend, bar=compare cats, scatter=correlate, pie<=5 slices.
- Bookmarks capture state (filters, selection, visibility) for storytelling.
- Drillthrough passes context to detail page.
- Paginated reports = print/PDF/multi-page (Power BI Report Builder, RDL).
- Workspace roles: Admin > Member > Contributor > Viewer.
- App = polished release. Workspace = build/collab area.
- Pro: 8 refreshes/day. Premium/PPU: 48.
- Standard gateway = prod, multi-user, supports DQ. Personal = single user, Import only.
- Promoted = owner endorsement. Certified = central authority (admin) endorsement.
- Deployment pipelines: Dev -> Test -> Prod (Premium / PPU).
