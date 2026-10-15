# Video Comparison

Website: https://against-wu.github.io/video-comparison/

This page contains only two sections:

- Side-by-side video comparisons, with no upper limit on methods per case, group playback, shared seeking and 1×/2×/4×/8× speed controls.
- VBench-Long metric comparison, with seven core quality dimensions, all sixteen dimensions and three optional aggregate score fields.

The initial videos are labeled animated placeholders. Method A and Method B are placeholder labels. Scores are intentionally empty; no evaluation results are invented.

## Edit

Open https://against-wu.github.io/video-comparison/?edit=1

- Video cases use one State-of-the-Art section. Existing cases from other categories are merged into it.
- Click 编辑视频 to choose videos or enter video URLs. Click 添加对比方法 to add as many methods as needed; videos wrap to keep each player readable.
- Click 编辑指标 to add method names, scores and evaluation settings.
- Scores use the 0–100 percentage scale. Empty cells remain unreported. Total, Quality and Semantic scores must come from your evaluation results and are not calculated by the page.
- Metric CSV files can be exported, edited and imported. Keep the exported column names and percentage scale.
- Click 导出 GitHub 网页 to download the full website ZIP, including local videos and metric data.
- Unzip and commit the files to this repository's main branch. Keep media/ paths intact.

Changes are saved only in the current browser until exported and committed. The ?edit=1 interface edits a local draft; it does not grant repository write access or update the public website directly.

## VBench-Long definitions

Metric names follow the [official VBench-Long implementation](https://github.com/Vchitect/VBench/tree/master/vbench2_beta_long).
The seven core quality dimensions are subject consistency, background consistency, temporal flickering, motion smoothness, dynamic degree, aesthetic quality and imaging quality.
Full evaluation adds object class, multiple objects, human action, color, spatial relationship, scene, appearance style, temporal style and overall consistency.

Use results from comparable evaluation settings (duration, frame rate, resolution, prompt suite and benchmark version). For temporal flickering, the official standard evaluation uses a static filter. Arbitrary custom-input evaluation supports six dimensions; use the official protocol for the remaining dimensions.

## Hosting

GitHub Pages publishes main / (root). The .nojekyll file keeps the static HTML publishing path.
