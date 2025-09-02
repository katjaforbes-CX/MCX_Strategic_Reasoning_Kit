# Create a Machine-Readable Enterprise Value Proposition File for AI Procurement Systems

You are tasked with creating a JSON file that makes your B2B business easily discoverable and evaluable by enterprise AI procurement systems, autonomous buying platforms, and AI-powered vendor management systems. This file helps procurement algorithms quickly assess whether your business meets their requirements for vendor evaluation, RFP responses, and ongoing supplier relationships.

## Instructions

**Step 1: Analyze the Business**
Visit the business website URL provided and extract key information about:
- Products/services offered to enterprise customers
- Enterprise customer segments and use cases
- Pricing models (subscription, enterprise, custom)
- Compliance certifications and security credentials
- Integration capabilities and API availability
- Support and service level commitments
- Company scale indicators (employee count, revenue range, customer count)

**Step 2: Generate the JSON File**
Create a JSON file named `enterprise-vp.json` with the following structure:

```json
{
  "schema_version": "1.0",
  "last_updated": "[TODAY'S DATE]",
  "business_info": {
    "name": "[Company Name]",
    "description": "[Clear enterprise value proposition]",
    "primary_category": "[e.g., 'saas_software', 'professional_services', 'manufacturing', 'technology_infrastructure']",
    "sub_categories": ["category1", "category2"],
    "website": "[Website URL]",
    "headquarters": "[Location]",
    "founded_year": "[Year or 'not_available']"
  },
  "enterprise_profile": {
    "employee_count_range": "[e.g., '51-200', '1000+', 'not_disclosed']",
    "revenue_range": "[e.g., '$10M-$50M', '$100M+', 'not_disclosed']",
    "customer_count_range": "[e.g., '100-500', '1000+', 'not_available']",
    "years_in_business": "[Number or 'not_available']",
    "business_model": "[e.g., 'SaaS', 'Professional Services', 'Product Sales', 'Hybrid']"
  },
  "value_proposition": {
    "core_value": "[Primary business value in measurable terms]",
    "target_industries": ["industry1", "industry2"],
    "target_company_sizes": ["SME", "Enterprise", "Mid-market"],
    "key_benefits": [
      {
        "benefit": "[Specific benefit]",
        "quantified_impact": "[ROI, time savings, cost reduction with numbers]",
        "proof_point": "[Case study, metric, or validation]"
      }
    ],
    "competitive_differentiators": ["differentiator1", "differentiator2"]
  },
  "products_services": {
    "primary_offerings": [
      {
        "name": "[Product/Service Name]",
        "category": "[Category]",
        "description": "[Brief description]",
        "pricing_model": "[e.g., 'subscription', 'per_user', 'enterprise_contract', 'custom']"
      }
    ],
    "pricing_transparency": "[e.g., 'public_pricing', 'tiered_pricing', 'custom_only', 'not_disclosed']",
    "contract_terms": {
      "minimum_contract_length": "[e.g., 'monthly', '1_year', 'varies']",
      "enterprise_discounts": "[available/not_available/unknown]",
      "volume_pricing": "[available/not_available/unknown]"
    }
  },
  "compliance_security": {
    "security_certifications": ["ISO27001", "SOC2", "etc"],
    "compliance_frameworks": ["GDPR", "HIPAA", "SOX", "etc"],
    "data_residency_options": ["US", "EU", "Multi-region", "not_specified"],
    "security_audit_frequency": "[annual/quarterly/not_specified]"
  },
  "technical_capabilities": {
    "api_availability": "[public_api/partner_api/custom_integration/none]",
    "integration_options": ["REST_API", "SOAP", "Webhooks", "Third_party_platforms"],
    "supported_platforms": ["Web", "Mobile", "Desktop", "API_only"],
    "uptime_sla": "[percentage or 'not_specified']",
    "scalability": "[enterprise_grade/scalable/limited/unknown]"
  },
  "support_services": {
    "support_tiers": ["basic", "premium", "enterprise"],
    "support_channels": ["email", "phone", "chat", "dedicated_rep"],
    "response_time_sla": {
      "critical": "[time or 'not_specified']",
      "standard": "[time or 'not_specified']"
    },
    "professional_services": "[available/not_available/unknown]",
    "training_programs": "[available/not_available/unknown]"
  },
  "procurement_readiness": {
    "rfp_response_capability": "[yes/no/unknown]",
    "vendor_portal_participation": "[yes/no/unknown]",
    "references_available": "[yes/no/unknown]",
    "pilot_program_available": "[yes/no/unknown]",
    "procurement_team_contact": "[available/not_available]"
  },
  "trust_signals": {
    "client_testimonials": "[available/not_available]",
    "case_studies": "[available/not_available]",
    "industry_awards": ["award1", "award2", "none_listed"],
    "analyst_recognition": ["Gartner", "Forrester", "none_listed"],
    "notable_enterprise_clients": ["client1", "client2", "not_disclosed"],
    "financial_backing": "[public_company/private_equity/vc_funded/bootstrapped/unknown]"
  },
  "risk_assessment": {
    "business_continuity_plan": "[documented/not_available/unknown]",
    "disaster_recovery": "[available/not_available/unknown]",
    "insurance_coverage": "[professional_liability/cyber/general/unknown]",
    "regulatory_compliance": "[current/not_applicable/unknown]"
  }
}
```

**Step 3: Handle Missing Information**
If certain information isn't available from the website scan:
- Use `"not_available"` for data not found on the website
- Use `"unknown"` for technical capabilities that can't be verified
- Use `"not_specified"` for policies or SLAs not clearly stated
- Use `"not_disclosed"` for information companies typically keep private

**Step 4: Output the Complete File**
Present the complete JSON file, followed by a section titled "## Enterprise Information Gaps" that lists critical B2B details that should be added manually for optimal procurement system evaluation.

## File Placement Instructions

1. **Save the file as:** `enterprise-vp.json`
2. **Place in root directory** (same level as your main website files)
3. **Make it discoverable** by adding this line to your robots.txt file:
   ```
   # Enterprise procurement file
   Allow: /enterprise-vp.json
   ```
4. **Consider adding to common procurement paths:**
   - Link from `/vendor` or `/partners` pages
   - Include in RFP response templates
   - Reference in vendor portal submissions

## Example Usage

**Input:** Please analyze https://example-enterprise-software.com and create an enterprise-vp.json file

**Expected Output:** Complete JSON file + list of enterprise-specific information to verify/add manually

---

*This format is optimized for enterprise AI procurement systems, vendor management platforms, and autonomous B2B buying systems that need to quickly evaluate supplier capabilities, compliance, and fit for enterprise requirements.*