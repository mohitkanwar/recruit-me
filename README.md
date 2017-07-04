# recruit-me
This is a webapp which is used to manage recruitment process in an organization.

# User Roles
* Recruiter
* Applicant
* Referrer
* Interviewer
* Manager

A job will be posted by a Manager with specific Job Description containing desired years of experience in desired experience areas.

An Applicant can apply directly to the Job, or can be referred by a referrer. To apply for the job, following things are expected
  - resume
  - Name
  - Email Id
  - Phone number
  - years of experience in various areas
  
 A recruiter will filter resumes and align interview panel
 
 Interview panel will conduct interviews with the applicant and fill up feedback and ratings
 Next panel will be able to see ratings from previous interview/test
 
 Once all rounds are cleared, manager will approve/reject applicant.
 Recruiter will followup with applicants/interview panel/ manager on next steps
 
 
 # Domain Model
 * Job Post
 * Job Description
    * Job Title
    * List of Experience Areas
 * Experience Area
        * Area
        * Pet Questions
 * Interview Process Chain
    * Interview Process
      * Time
      * Test
 * Ratings
 * Users
 * User Roles
    * Recruiter
    * Applicant
    * Referrer
    * Interviewer
    * Manager
    
 # APIs
 GET    /jobs  
 GET    /job/{job-id}  
 PUT    /job/{job-id}  
 POST   /job/{job-id}  
 GET    /job/applicants  
 GET    /applicant/{applicant-id}  
 PUT    /applicant/{applicant-id}  
 POST   /applicant/{applicant-id}  
 PUT    /job/{job-id}/applicant/{applicant-id}  
 POST   /job/{job-id}/applicant/{applicant-id}  
 GET    /panel/{panel-id}  
 PUT    /panel/{panel-id}  
 POST   /panel/{panel-id}  
 GET    /manager/{manager-id}  
 PUT    /manager/{manager-id}  
 POST   /manager/{manager-id}  
 GET    /recruiter/{recruiter-id}  
 PUT    /recruiter/{recruiter-id}  
 POST   /recruiter/{recruiter-id}  
 GET    /zoneofexperience/{zone-id}  
 PUT    /zoneofexperience/{zone-id}   
 POST   /zoneofexperience/{zone-id}   
 GET    /interviewprocess/{process-id}  
 PUT    /interviewprocess/{process-id}   
 POST   /interviewprocess/{process-id}  
 GET    /interviewprocesschain/{process-chain-id}  
 PUT    /interviewprocesschain/{process-chain-id}   
 POST   /interviewprocesschain/{process-chain-id}  
 POST   /login  
