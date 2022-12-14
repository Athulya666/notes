#security_driven_networking
__SECURITY DRIVEN NETWORKING overview__
provides secure high performance connectivity between users,applications,devices.
uses- internal segmentation/automated threat protection/policy enforcement

what is digital transformation
the process of using digital technologies to create new or to modify existing organizational processes,culture and customer experiences to meet changing requirements.
benefits are enhances the collection of customer data/uses resources more efficiently. 

digital transformation creates many network edges inconsistent security, unpredictable experience, complex to manage.

__FORTIGATE__
ngfw - next generation firewall
powered by fortios
root fortigate is in edge.
can see access points, endpoints, threats, on premise and SaaS applications.
FORTIGATE advanced NGFW functions
application control(to create policies), intrusion prevention, antivirus, URL filtering, sandboxing, SSL inspection
spu - security process units(fortigate devices powered by spu)
SD-WAN is built into fortigate and can be enabled- application steering(block unathorized applications), wan path remediation(optimizing bandwidth), ipsec VPN
FORTIGATE FORM FACTORS- physical, VM, firewall as a service
FortiManager - centrally manages security fabric devices like fortigate. provide centralized policy enforcement. 

__FORTIAP__
fortiap is a secure access point device designed and produced by fortinet that allows users to access the network using wifi technologies.
secure LAN edge.
fortinet secure lan edge through fortilink
fortiwlm - troubleshooting, wireless management.
fortideploy - deploy fortiap, fortiAP connects to fortiDeploy/ fortiap direct to fotigate.

__FORTIMANAGER__
fortimanager is a device either physical or virtual provides single console to administrator and gain visibility to fortinet devices
fabric management center- enable customers to simplify the network operations.
	simplified provisioning- 
	centralized management-
	network analytics -
	compliance reporting-
	network automation-

__FORTISWITCH__
fortiswitch is a secure network switch which is designed by fortinet
fortiwsitch deployment options - fortilink/ standalone
fortinet secure ethernet through fortilink
fortilink enables fortigate to extend its NGFW features into wired and wireless network component. 
fortilink connects fortigate and fortiswitch, fortiapi is connected to fortiswitch
fortiswithc product
	access switch family
	data center switch family
	fortiswitch rugged
cloud management for fortiswitch
	fortiswitch cloud- manage stand alone fortiswitch deployment
	fortigate cloud- manage fortilink enabled fortiswitch deployment

__FORTISASE__
__FORTIEXTENDER__ - integrating 5G LTE(long term evolution) connections into sd-wan

#Zero_trush_access
fortinet zta
enables organizations to see and control everyone and everything on the network
principles of the fortinet ZTA
	verify
	give minimal access
	assume that the network is compromised
reducing attack surface

__forticlient EMS__ endpoint management server.(use zero trush tagging rules)
__Fortinet fabric management center__
	fortimonitor
	forti analyzer
	forti siem
	forti soar
	forti EDR
	forti AI

Products of the zero trust access solution
	FortiAuthenticator
	is gatekeeper of authorzation into the fortinet secured enterprise network.identifying users,querying access permissions from third party systems, communicating the information to fortigate
	fortiClient
	connects endpoints with the fortinet security fabric.
	FortiNAC
	is a security product that implements policy on devices that access networks to increase network visibility and control and facilitate automated responses.

__FORTIAUTHENTICATOR__
identity management

__FORTICLIENT__
is intergrated endpoint agent
what problems it solve- lack of visibility, vulnerable endpoints, unsuspectting users,
epp- endpoint protection platform 
1. fabric agent- visibility, quarantine, vulnerability, app inventory
2. secure remote access - ssl/ipsec vpn, sso and ZTNA (single sigh on (SSO))
3. advanced threat protection - sandbox integration
4. endpoint protection platform(EPP) - app fw, antimalware, anti-exploit,web filtering. (CPRL- compact pattern recognition language)

forticlient integrates with fortiauthenticator to support multi factor authentication.

__FORTINAC__
network access control is security solution that identifies and enforces policy on devices that access networks to increase visibility and reduce risk.
nac goals - visibility, control, automated response
FortiGate provides security rating service. the scores can be viewed from the root fortigate, fortiNAC identifies and classifies devices. 

FortiNAC integrates with:
	fortigate
	fortianalyzer
	fortiSIEM
	fortiSwitch
	fortiAP
	forticlient
	fortiEDR

