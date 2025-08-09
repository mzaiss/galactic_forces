# galactic_forces

https://mzaiss.github.io/galactic_forces/

## Physics Implementation

**Integrator**: Leapfrog algorithm for numerical integration of Newton's equations of motion. This symplectic integrator preserves energy better than Euler methods for long-term simulations.

**Assumptions**:
- Point masses with no internal structure
- Central forces only (no angular momentum transfer)
- Force cutoff at 4×planet radius to prevent extreme accelerations, no collisions
- Constant mass (no accretion or evaporation)
- Isolated system (no external forces)

**Limits**:
- Energy and Momentum is not well preserved due to simple integrator
- Longer simulations become unrealistic espacially for 1/r^x laws.

**Force Laws**: 1/r³, 1/r², 1/r, constant, log(r), √r, r, r², r³. Forces are normalized by the corner planet to maintain consistent time scales across different laws.
