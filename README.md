# Dev. Work Report

## Project: Sales Analysis Pipeline – TechStore

### Goal
Document technical errors, debugging strategies, repository organization, deployment workflow, and lessons learned during the development and publication process.

---

## STEP 1 — Repository Configuration

### Problem
The repository could not be found during remote connection attempts.

### Cause
Incorrect repository URL configuration caused routing failure.

### Solution
Corrected the repository name directly in the GitHub interface and validated the remote configuration.

### Learning
• Importance of repository validation  
• URL structure verification  
• Remote connection workflow  

### Improvement
• Validate repository configuration before authentication setup  
• Standardize repository naming conventions  

---

## STEP 2 — Authentication and Access

### Problem
Authentication failed even with a valid GitHub token.

### Cause
The token was automatically invalidated after exposure during the workflow process.

### Solution
Migrated authentication strategy from HTTPS token access to SSH key authentication.

### Learning
• Authentication security practices  
• SSH workflow configuration  
• Credential management importance  

### Improvement
• Avoid token exposure during configuration  
• Use SSH authentication as default workflow  

---

## STEP 3 — SSH Permission Configuration

### Problem
SSH connection failed during repository access.

### Cause
The public SSH key had not been registered in the GitHub account settings.

### Solution
Generated and linked the public SSH key to the GitHub account manually.

### Learning
• SSH key structure and validation  
• Access permission management  
• Secure remote authentication workflow  

### Improvement
• Configure SSH authentication before repository operations  

---

## STEP 4 — Directory Structure and Tracking

### Problem
Git could not locate the project files during tracking operations.

### Cause
The terminal targeted the incorrect directory level while the actual project files were stored inside the src/ folder.

### Solution
Adjusted the Git tracking scope to the correct project directory structure.

### Learning
• Directory hierarchy organization  
• Git tracking workflow  
• Importance of project structure consistency  

### Improvement
• Organize folder hierarchy before version control initialization  
• Create standardized project structures  

---

## STEP 5 — Cache and Synchronization Failure

### Problem
GitHub Desktop remained stuck during synchronization attempts.

### Cause
Corrupted cache references and fragmented commit history affected repository synchronization.

### Solution
Applied a manual deployment workflow:
• Downloaded clean repository ZIP  
• Reorganized project structure locally  
• Uploaded files directly through GitHub web interface  

### Learning
• Alternative deployment strategies  
• Manual repository recovery workflow  
• Cache failure troubleshooting  

### Improvement
• Maintain clean commit history  
• Validate synchronization state frequently  

---

## Workflow Structure

The final project pipeline followed this structure:

• Data Extraction and Reading  
• Data Cleaning and Grouping  
• Statistical Visualization  
• Automated Executive Report Generation in Excel  

---

## Technical Reflection

The debugging and deployment process reinforced:
• workflow organization  
• troubleshooting methodology  
• repository management  
• persistence during technical failures  
• adaptive problem-solving strategies  

The project also improved understanding of:
• Git workflows  
• authentication systems  
• data processing pipelines  
• debugging logic  
• deployment organization  

---

Author: Géssica Nascimento  
Systems Analysis & Development Student  

Date: 28/05/2026
