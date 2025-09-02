# Create a Machine-Readable Value Proposition File for AI Agents

You are tasked with creating a JSON file that makes your B2C business easily discoverable and understandable to AI agents like ChatGPT, Claude, and autonomous shopping assistants. This file will help AI agents quickly evaluate whether your business matches their user's needs and can make confident recommendations.

## Instructions

**Step 1: Analyze the Business**
Visit the business website URL provided and extract key information about:
- What the business sells (products/services)
- Target customer segments
- Key value propositions and benefits
- Pricing information (if available)
- Special features or differentiators

**Step 2: Generate the JSON File**
Create a JSON file named `agent-vp.json` with the following structure:

```json
{
  "schema_version": "1.0",
  "last_updated": "[TODAY'S DATE]",
  "business_info": {
    "name": "[Business Name]",
    "tagline": "[One-line description]",
    "primary_category": "[e.g., 'retail_fashion', 'food_delivery', 'health_wellness']",
    "website": "[Website URL]"
  },
  "value_proposition": {
    "core_value": "[Primary benefit in clear, measurable terms]",
    "target_segments": ["segment1", "segment2"],
    "key_benefits": [
      {
        "benefit": "[Specific benefit]",
        "quantified": "[Metric if available, e.g., '30% faster', '$50 savings']"
      }
    ]
  },
  "products_services": {
    "categories": ["category1", "category2"],
    "price_range": {
      "min": "[Lowest price or 'varies']",
      "max": "[Highest price or 'varies']",
      "currency": "[Currency code]"
    },
    "availability": {
      "geographic": ["region1", "region2"],
      "delivery_options": ["shipping", "pickup", "digital"],
      "typical_fulfillment": "[e.g., '2-3 days', 'instant', '24 hours']"
    }
  },
  "trust_signals": {
    "certifications": ["certification1", "certification2"],
    "guarantees": ["guarantee1", "guarantee2"],
    "social_proof": {
      "review_count": "[number or 'not_available']",
      "average_rating": "[rating or 'not_available']",
      "notable_customers": ["customer1", "customer2"]
    }
  },
  "agent_optimization": {
    "api_available": false,
    "bulk_ordering": "[true/false/unknown]",
    "real_time_inventory": "[true/false/unknown]",
    "structured_data_present": "[true/false - check for schema.org markup]"
  },
  "contact_methods": {
    "customer_service": "[phone/email/chat/not_available]",
    "agent_contact": "[if special agent contact method available]",
    "business_hours": "[hours or 'not_specified']"
  }
}
```

**Step 3: Handle Missing Information**
If certain information isn't available from the website scan:
- Use `"not_available"` for missing data points
- Use `"unknown"` for technical capabilities you can't verify
- Use `"not_specified"` for policies or details not clearly stated

**Step 4: Output the Complete File**
Present the complete JSON file, followed by a section titled "## Missing Information" that lists any key details that should be added manually.

## File Placement Instructions

1. **Save the file as:** `agent-vp.json`
2. **Place in root directory** (same level as your main index.html)
3. **Make it discoverable** by adding this line to your robots.txt file:
   ```
   # Agent value proposition file
   Allow: /agent-vp.json
   ```

## Example Usage

**Input:** Please analyze https://example-store.com and create an agent-vp.json file

**Expected Output:** Complete JSON file + list of information to verify/add manually

---

*This format follows emerging standards for machine-readable business information and is optimized for AI agents that need to quickly evaluate businesses for their users.*