the product components of fortinet ZTNA are:
	fortigate NGFW
	fortimanager for centralized management
	forticlient as the ZTNA agent at the endpoint
	forticlient endpoint management server(EMS) to configure the forticlient ZTNA agents
	FortiAuthenticator
	fotitoken
FortiNAC uses rules, which can consist of up to 20 profiling methods, to identify and categorize an unknown device. once device is assigned a device type it can be added to a role and group that can restrict what the device can do. 

#Adaptive_cloud_security
adaptive cloud security solution principal
1. native integration- supports the auto scaling capabilities of the cloud providers
2. broad protection - provide zero day threat protection against new AI and ML
3. management and automation- enables regulatory compliance through centralized security management, automated workflows and shared threat intelligence.

Products of the solution
	fortigate cloud
	fortiDDoS
	fortiWeb
	fortiMail
	FortiADC
	fortiCASB
	fortiCNP
value of the solution
	security posture
	IT
	business

__FortiADC__
application delivery controller.
scale web based applications for capacity and availability.
what problems does fortiADC solve
	server load balancing
	secure traffic offloading
	global server load balancing
	persistence
	HTTP compression
the correct topology positioning for FortiADC
wireless access point-> firewall-> application device controller-> application servers

__FORTIMAIL__
operation modes - gateway mode, microsoft 365 API claw back, transparent mode, server mode
email continuity - is designed to protect valuable productivity by providing emergency mailbox services when organizations experience an outage in their mail services.
fortiisolarot- allows users to browse in isolated env.
dynamic image analysis service.

__FortiWeb__

#security_operations
fortinet fabric management center 
	soc platform - centralized management, security fabric analytics
	breach protection - security automation and orchestration, advanced threat detection
	end point security - detection and response for endpoints.

product of the solution
SOC platform
	fortianalyzer
	fortiSIEM
	fortiSOAR
	fortiXDR
Advanced threat protection
	fortiSandbox
	fortiDeceptor
	fortiilnsight
	fortiAI
Endpoint security
	fortiClient(fabric agent)
	fortiEDR
security fabric integration
	fortiGate
	fortiManager

__fortiNDR__
network detection and response
use ai and other analytics to identify suspicious activities, covering both network traffic and file based analysis(virtual security analyst, detect, trace ,respond
fortinet products that feed fortiNDR files for analysis are fortiGate, fortiProxy, fortiSandbox and fortiWeb. 
the principal features of fortiNDR are the VSA, detecting,tracing,responding,

__FortiAnalyzer__
allows to create playbooks for automation
form factors
	appliance
	virtual machine (vmware,ms hyper-v)
	cloud (aws,azure)
	hosted (fortianalyzer cloud)
key benifits
	increase security
	reduces complexity
	lowers TCO
	automates compliance
FortiAnalyzer correlates logs to construct a comprehensive security view of the network
FortiGuard indicator of compromise service provides daily threat intelligence updates to construct a list of possible compromised hosts.
fortiView provides real time reporting of threat intelligence through dashboards and monitors
FortiGuard security rating service performs ongoing security autdit of the network and highlights gaps in security and problem areas. 

___FortiDeceptor___
act as a honeypot
steps of fortiDeceptor
	expose- acts as an early warning system that generates alerts for review and validation
	Eliminate- can trigger fortigate to quarantine the ip address of the threat actor
	deceive- lures attackers with decoys and real devices equipped with tokens that appear indistinguishable from real IT and OT assets.

___FORTIEDR___
epp(endpoint protection) with detection and response.
	discover and prevent attacks
	detect, defuse and respond
	remediate and investigate
features
	pre infection- discover and predict
	post infection - block,detect defuse, respond and investigate

___forti sandbox___
safe isolated env which can analyse dynamic behavior

___FORTISIEM___
features
	CMDB(configuration management db)- discovery and inventory
	monitor and maintain business services
	detect and remediate
	assess and report on compliance
	extensible and customizable
multi tenancy for MSP(manage service providers)

___FortiSOAR___
automated playbook/ incident triage/ real time remediation
key differentiators of fortisoar
	advanced case management
	sophisticated role based access control(RBAC)
	simplified playbook designer
	enterprise scalable architecture

___FortiXDR___
endpoint and IOT security/ network access and security/ application and cloud security





