                    ┌─────────────────────┐
                    │     Developer       │
                    └──────────┬──────────┘
                               │
                           Git Push
                               │
                               ▼
                    ┌─────────────────────┐
                    │ GitHub Repository   │
                    │   Source Code       │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │   GitHub Actions    │
                    │    CI/CD Pipeline   │
                    │                     │
                    │ • Build             │
                    │ • Quality Check     │
                    │ • Docker Build      │
                    └──────────┬──────────┘
                               │
                          CI Success
                               │
                               ▼
                    ┌─────────────────────┐
                    │       Render        │
                    │   Cloud Platform    │
                    └──────────┬──────────┘
                               │
                   ┌───────────┴───────────┐
                   ▼                       ▼
          ┌─────────────────┐     ┌─────────────────┐
          │ React Frontend  │     │ Express Backend │
          │                 │     │ Docker/App      │
          └────────┬────────┘     └────────┬────────┘
                   │                       │
                   │              ┌────────▼────────┐
                   │              │ /health        │
                   │              │ Monitoring     │
                   │              └─────────────────┘
                   │
                   ▼
          ┌─────────────────┐
          │      Users      │
          │   Web Browser   │
          └─────────────────┘
