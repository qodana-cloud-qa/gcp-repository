# 🏰 Global Configuration repository examples

Requirements (the needs/goals which it should achieve)
- Multiple Global configurations
- One “Global Configuration” is an organization-level entity
- “Global Configuration” has multiple projects linked to it, specified in QDCL UI
- There could be multiple “global configuration” repositories
- Repository structure is independent of “weak server” or “strong server”
- One “Global configuration” should be able to inherit some properties from the other configuration
- Example in `/sample-1-yaml`
    - `/global-base` (qodana.yaml with quality gates, base flexinspect, base profiles)
    - `/intellij-products` (inherit profiles and qodana.yaml from global-base, include flexinspect from base)
    - `/ai-products` (inherit profiles and qodana.yaml from global-base, include flexinspect from base)
    - `global-configuration.yaml` defines the list of configurations