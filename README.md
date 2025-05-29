# NFT_AI_Resume

Concept: ZK-Abstracted Resume System

🔐 "Selective CV disclosure based on viewer role — without revealing the full CV."

Concept Summary

We will build a minimal ZK dApp that allows users to:

Create a full CV once.

Automatically generate different abstraction layers of the CV depending on who is viewing it (e.g., HR Manager, CEO, Interviewer, Public Viewer).
Without revealing unnecessary or sensitive information to unauthorized viewers.


The system will:

Accept full user CV input.

Generate different ZK proofs corresponding to each abstraction layer.

Produce a shareable verification link or access token for each viewer type.

Ensure viewers only see the level of information they are permitted to, validated with ZK proofs.

Present each abstraction in an NFT format


🔁 User Flow 
User Input:

Full CV details (Education, Work History, Skills, Achievements, Contact Info).


System Processing:

Generates 4 abstraction layers:


Public View (basic bio, headline)


Interviewer View (skills + recent projects)


HR View (full work history + education)


CEO View (strategic highlights only)



Creates ZK proofs for each abstraction level.


ZK Circuit (Leo):

Confirms that only the appropriate CV abstraction is accessible for a given role (input).

Uses hash commitments for each abstraction to maintain privacy.

Outputs the allowed CV subset based on the viewer’s authorized role.


Verifier (CLI or simple UI):

Viewer selects their role (HR, CEO, Interviewer, Public) and submits proof.

System reveals the corresponding abstraction layer without exposing full CV.
