# PL-300 Flashcards

Click each card to flip.

<section class="fc-section" data-fc-title="Prepare the Data">
<div class="flashcard-grid">
<div class="flashcard"><div class="fc-q">Q: When pick DirectQuery over Import?</div><div class="fc-a">A: When data is very large, must be real-time, and source supports DQ - accept perf trade-off.</div></div>
<div class="flashcard"><div class="fc-q">Q: What is query folding?</div><div class="fc-a">A: Power Query pushes M transformations back to the source as a single SQL query.</div></div>
<div class="flashcard"><div class="fc-q">Q: Append vs Merge?</div><div class="fc-a">A: Append stacks rows (UNION); Merge joins columns from related tables.</div></div>
<div class="flashcard"><div class="fc-q">Q: When use Dual storage mode?</div><div class="fc-a">A: In composite models for small dimension tables that may join to either Import or DQ fact tables.</div></div>
<div class="flashcard"><div class="fc-q">Q: Personal vs Standard gateway?</div><div class="fc-a">A: Personal = single user, Import only, sleeps when user logs out. Standard = enterprise, multi-user, supports DQ + Live.</div></div>
<div class="flashcard"><div class="fc-q">Q: Why profile a column?</div><div class="fc-a">A: Spot data quality issues (errors, empties), distribution, distinct values - before modeling.</div></div>
</div>
</section>

<section class="fc-section" data-fc-title="Model the Data">
<div class="flashcard-grid">
<div class="flashcard"><div class="fc-q">Q: Calculated column vs measure?</div><div class="fc-a">A: Calculated column is per-row, stored, good for slicing. Measure is dynamic aggregation, computed at query time.</div></div>
<div class="flashcard"><div class="fc-q">Q: Why a dedicated Date table?</div><div class="fc-a">A: Time intelligence functions require continuous, marked date table. Lets you filter across multiple fact tables.</div></div>
<div class="flashcard"><div class="fc-q">Q: RLS vs OLS?</div><div class="fc-a">A: RLS hides rows by role; OLS hides entire columns/tables by role.</div></div>
<div class="flashcard"><div class="fc-q">Q: When use VAR in DAX?</div><div class="fc-a">A: To compute a value once and reuse - improves readability AND perf.</div></div>
<div class="flashcard"><div class="fc-q">Q: Cross-filter direction default?</div><div class="fc-a">A: Single (from dim 'one' side to fact 'many' side).</div></div>
<div class="flashcard"><div class="fc-q">Q: Star schema benefit?</div><div class="fc-a">A: Simpler model, better compression, single direction filtering, faster queries.</div></div>
<div class="flashcard"><div class="fc-q">Q: How implement role-playing date dim?</div><div class="fc-a">A: Multiple inactive relationships + USERELATIONSHIP() in measures, OR duplicate the Date table.</div></div>
</div>
</section>

<section class="fc-section" data-fc-title="Visualize and Analyze the Data">
<div class="flashcard-grid">
<div class="flashcard"><div class="fc-q">Q: Best visual for trend over time?</div><div class="fc-a">A: Line chart.</div></div>
<div class="flashcard"><div class="fc-q">Q: Best AI visual to identify what drives a KPI?</div><div class="fc-a">A: Key Influencers.</div></div>
<div class="flashcard"><div class="fc-q">Q: Paginated vs interactive reports?</div><div class="fc-a">A: Paginated = multi-page, print-ready, RDL, fixed layout. Interactive = visuals, slicers, drillthrough.</div></div>
<div class="flashcard"><div class="fc-q">Q: How let users print full multi-page list?</div><div class="fc-a">A: Use a paginated report (Power BI Report Builder).</div></div>
<div class="flashcard"><div class="fc-q">Q: Sync slicer purpose?</div><div class="fc-a">A: One slicer affects multiple report pages.</div></div>
<div class="flashcard"><div class="fc-q">Q: Drillthrough use?</div><div class="fc-a">A: Right-click to navigate to a detail page filtered by selection context.</div></div>
</div>
</section>

<section class="fc-section" data-fc-title="Deploy and Maintain Assets">
<div class="flashcard-grid">
<div class="flashcard"><div class="fc-q">Q: Four workspace roles?</div><div class="fc-a">A: Admin, Member, Contributor, Viewer.</div></div>
<div class="flashcard"><div class="fc-q">Q: App vs workspace direct share?</div><div class="fc-a">A: App = curated, polished experience for many end users; workspace = creator/collab space.</div></div>
<div class="flashcard"><div class="fc-q">Q: Max scheduled refreshes Pro vs Premium/PPU?</div><div class="fc-a">A: Pro 8/day. Premium/PPU 48/day.</div></div>
<div class="flashcard"><div class="fc-q">Q: When need an on-prem data gateway?</div><div class="fc-a">A: When dataset source is behind a firewall (on-prem SQL/files) - for both refresh and DirectQuery.</div></div>
<div class="flashcard"><div class="fc-q">Q: Promoted vs Certified content?</div><div class="fc-a">A: Promoted = owner says it's good. Certified = tenant admin/data steward formally endorses.</div></div>
<div class="flashcard"><div class="fc-q">Q: How separate dev / test / prod in Power BI?</div><div class="fc-a">A: Use deployment pipelines (Premium/PPU).</div></div>
</div>
</section>
