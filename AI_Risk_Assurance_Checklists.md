# AI Risk Assurance Framework - Practical Checklists

## Step 1: Team Formation and Planning Checklist

### Team Assembly

- [ ] Appoint executive sponsor/senior responsible officer
- [ ] Recruit technical lead (AI/ML engineer or data scientist)
- [ ] Assign data architect/engineer
- [ ] Include legal/privacy officer
- [ ] Add records management specialist
- [ ] Include ethics advisor/officer
- [ ] Assign business/operational owner
- [ ] Include risk management professional
- [ ] Add security specialist
- [ ] Include evaluation/testing lead
- [ ] Consider HR/WHS representative for workforce impacts

### Planning Activities

- [ ] Schedule initial kickoff meeting
- [ ] Define team roles and responsibilities (RACI matrix)
- [ ] Set meeting cadence (weekly/fortnightly)
- [ ] Create project timeline with key milestones
- [ ] Book workshop sessions for:
  - [ ] Systems scoping session
  - [ ] Stakeholder mapping workshop
  - [ ] Values and ethics assessment
  - [ ] Risk identification workshop
  - [ ] Control planning session
- [ ] Establish communication channels (Teams, email lists, etc.)
- [ ] Create shared document repository
- [ ] Define decision-making process
- [ ] Set escalation pathways

---

## Step 2: Define the AI Solution Checklist

### FAIRA Part A Documentation

- [ ] Complete Table 1: Solution Overview
  - [ ] Solution name and description
  - [ ] Purpose and objectives
  - [ ] Expected benefits
- [ ] Complete Table 2: Component Architecture
  - [ ] List all AI/ML models
  - [ ] Document algorithms used
  - [ ] Identify third-party components
  - [ ] Map system integrations
- [ ] Complete Table 3: Interfaces
  - [ ] User interfaces (web, mobile, API)
  - [ ] System interfaces
  - [ ] Data exchange points
- [ ] Complete Table 4: Data Sources
  - [ ] Internal data sources
  - [ ] External data feeds
  - [ ] Training data origins
  - [ ] Real-time data inputs
- [ ] Complete Table 5: Data Types
  - [ ] Personal information
  - [ ] Sensitive/classified data
  - [ ] Business data
  - [ ] Public data
- [ ] Complete Table 6: Outputs
  - [ ] Predictions/recommendations
  - [ ] Reports/dashboards
  - [ ] Automated actions
  - [ ] Decision support outputs
- [ ] Complete Table 7: Users and Stakeholders
  - [ ] Primary users
  - [ ] Secondary users
  - [ ] Affected parties
  - [ ] System administrators
- [ ] Complete Table 8: Governance Structure
  - [ ] Oversight committees
  - [ ] Approval processes
  - [ ] Review cycles
- [ ] Complete Table 9: Related Systems
  - [ ] Dependencies
  - [ ] Downstream systems
  - [ ] Integration points

### Technical Security Controls

- [ ] Define Role-Based Access Control (RBAC) requirements
- [ ] Plan model versioning strategy
- [ ] Design input sanitisation approach
- [ ] Establish data integrity validation methods
- [ ] Map API endpoints and security requirements
- [ ] Identify sensor inputs and validation needs
- [ ] Document deployment vectors and security

### WHS Considerations

- [ ] Assess impact on worker autonomy
- [ ] Evaluate changes to task load/complexity
- [ ] Identify role redundancy risks
- [ ] Document potential for harm from system errors
- [ ] Assess training requirements
- [ ] Consider fatigue/stress from AI interaction
- [ ] Complete FAIRA Tables 2.2 and 2.3 for WHS impacts

---

## Step 3: Values Assessment Checklist

### For Each of the 8 AI Ethics Principles

#### 1. Human, Social and Environmental Wellbeing

- [ ] Document intended wellbeing benefits
- [ ] Identify wellbeing risks
- [ ] Plan mitigation measures
- [ ] Consider environmental impacts
- [ ] Assess social equity implications

#### 2. Human-Centred Values

- [ ] Define human rights considerations
- [ ] Document respect for human dignity
- [ ] Identify value conflicts
- [ ] Plan value alignment measures

#### 3. Fairness

- [ ] Assess bias risks in data
- [ ] Evaluate algorithmic fairness
- [ ] Document discrimination risks
- [ ] Plan fairness testing approach
- [ ] Define fairness metrics

#### 4. Privacy Protection and Security

- [ ] Complete Privacy Impact Assessment reference
- [ ] Document data minimisation approach
- [ ] Define consent mechanisms
- [ ] Plan security controls
- [ ] Address data retention/disposal

#### 5. Reliability and Safety

- [ ] Define safety requirements
- [ ] Document failure modes
- [ ] Plan testing approach
- [ ] Establish performance metrics
- [ ] Create incident response plan

#### 6. Transparency and Explainability

- [ ] Document explanation requirements
- [ ] Plan user communication
- [ ] Define audit trail needs
- [ ] Create transparency notices
- [ ] Design explainability features

#### 7. Contestability

