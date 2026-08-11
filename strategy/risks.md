# Key Risks & Mitigations

| Risk | Mitigation |
| --- | --- |
| Otopic dev time stolen by Sapilon emergencies | Ring-fenced engineering hours per week, protected from reallocation. A revenue-percentage rule funds Otopic R&D. |
| One client's needs warping the core product | Microservice isolation + the 3-client promotion rubric ([`./governance.md`](./governance.md)). |
| Pricing model mismatch between segments | Two pricing motions, not one: hosted SaaS (Free/Pro) for SME teams, PAYG (Sovereign) for enterprise. |
| BYOC operational complexity | Heavy investment in deployment automation (Terraform/CDK) **before** scaling the Sovereign tier. |
| Free users diluting the AI-native positioning | Free tier *includes* AI (rate-limited), so every user experiences the differentiator on day one. |
