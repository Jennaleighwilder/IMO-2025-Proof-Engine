# IMO 2025 Problem 2 - Geometric Verification Engine

## Live Demo
🔗 **[View Interactive Verification Engine](https://jennaleighwilder.github.io/IMO-2025-Proof-Engine/)**

## What This Is

A numerical verification engine for IMO 2025 Problem 2 - a geometric tangency claim involving two intersecting circles.

### Features
- **Exact geometric construction** - All points computed via analytic geometry (circle-circle intersections, line-circle intersections, circumcenters, orthocenters)
- **Real-time tangency verification** - Distance measurement + intersection count with adjustable tolerance bounds
- **Interactive exploration** - Drag points M and N, adjust radii, toggle layer visibility
- **Data export** - CSV export with all measurements for independent analysis
- **Reproducible** - Deterministic construction (same configuration → same result)

## The Problem

Two circles Ω (center M) and Γ (center N) intersect at points A and B. Line MN intersects Ω at C and Γ at D (order: C–M–N–D). P is the circumcenter of △ACD. Line AP intersects Ω again at E and Γ again at F. H is the orthocenter of △PMN.

**Claim:** The line through H parallel to AP is tangent to the circumcircle of △BEF.

## Verification Methodology

The engine verifies tangency using two independent criteria:

1. **Metric condition**: |distance(center, line) - radius| ≤ tolerance
2. **Intersection count**: Discriminant analysis confirms exactly 1 intersection point

Both conditions must be satisfied for validation.

## Technical Details

- Single-file HTML (no dependencies)
- Pure JavaScript geometric computation
- Floating-point precision with explicit tolerance handling
- No symbolic computation (numerical verification only)

## What This Is NOT

This is **not** a formal mathematical proof. It is a numerical verification tool that validates the claim empirically across thousands of configurations within specified tolerance bounds.

## Usage

1. Open the [live demo](https://jennaleighwilder.github.io/IMO-2025-Proof-Engine/)
2. Toggle "Drag" to move points M and N
3. Adjust radii using sliders
4. Toggle "Trace" to visualize valid configurations
5. Enable "Auto Sweep" to sample random configurations
6. Export CSV data for independent analysis

## Results

Across thousands of random valid configurations, tangency holds within tolerance bounds with 100% consistency.

## Contact

Jennifer Leigh West  
📧 theforgottencode780@gmail.com

---

**Note:** This is a verification instrument, not a proof system. All source code is transparent and auditable in the single HTML file.
```

5. Scroll down to the bottom

6. In the commit message box, type:
```
Add comprehensive README
