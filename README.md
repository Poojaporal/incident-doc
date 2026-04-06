

	Score job monitoring and incidents
Description : This skill is used for monitoring scheduled jobs, identifying failures, analyzing errors, and performing rerun the jobs or corrective actions. It ensures smooth job execution and minimal business impact.
Step 1:
Before running any commands, extract these key fields from the ticket:
Field     	               What to look for
System type   	            AS400-MBS001(PROD)
Alert / error message     	Job started, MSGW, ended abnormally, job did not start, Po conformation 
Time of failure	Dependency job not completed
**STEP 2:
**
When to Use
Use this skill when:
- A job fails or goes into an abnormal state
- An incident triggered for job failure
- Job output is incorrect or incomplete
- Dependencies between jobs are broken
- Rerun or recovery actions are required
 STEP 3:
Core Workflow:
**3. 1. Job Monitoring**
- Continuously monitor job schedules and execution status
- Check job completion, delays, or failures
- Validate job outputs and logs
** 3.2. Incident Identification**
- Receive alerts/incidents from monitoring tools
- Identify impacted job and system
- Categorize severity (high/medium/low)
**3.3. Root Cause Analysis**
- Analyze job logs and error messages
- Check:
  - File availability
  - Database issues
  - Dependency failures
  - System/environmental issues
- Identify exact failure reason
**3. 4. Resolution / Action**
- Fix the issue based on root cause:
  - Restart services if required
  - Correct data or file issues  
- Coordinate with dependent teams
**3.5. Job Rerun**
- Rerun failed jobs after fixing issue
- Ensure:
 - No duplicate data
  - Dependencies are satisfied
- Monitor rerun until successful completion
**3.6. Validation**
- Confirm job completed successfully
- Validate output/data correctness
- Ensure downstream jobs are not impacted
**3.7. Decision Rules**
 - If failure is due to dependency → Fix dependency first, then rerun
- If data issue → Correct data before rerun
- If system issue → Restart/recover system before rerun
- If repeated failure → escalate to L2/L3 or development team
**  Common Issues**
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
https://mckessoncorp-[my.sharepoint.com/:x:/r/personal/krishnaveni_gangarapu_mckesson_com/Documents/Microsoft%20Teams%20Chat%20Files/incident%20jan%20to%20march%204.xlsx?d=w6040d7b52f584dfd83fde981a1fc9447&csf=1&web=1&e=EmFPQ](https://mckessoncorp-my.sharepoint.com/:x:/r/personal/krishnaveni_gangarapu_mckesson_com/Documents/Microsoft%20Teams%20Chat%20Files/incident%20jan%20to%20march%204.xlsx?d=w6040d7b52f584dfd83fde981a1fc9447&csf=1&web=1&e=Eeko1K)I

