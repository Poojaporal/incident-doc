

This skill is used for monitoring scheduled jobs, identifying failures, analyzing errors, and performing rerun the jobs or corrective actions. It ensures smooth job execution and minimal business impact.
Name	Score job monitoring
Description  Use this skill when monitoring batch jobs, handling job failures, analyzing errors, and rerunning jobs in production 
Step 1:
Before running any commands, extract these key fields from the ticket:
Field	What to look for
System type	AS400-MBS001(PROD)
Alert / error message	Job started, MSGW, ended abnormally, job did not start, Po conformation 
Time of failure	Dependency job not completed

STEP 2:
When to Use
Use this skill when:
- A job fails or goes into an abnormal state
- An incident triggered for job failure
- Job output is incorrect or incomplete
- Dependencies between jobs are broken
- Rerun or recovery actions are required
 STEP 3:
Core Workflow:
3. 1. Job Monitoring
- Continuously monitor job schedules and execution status
- Check job completion, delays, or failures
- Validate job outputs and logs
 3.2. Incident Identification
- Receive alerts/incidents from monitoring tools
- Identify impacted job and system
- Categorize severity (high/medium/low)
3.3. Root Cause Analysis
- Analyze job logs and error messages
- Check:
  - File availability
  - Database issues
  - Dependency failures
  - System/environmental issues
- Identify exact failure reason
3. 4. Resolution / Action
- Fix the issue based on root cause:
  - Restart services if required
  - Correct data or file issues  
- Coordinate with dependent teams
3.5. Job Rerun
- Rerun failed jobs after fixing issue
- Ensure:
 - No duplicate data
  - Dependencies are satisfied
- Monitor rerun until successful completion
3.6. Validation
- Confirm job completed successfully
- Validate output/data correctness
- Ensure downstream jobs are not impacted
3. 7. Incident Closure
- Update incident with:
  - Root cause
  - Resolution steps
  - Preventive actions
- Close ticket after confirmation
 3.8. Decision Rules
 - If failure is due to dependency → Fix dependency first, then rerun
- If data issue → Correct data before rerun
- If system issue → Restart/recover system before rerun
- If repeated failure → escalate to L2/L3 or development team
 Best Practices
- Always check logs before rerun
- Avoid blind returns (may cause duplicate data)
- Maintain proper communication with stakeholders.
- Document recurring issues for future prevention
  Common Issues
- Missing input files
- Job dependency failure
- Database connection issues
- Timeout or performance issues
- Incorrect job configuration
  Outcome
- Jobs are successfully executed
- Incidents are resolved quickly
- Business impact is minimized
Step 4:
Reference link:
**incident jan to March 4.xlsx**