- [ ] Design appeal processes
- [ ] Document review mechanisms
- [ ] Create feedback channels
- [ ] Define human override options
- [ ] Establish complaint procedures

#### 8. Accountability

- [ ] Define responsibility matrix
- [ ] Document decision rights
- [ ] Establish audit processes
- [ ] Create governance structure
- [ ] Plan compliance monitoring

### Legislative Compliance

- [ ] Review Work Health and Safety Act 2011 (Qld) requirements
- [ ] Check Human Rights Act 2019 (Qld) compliance
- [ ] Verify Public Sector Ethics Act 1994 alignment
- [ ] Document other relevant legislation

### Human-Machine Interaction

- [ ] Assess psychological impacts
- [ ] Evaluate ergonomic considerations
- [ ] Plan mental wellbeing supports
- [ ] Design safe interaction patterns

---

## Step 4: Risk Assessment and Scoring Checklist

### Risk Register Creation

- [ ] Create risk register template with fields for:
  - [ ] Risk ID and description
  - [ ] Category (technical, ethical, operational, WHS)
  - [ ] Severity rating (1-5)
  - [ ] Likelihood rating (1-5)
  - [ ] Impact assessment
  - [ ] Risk owner
  - [ ] Current controls
  - [ ] Proposed controls
  - [ ] Residual risk rating

### Risk Identification

- [ ] Technical risks:
  - [ ] Model performance degradation
  - [ ] Data quality issues
  - [ ] System availability
  - [ ] Integration failures
  - [ ] Scalability concerns
