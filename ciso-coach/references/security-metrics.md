# Security Metrics for CISOs

Key metrics that matter for security leadership and executive reporting.

## Core Measurement Categories

### 1. Detection & Response Metrics

**Mean Time to Detect (MTTD)**
- How long it takes to discover a security incident
- Industry benchmark: 24-48 hours for mature programs
- Report as: Trend over time, not just a number

**Mean Time to Respond (MTTR)**
- Time from detection to containment
- Industry benchmark: 4-8 hours for critical incidents
- Report as: By severity level

**Detection Coverage**
- % of environment with active monitoring
- % of critical assets with EDR/logging
- Goal: 95%+ for critical assets

### 2. Vulnerability Management Metrics

**Time to Patch**
- Critical: <24 hours
- High: <7 days
- Medium: <30 days
Report by severity, not as averages

**Vulnerability Remediation Rate**
- % of identified vulns fixed within SLA
- More useful than total vuln count
- Target: 95%+ of criticals on time

**Exposure Window**
- Days between vulnerability disclosure and patch
- Critical for zero-days

### 3. Access & Identity Metrics

**MFA Coverage**
- % of users with MFA enabled
- % of critical systems requiring MFA
- Target: 100% for privileged access, 95%+ for all users

**Privileged Access Review**
- % of privileged accounts reviewed quarterly
- Average days since last access review
- Target: 100% quarterly reviews

**Access Removal Speed**
- Time from termination to access removal
- Target: Same day for terminations

### 4. Security Awareness Metrics

**Phishing Simulation Results**
- Click rate on simulated phishing
- Report rate from users
- Trend more important than absolute numbers

**Training Completion**
- % of employees completing security training
- Target: 95%+ annually

**Repeat Offenders**
- Users who repeatedly fail phishing tests
- Indicates need for targeted training

### 5. Compliance & Risk Metrics

**Control Effectiveness**
- % of security controls functioning as intended
- Based on control testing results
- Target: 95%+ effective

**Policy Compliance Rate**
- % of systems/users meeting security policies
- Track by policy domain

**Risk Acceptance Tracking**
- Number of accepted risks
- Dollar value of accepted risks
- Age of accepted risks

### 6. Program Health Metrics

**Security Debt**
- Known issues not yet addressed
- Quantified in risk or dollars
- Trend should be decreasing

**Vendor Risk**
- % of vendors with completed assessments
- % of high-risk vendors with remediation plans
- Target: 100% of critical vendors assessed

**Budget Utilization**
- % of security budget spent
- Should align with project completion

## Reporting Frameworks

### Monthly Executive Dashboard (One Page)

1. **Risk Posture** (Red/Yellow/Green)
   - Critical vulnerabilities: X open
   - Detection coverage: Y%
   - Incidents this month: Z

2. **Key Metrics Trends** (3-month view)
   - MTTD/MTTR trending
   - Phishing click rate trending
   - Patching SLA compliance

3. **Notable Events**
   - Incidents (brief)
   - Major projects completed
   - Upcoming compliance deadlines

4. **Asks**
   - Decisions needed
   - Resources needed
   - Policy approvals needed

### Quarterly Board Presentation

1. **Strategic Overview** (2 min)
   - Overall security posture
   - Progress on annual goals

2. **Key Metrics** (3 min)
   - 3-5 most important metrics
   - Year-over-year trends

3. **Major Incidents** (2 min)
   - What happened
   - Business impact
   - Lessons learned

4. **Looking Ahead** (3 min)
   - Emerging threats
   - Planned initiatives
   - Investment needs

Total: 10 minutes for presentation + 5-10 for questions

## Metrics to Avoid

**Don't report:**
- Total vulnerabilities (meaningless without context)
- Logs collected (activity metric, not outcome)
- Alerts generated (says nothing about effectiveness)
- GB of data scanned
- Number of policies written

**These are "vanity metrics"** - they show activity but not value or improvement.

## Benchmarking Your Metrics

Compare against:
- **Industry standards** (NIST, CIS, ISO 27001)
- **Peer organizations** (similar size/sector)
- **Your own history** (year-over-year improvement)

Never compare against:
- Generic "best in class" (often marketing)
- Organizations in different risk profiles
- Metrics without methodology transparency
