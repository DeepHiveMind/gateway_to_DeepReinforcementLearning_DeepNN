# Deep Dive into AI SECURITY
'AI Security' is now often being discussed a lot, and is increasingly becoming a point of concern as, in a technical parlance, AI/ML model endpoints are been exploited as attack-vector / vulnerability vector. *AI/ML Model endpoint Privacy*  | *Data Privacy in Real World AI/ML System* | *Lack of Comprehensive adoption of DevSecOps Pipeline in Real World AI/ML system* et al.

#### Why AI SECURITY is important
- AI/ML Models are getting deployed on edge devices / edge gateways / Fog devices / Mobiles for offline predictions (owing to rapid proliferation of IIoT/ CIoT) 
	- Agile, Dynamic Security Perimeter of AI/ML Serving end points
- AI/ML Models gets exposed to real data, and inferencing of models can expose sensitive information
- AI/ML Models generally are not trained on Masked data
- AI/ML Model endpoint security (owing to uS Microservice style of AI/ML serving, AI-as-a-Service)
	- AI/ML RESTful or gRPC end point Authentication & Authorization
	- AI/ML Federated User Pool & Identity Pool management (FIdM/ FIM)
- Absence of DevSecOps *(Security-as-a-Code)* implementation pipeline in AI/ML Application productionization- i.e., lack of awareness for 
	- Vulnerability Scanning while Application development, such as *SAST Vulnerability Scanning*
	- Vulnerability Scanning while Application deployment, such as *DAST Vulnerability Scanning*
	- SIEM in production (Continuous Monitoring, Threat detection and alerting, Threat remediation)
	

#### Real World AI Comprehensive SOC Solution
There is comprehensive SOC solution (SOC- Security Operation Control - Plane) for *real world AI/ML*.

Real World AI/ML SOC Plane is a custom solution, and is composed of following solution components primarily:

- Privacy Preserving Machine Learning
	- Differntial Privacy (offered by libraries such as Tensorflow Privacy)
	- ε-differentially private algorithms (Google's Differential Privacy)
	- Homomorphic Encryption (Intel n-Graph with Tensorflow, or, Microsoft SEAL)
{P.S.: Homomorphic encryption is a form of encryption that allows computation on encrypted data, and is an attractive remedy to increasing concerns about *data privacy in the field of machine learning*.}	
	
- AI/ML API/Endpoint Security 
	- AI/ML RESTful or gRPC end point Authentication & Authorization
	- AI/ML Federated User Pool & Identity Pool management (FIdM/ FIM)

- Implementation DevSecOps (Security-as-Code) pipeline for AI/ML Application development, deployment, monitoring, Threat detection and alerting, Threat remediation
	- Please refer to my another repo [DevSecOps Sec-as-a-Code]() for delving deeper into the awesome world of DevSecOps.
