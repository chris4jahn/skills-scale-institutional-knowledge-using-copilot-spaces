# OctoAcme — Documentation Guidelines

## Purpose
Ensure user-facing and internal documentation stays accurate, current, and useful throughout the product lifecycle.

---

## Documentation Responsibilities

### Technical Writer
- **Primary Owner** of user-facing documentation (guides, tutorials, FAQs)
- Write and publish release notes for each release
- Maintain documentation templates and style guide
- Review all documentation before releases for accuracy and completeness
- Coordinate with Developers and PM to understand feature details

### Developers
- Document code with inline comments for complex logic
- Write and maintain API documentation (e.g., OpenAPI specs, README files)
- Update technical documentation when implementation changes
- Provide Technical Writer with feature details and technical context
- Review documentation for technical accuracy

### Product Manager
- Define what should be documented based on user needs
- Provide context on feature goals and user value in planning
- Review release notes and user-facing docs for clarity and messaging
- Prioritize documentation updates in the backlog
- Validate that documentation addresses common user questions

### Customer Support Lead
- Provide feedback on gaps in documentation based on support trends
- Suggest FAQ topics and troubleshooting guides
- Review documentation to ensure it addresses common user issues
- Alert Technical Writer and PM to outdated or incorrect documentation

---

## Documentation Lifecycle

### During Planning
- PM and Technical Writer identify documentation needs in project kickoff
- Add documentation tasks to backlog with clear acceptance criteria
- Developers flag API or technical doc changes during design reviews
- Estimate time required for documentation alongside feature work

### During Development
- Developers update code comments and technical docs as they code
- Technical Writer drafts user-facing documentation using feature specs
- UX Designer provides screenshots or workflows for visual documentation
- PM reviews draft documentation for alignment with product messaging

### Before Release
- Technical Writer reviews all documentation for completeness and accuracy
- Developers review API docs and ensure examples work
- QA validates that documentation matches actual feature behavior
- Release Manager includes documentation review in release checklist

### After Release
- Technical Writer publishes release notes and updated documentation
- Customer Support Lead monitors for documentation-related support issues
- PM and Technical Writer track documentation feedback and prioritize updates
- Team reviews documentation effectiveness in retrospectives

---

## Release Notes Template

Use this template for all releases to ensure consistency and completeness.

```markdown
# Release [Version] — [Date]

## Summary
[2-3 sentence overview of the release and its primary goals]

## New Features
- **[Feature Name]**: [Brief description of what users can now do]
- **[Feature Name]**: [Brief description of what users can now do]

## Improvements
- **[Improvement Area]**: [What was enhanced and the user benefit]
- **[Improvement Area]**: [What was enhanced and the user benefit]

## Bug Fixes
- Fixed [issue description] that caused [user impact]
- Resolved [issue description] affecting [specific scenario]

## Breaking Changes
[If none, state "None." Otherwise, list changes that require user action]
- **[API/Feature]**: [What changed and what users need to do]

## Migration Steps
[If none, state "No migration required." Otherwise, provide step-by-step instructions]
1. [Step 1]
2. [Step 2]

## Known Issues
[If none, state "None." Otherwise, list with workarounds if available]
- [Issue description] — Workaround: [If available]

## Documentation
- [Link to updated user guide]
- [Link to API documentation]
- [Link to tutorial or how-to]

## Questions or Feedback?
Contact [support email or link] for assistance.
```

---

## API Documentation Template

Use this template for documenting APIs to ensure consistency and usability.

```markdown
# [API Name] Documentation

## Overview
[Brief description of what this API does and its primary use cases]

## Authentication
[How to authenticate requests — e.g., API key, OAuth, etc.]

## Base URL
```
[Base URL for all endpoints]
```

## Endpoints

### [Method] [Endpoint Path]
[Brief description of what this endpoint does]

**Request**
- **Method**: [GET, POST, PUT, DELETE, etc.]
- **URL**: `[full endpoint path with parameters]`
- **Headers**:
  - `[Header-Name]`: [Description and example value]
- **Query Parameters** (if applicable):
  - `[param_name]` (type, required/optional): [Description]
- **Request Body** (if applicable):
  ```json
  {
    "field_name": "example_value"
  }
  ```

**Response**
- **Success (200)**:
  ```json
  {
    "field_name": "example_value"
  }
  ```
- **Error (4xx/5xx)**:
  ```json
  {
    "error": "Error message"
  }
  ```

**Example**
```bash
curl -X [METHOD] [URL] \
  -H "[Header]: [Value]" \
  -d '[Request Body]'
```

## Error Codes
| Code | Description | Recommended Action |
|------|-------------|-------------------|
| 400  | [Error description] | [What user should do] |
| 401  | [Error description] | [What user should do] |

## Rate Limits
[Describe any rate limiting policies]

## Support
Contact [support email or link] for questions or issues.
```

---

## Best Practices

### Writing Style
- Use clear, concise language — avoid jargon unless it's industry-standard
- Write in active voice and present tense
- Use numbered lists for procedures, bullet points for non-sequential items
- Include code examples and screenshots where helpful

### Maintenance
- Review documentation quarterly or after major releases
- Archive deprecated documentation and clearly mark it as outdated
- Use version control (e.g., Git) to track documentation changes
- Link related documentation to help users navigate

### Accessibility
- Use descriptive link text (avoid "click here")
- Provide alt text for images and diagrams
- Ensure documentation is readable with screen readers
- Use headings and structure to improve navigation

---

## Documentation Checklist

Use this checklist when creating or updating documentation:

- [ ] Purpose and audience clearly defined
- [ ] Information accurate and matches current product behavior
- [ ] Examples tested and working
- [ ] Screenshots current and annotated if needed
- [ ] Links valid and pointing to correct resources
- [ ] Style consistent with existing documentation
- [ ] Reviewed by Developer for technical accuracy
- [ ] Reviewed by PM for messaging and clarity
- [ ] Accessibility guidelines followed
- [ ] Published and discoverable by users
