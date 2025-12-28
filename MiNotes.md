# Terraform CDK (CDKTF) – Sunset Notice & Migration Guide

## Overview

**Cloud Development Kit for Terraform (CDKTF)** is being officially sunset and will be archived on **December 10, 2025**.

After this date:
- The GitHub repository will become **read-only**
- No new features, bug fixes, or compatibility updates will be provided
- The project will remain available under the **Mozilla Public License (MPL)**

HashiCorp (an IBM company) made this decision because CDKTF did not achieve sufficient product-market fit. Future investments will focus on **Terraform core and its broader ecosystem**.

---

## Can You Still Use CDKTF?

Yes — **but at your own risk**.

- The archived source code will remain available
- No security patches or Terraform/provider updates will be released
- Future Terraform versions may break compatibility

Community forks are allowed and encouraged if there is interest in maintaining the project independently.

---

## Recommended Migration Path

### Migrate to Standard Terraform (HCL)

HashiCorp provides a migration command to generate Terraform-compatible HCL files from an existing CDKTF project:

```bash
cdktf synth --hcl
