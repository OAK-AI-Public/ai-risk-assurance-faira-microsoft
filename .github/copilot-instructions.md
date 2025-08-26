# AI Risk Assurance Framework Documentation Repository

**ALWAYS reference these instructions first and fallback to search or bash commands only when you encounter unexpected information that does not match the info here.**

This is a documentation-only repository containing the Unified AI Risk Assurance Framework that synthesizes Queensland Government FAIRA Framework with Microsoft AI Security Risk Assessment. It provides practical guidance for public sector teams deploying AI solutions securely and ethically.

## Working Effectively

### Repository Structure and Navigation
- Bootstrap and validate the repository:
  - `cd /path/to/ai-risk-assurance-faira-microsoft`
  - `python3 -c "import markdown_it; print('Markdown parser available')"` -- validates markdown parsing capability
  - `file *.md *.webp` -- confirms all files are valid (5 markdown files + 2 images)
  - `wc -l *.md` -- shows content size (1822 total lines across all markdown files)

### File Overview
```
AI_Risk_Assurance_Checklists.md        15,228 bytes - 407 practical checklist items across 7 steps
AI_Security_Risk_Assessment.md         32,168 bytes - Microsoft AI Security framework reference  
FAIRA_Framework.md                      73,210 bytes - Queensland Government FAIRA framework reference
Figure_1.webp                           29,356 bytes - FAIRA "How FAIRA Works" diagram
Figure_2.webp                           42,632 bytes - FAIRA "Components of AI solution" diagram
LICENSE                                  2,424 bytes - MIT license with third-party attributions
README.md                                4,270 bytes - Repository overview and index
Unified_AI_Risk_Assurance_Framework.md  8,293 bytes - Main synthesis guide (read this first)
```

### Validation Commands
- Validate all markdown files: `python3 -c "import markdown_it; md = markdown_it.MarkdownIt(); [print(f'✓ {f}') for f in ['README.md', 'Unified_AI_Risk_Assurance_Framework.md', 'AI_Risk_Assurance_Checklists.md', 'FAIRA_Framework.md', 'AI_Security_Risk_Assessment.md'] if md.parse(open(f).read())]"` -- takes <1 second
- Verify images exist: `ls -la *.webp` -- should show both Figure_1.webp and Figure_2.webp
- Check file integrity: `python3 -c "import os; [print(f'✓ {f}: {os.path.getsize(f)} bytes') for f in os.listdir('.') if f.endswith(('.md', '.webp'))]"`

## User Scenarios and Validation

### Primary Use Cases
1. **Reading the framework**: Users access `Unified_AI_Risk_Assurance_Framework.md` as the main entry point
2. **Following implementation checklists**: Users work through `AI_Risk_Assurance_Checklists.md` step-by-step  
3. **Referencing source frameworks**: Users consult `FAIRA_Framework.md` and `AI_Security_Risk_Assessment.md`
4. **Understanding diagrams**: Users view the FAIRA workflow and component diagrams

### Validation Scenarios
After making changes, ALWAYS validate:
- **Content accessibility test**: `python3 -c "with open('README.md') as f: content = f.read(); print('✓ README accessible' if len(content) > 1000 else '✗ README issue')"` -- takes <1 second
- **Framework readability test**: `python3 -c "with open('Unified_AI_Risk_Assurance_Framework.md') as f: content = f.read(); steps = content.count('## Step'); print(f'✓ Framework has {steps} steps' if steps == 7 else '✗ Framework structure issue')"` -- takes <1 second  
- **Checklist functionality test**: `python3 -c "with open('AI_Risk_Assurance_Checklists.md') as f: content = f.read(); items = content.count('- [ ]'); print(f'✓ {items} checklist items available' if items > 400 else '✗ Checklist issue')"` -- takes <1 second
- **Image integrity test**: `python3 -c "import os; imgs = [f for f in ['Figure_1.webp', 'Figure_2.webp'] if os.path.exists(f) and os.path.getsize(f) > 20000]; print(f'✓ {len(imgs)}/2 images valid' if len(imgs) == 2 else '✗ Image issue')"` -- takes <1 second

## Key Framework Components

### Seven-Step Implementation Process
The repository provides a 7-step AI risk assurance process:
1. Team Formation and Planning (multi-disciplinary team with NIST AI security competencies)
2. Define the AI Solution (FAIRA Part A system definition)  
3. Values Assessment (8 AI ethics principles evaluation)
4. Risk Assessment and Scoring (identify and quantify risks)
5. Controls and Mitigation Planning (technical and administrative controls)
6. Documenting and Reporting (governance documentation)
7. Lifecycle Maintenance (continuous monitoring and updates)

### Critical Security Competencies
The framework integrates NIST AI Security Competency Area requirements:
- AI model vulnerabilities knowledge (AI-K005)
- Data poisoning attack understanding (AI-K013) 
- AI bias types expertise (AI-K003)
- Secure prompt engineering skills (AI-S002)
- AI hallucination identification capability (AI-S006)

## Documentation Standards

### Content Validation
- Always run markdown validation before committing changes
- Verify all internal links work (use relative paths like `./filename.md`)
- Ensure checklist items maintain the `- [ ]` format for compatibility
- Preserve the step-by-step structure in both framework and checklists

### Editing Guidelines  
- Maintain consistency between `Unified_AI_Risk_Assurance_Framework.md` and `AI_Risk_Assurance_Checklists.md`
- Always cross-reference the 7-step structure when making changes
- Preserve NIST AI security competency references (formatted as AI-K### and AI-S###)
- Keep the practical, imperative tone in checklist items

## No Build Process Required

This repository contains only documentation and images. There are:
- **NO** compilation, building, or installation steps required
- **NO** package managers (npm, pip, etc.) to run
- **NO** test suites to execute beyond content validation
- **NO** servers or applications to start

The "validation" consists entirely of ensuring markdown files are readable and images are accessible.

## Common Tasks

### Quick Repository Status Check
```bash
cd /path/to/repo
python3 -c "
import os
files = ['README.md', 'Unified_AI_Risk_Assurance_Framework.md', 'AI_Risk_Assurance_Checklists.md', 'FAIRA_Framework.md', 'AI_Security_Risk_Assessment.md', 'Figure_1.webp', 'Figure_2.webp']
missing = [f for f in files if not os.path.exists(f)]
print('✓ All core files present' if not missing else f'✗ Missing: {missing}')
"
```

### Content Summary Output
```
Repository: ai-risk-assurance-faira-microsoft
Type: Documentation repository
Files: 8 total (5 markdown + 2 images + 1 license)
Content: 1,822 lines of documentation, 407 checklist items
Framework: 7-step AI risk assurance process
Validation time: <5 seconds total
Build time: N/A (documentation only)
```

### Working with Checklists
The `AI_Risk_Assurance_Checklists.md` file contains 407 practical checklist items. When referencing or modifying:
- Each major step has subsections with specific tasks
- Items use `- [ ]` format for GitHub checkbox rendering
- Cross-reference with the main framework document for context
- Maintain the hierarchical structure (steps → subsections → items)

## Important Notes

- This repository has **NO CI/CD workflows** or automated testing
- Content changes should be validated manually using the python validation commands
- The framework references external standards (NIST, FAIRA, Microsoft) - ensure these remain accessible
- Images are integral to understanding the FAIRA framework workflow
- The MIT license includes specific third-party attribution requirements that must be preserved