# GXV-HTF-Profiler

GXV HTF PROFILER

HTF Profiler is a higher-timeframe analysis toolkit built to bring the context needed for profiling and framing entry models into one place.

Rather than stacking multiple tools across the chart, the profiler combines higher-timeframe structure, liquidity, imbalance, correlation and entry-model context into a single workflow.

It is designed as an analytical framework, not a signal generator.


HTF PROFILER

At the core of the indicator are three configurable HTF panes that reconstruct and display higher-timeframe candles directly alongside the execution chart.

Each profiler can display:

HTF candles
Liquidity sweeps
C1 / C2 / C3 sequencing
HTF Fair Value Gaps
HTF SMT
PSP
Candle timers
Relevant HTF information

The three panes can either be configured manually or handled automatically according to the active chart timeframe.


AUTO HTF & TIMEFRAME SEQUENCING

The automated timeframe system is designed to remove the repetitive process of manually changing HTF references when moving between execution timeframes.

Auto HTF dynamically assigns the appropriate higher-timeframe structure based on the active chart timeframe.

Auto Count adjusts the amount of HTF candle history displayed.

The profiler also supports two sequencing frameworks:

Classic Sequence
GXT Sequence

Auto Sequence automatically manages the active sequencing framework, while full manual control remains available when a fixed HTF structure is preferred.


HTF LIQUIDITY SWEEPS

Liquidity sweeps are detected directly from the reconstructed HTF candles.

A high sweep occurs when the following HTF candle trades above the previous candle's high and closes back below it.

A low sweep occurs when the following HTF candle trades below the previous candle's low and closes back above it.

Sweeps can be displayed:

Inside the HTF panes
Directly on the main chart
On both simultaneously

Historical sweep rendering can also be limited to keep the chart focused on the most relevant structures.


C1 / C2 / C3 PROFILING

Valid HTF structures can be organized into C1, C2 and C3 sequences directly inside the profiler.

This provides a visual representation of the higher-timeframe structure surrounding a liquidity event without requiring a separate HTF chart.

Optional equilibrium levels are also available for the corresponding structure.


HTF FAIR VALUE GAPS

Fair Value Gaps are detected directly from the reconstructed candles of each HTF pane.

This keeps the imbalance visually connected to the exact higher timeframe and candle structure from which it originated.

Bullish and bearish HTF FVGs can be configured independently.


HTF SMT

HTF SMT is calculated using the same higher-timeframe candles displayed inside the profiler.

The engine compares synchronized HTF periods across correlated markets and identifies divergence between equivalent structures.

Bullish and bearish SMT relationships are rendered directly inside their corresponding HTF pane, keeping correlation context attached to the structure being profiled.


PSP

PSP extends the HTF correlation framework by combining SMT divergence with the directional relationship between the corresponding HTF candle bodies.

PSP conditions can be represented through:

Directional markers
HTF candle coloring

This allows the condition to remain visible without adding unnecessary structures to the chart.


MULTI-TIMEFRAME SMT

Alongside HTF SMT, the indicator includes a broader multi-timeframe SMT engine for cross-market divergence analysis.

Supported SMT timeframes include:

15m
30m
1H
90m
4H
6H
7H
12H
1D
1W
1M
3M
12M

The correlation system can automatically resolve supported comparison markets and operate through:

Dyad
Triad
Tetrad

Both Classic and GXT correlation modes are available.

SMT rendering also includes configurable timeframe filtering, labeling, historical limits and cleanup logic to reduce redundant structures.


AUTO SMT

When Auto SMT is enabled, the active intraday SMT framework follows the profiler's current HTF sequence.

This allows the correlation framework to remain synchronized with the higher-timeframe structure being profiled without requiring individual SMT timeframes to be managed manually.


SMT-FILL & ON-CHART FVG

The integrated SMT-Fill framework combines on-chart Fair Value Gaps with cross-market correlation.

It can:

Detect bullish and bearish FVGs
Track mitigated and filled gaps
Extend FVGs to their relevant interaction
Filter correlated FVG structures
Display SMT-Fill relationships
Control the amount of historical structures displayed

This keeps imbalance and correlation analysis within the same entry-model environment.


CISD

The profiler includes an integrated CISD framework connected directly to the HTF sweep and C2 structure.

CISD candidates are managed through their own confirmation, displacement and invalidation lifecycle.

Available display modes include:

All
High Probability

An optional Early CISD mode can also display developing conditions before confirmation.

Confirmed CISD structures require confirmed chart bars, while Early CISD is intentionally provisional and may develop as the current candle trades.


BIAS ENGINE

The Bias Engine provides an optional directional layer for the profiler.

Available modes include:

Off
Auto
Auto + Unbiased SMTs
Bullish
Bearish

In Auto mode, the active HTF panes contribute directional information from their current structure and the profiler evaluates agreement between them.

The bias framework acts primarily as a presentation and filtering layer rather than removing the underlying opposite-direction detections.

Auto + Unbiased SMTs preserves the automatic HTF bias while allowing SMT structures from both directions to remain visible.


KEY LEVELS

Previous-period reference levels can also be projected directly onto the chart.

Supported reference periods include:

4H
6H
7H
Daily

Available levels include:

Previous High
Previous Low
Previous Equilibrium

Daily references are displayed as PDH, PDL and PD-EQ.


STATUS TABLE

An optional status table provides a compact overview of the profiler's current state, including:

Active model
Current bias
Automation state
Correlated assets

The purpose is to keep the current framework visible without repeatedly opening the indicator settings.


CUSTOM DAILY OPEN

For models using a non-standard daily boundary, the profiler also provides custom daily-open handling.

Daily HTF processing can be aligned to:

Midnight
18:00 New York time


CUSTOMIZATION

Most components can be configured or disabled independently.

This includes:

HTF candle appearance
Pane positioning and spacing
Candle width
Sweep history
Labels
Timers
FVG rendering
SMT presentation
CISD rendering
Key levels
Status table

The profiler can therefore be used as a complete framework or reduced to only the tools relevant to a particular model or workflow.


IMPORTANT

HTF Profiler works with live higher-timeframe data.

Structures derived from an HTF candle that is still forming can naturally develop as that candle trades. Features requiring confirmation are handled separately from provisional or developing states.

The indicator is intended as an analytical and profiling framework rather than a standalone buy or sell signal.

Execution criteria, market context and risk management remain at the discretion of the trader.


OPEN SOURCE

HTF Profiler is completely free and open-source.

This is the first public release, not the end of its development. Further refinements and additions are planned as the framework continues to evolve.

If you encounter a bug or an edge case, feel free to report it together with the symbol, timeframe and an example of the affected structure.