- [ ] Security risks (using Microsoft's threat matrix):
  - [ ] Model inversion attacks
  - [ ] Data poisoning
  - [ ] Adversarial inputs
  - [ ] Model theft
  - [ ] Privacy breaches
  - [ ] Evasion attacks
- [ ] Ethical risks:
  - [ ] Bias and discrimination
  - [ ] Privacy violations
  - [ ] Transparency gaps
  - [ ] Autonomy impacts
- [ ] Operational risks:
  - [ ] Process disruption
  - [ ] Resource constraints
  - [ ] Change management
  - [ ] Skills gaps
- [ ] WHS risks:
  - [ ] Physical safety
  - [ ] Psychological harm
  - [ ] Ergonomic issues
  - [ ] Workload impacts

### Risk Scoring

- [ ] Apply severity ratings based on:
  - [ ] Harm to life/safety
  - [ ] Infrastructure damage
  - [ ] Data compromise scale
  - [ ] Financial impact
  - [ ] Reputation damage
- [ ] Apply likelihood ratings based on:
  - [ ] Model exposure
  - [ ] Endpoint availability
  - [ ] Data provenance
  - [ ] Historical incidents
  - [ ] Threat intelligence
- [ ] Calculate risk scores (Severity × Likelihood)
- [ ] Prioritise risks by score
- [ ] Define risk appetite thresholds
- [ ] Document accepted risks with justification
- [ ] Identify risks requiring escalation

---

## Step 5: Controls and Mitigation Planning Checklist

### Technical Controls

- [ ] Encryption:
  - [ ] Data at rest encryption
  - [ ] Data in transit encryption
  - [ ] Model encryption
  - [ ] Key management plan
- [ ] Access controls:
  - [ ] Authentication mechanisms
  - [ ] Authorisation framework
  - [ ] Privileged access management
  - [ ] Session management
- [ ] Input validation:
  - [ ] Input sanitisation rules
  - [ ] Data type validation
  - [ ] Range checking
  - [ ] Format validation
- [ ] Model security:
  - [ ] Adversarial training approach
  - [ ] Model hardening techniques
  - [ ] Version control system
  - [ ] Model signing/verification
- [ ] Monitoring:
  - [ ] Security event logging
  - [ ] Anomaly detection
  - [ ] Performance monitoring
  - [ ] Audit trail implementation

### Policy Controls

- [ ] Privacy Impact Assessment completion
- [ ] Records management plan
- [ ] Data governance framework
- [ ] Acceptable use policy
- [ ] Incident response procedures
- [ ] Change management process
- [ ] Third-party management
- [ ] Compliance monitoring plan

### Human-Centred Controls

- [ ] Consent mechanisms:
  - [ ] Opt-in/opt-out design
  - [ ] Consent recording
  - [ ] Withdrawal process
- [ ] User interface design:
  - [ ] Clear labelling
  - [ ] Intuitive navigation
  - [ ] Accessibility compliance
  - [ ] Error messaging
- [ ] Support systems:
  - [ ] User training materials
  - [ ] Help documentation
  - [ ] Support channels
  - [ ] Feedback mechanisms
- [ ] Worker support:
  - [ ] Retraining programs
  - [ ] Change support
  - [ ] Wellbeing resources

### Engagement Controls

- [ ] Stakeholder communication plan
- [ ] Regular feedback sessions
- [ ] WHS committee engagement
- [ ] Transparency reporting
- [ ] Community consultation
- [ ] User advisory groups
- [ ] External audit/review

### Control Assignment

- [ ] Assign control owner for each measure
- [ ] Define implementation timeline
- [ ] Allocate resources/budget
- [ ] Create implementation plan
- [ ] Define success metrics
- [ ] Plan control testing
- [ ] Document control-risk mapping

---

## Step 6: Documenting and Reporting Checklist

### Core Documentation

- [ ] Finalised FAIRA template:
  - [ ] All tables completed
  - [ ] Values matrix filled
  - [ ] Risk register attached
  - [ ] Control plan included
- [ ] Security documentation:
  - [ ] Threat model
  - [ ] Security architecture
  - [ ] Incident response plan
  - [ ] Security test results
- [ ] WHS documentation:
  - [ ] Impact assessment
  - [ ] Consultation records
  - [ ] Training plans
  - [ ] Safety procedures
- [ ] Decision log:
  - [ ] Key decisions
  - [ ] Rationales
  - [ ] Approvals
  - [ ] Exceptions

### Linkages and Integration

- [ ] Link to enterprise risk register
- [ ] Reference in Human Rights Assessment
- [ ] Include in Privacy Impact Assessment
- [ ] Add to procurement documentation
- [ ] Update QITC alignment docs
- [ ] Connect to project management system
- [ ] Link to compliance tracking

### Reporting Structure

- [ ] Executive summary dashboard
- [ ] Detailed technical reports
- [ ] Compliance attestations
- [ ] Performance metrics
- [ ] Incident reports
- [ ] Audit findings
- [ ] Improvement recommendations

### Access and Distribution

- [ ] Define document access controls
- [ ] Create distribution lists
- [ ] Establish update notifications
- [ ] Plan regular reviews
- [ ] Version control setup
- [ ] Archive procedures

---

## Step 7: Lifecycle Maintenance Checklist

### Review Triggers

- [ ] Set annual review date
- [ ] Define change triggers:
  - [ ] Model updates
  - [ ] Algorithm changes
  - [ ] Training data refresh
  - [ ] New data sources
  - [ ] Scope expansion
  - [ ] User base changes
  - [ ] Incident occurrence
  - [ ] Audit findings
  - [ ] Regulatory changes
  - [ ] Technology updates

### Continuous Monitoring

- [ ] Model performance tracking:
  - [ ] Accuracy metrics
  - [ ] Drift detection
  - [ ] Bias monitoring
  - [ ] Error analysis
- [ ] Security monitoring:
  - [ ] Threat detection
  - [ ] Vulnerability scanning
  - [ ] Penetration testing
  - [ ] Log analysis
- [ ] Operational monitoring:
  - [ ] System availability
  - [ ] Response times
  - [ ] Resource utilisation
  - [ ] User satisfaction
- [ ] Compliance monitoring:
  - [ ] Policy adherence
  - [ ] Regulatory compliance
  - [ ] Ethics alignment
  - [ ] Control effectiveness

### Update Processes

- [ ] FAIRA refresh procedure:
  - [ ] Schedule review sessions
  - [ ] Update risk assessments
  - [ ] Revise control plans
  - [ ] Document changes
- [ ] Training updates:
  - [ ] User training refresh
  - [ ] Admin training updates
  - [ ] WHS training reviews
  - [ ] Awareness campaigns
- [ ] Documentation updates:
  - [ ] Procedure revisions
  - [ ] Policy updates
  - [ ] Guidance refresh
  - [ ] Template improvements

### Stakeholder Engagement

- [ ] Annual stakeholder review
- [ ] WHS committee updates
- [ ] User feedback sessions
- [ ] Executive briefings
- [ ] Audit committee reports
- [ ] External review planning
- [ ] Community updates

### Improvement Actions

- [ ] Incident lessons learned
- [ ] Enhancement opportunities
- [ ] Technology upgrades
- [ ] Process improvements
- [ ] Control optimisation
- [ ] Training enhancements
- [ ] Documentation improvements

### Sign-off and Approval

- [ ] Annual executive sign-off
- [ ] Risk acceptance reviews
- [ ] Control attestations
- [ ] Compliance certifications
- [ ] Audit sign-offs
- [ ] Committee approvals
- [ ] Budget renewals

---

## Quick Reference - Critical Must-Dos

### Before Development

- [ ] Form multi-disciplinary team
- [ ] Complete FAIRA Part A (system definition)
- [ ] Conduct values assessment
- [ ] Identify and score risks
- [ ] Plan controls and mitigations

### During Development

- [ ] Implement technical controls
- [ ] Create user documentation
- [ ] Conduct security testing
- [ ] Engage stakeholders
- [ ] Document decisions

### Before Deployment

- [ ] Complete all assessments (PIA, HRA, etc.)
- [ ] Test all controls
- [ ] Train users and operators
- [ ] Establish monitoring
- [ ] Get formal approvals

### After Deployment

- [ ] Monitor continuously
- [ ] Review annually
- [ ] Update for changes
- [ ] Address incidents
- [ ] Improve iteratively

---

_Remember: This is a living process. Regular reviews and updates ensure your AI system remains safe, secure, ethical, and compliant throughout its lifecycle._
