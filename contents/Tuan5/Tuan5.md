<!-- ! -->
II. Security and Privacy challenges
<!-- ! -->
In this section, we investigate the specific security and privacy challenges in cloud computing which require the development of advanced security technologies.
<!-- ! -->
A. Loss of Control
<!-- ! -->




In cloud computing, loss of control refers to the situation that cloud users’ control over their data is diminished
when they move the data from their own local servers to
remote cloud servers. A great number of concerns about
data protection are raised, since giving up direct control
has to be one of the hardest things enterprises have to do
[4].







<!-- 1) Data Loss and Data Breach -->
Data loss and data breaches were recognized as the top
threats in cloud computing environments in 2013 [5]. A
recent survey shows that 63% of customers would be less
likely to purchase a cloud service if the cloud vendor
reported a material data breach involving the loss or theft
of sensitive or confidential personal information [6].
Whether a CSP can securely maintain customers’ data
has become the major concern of cloud users. The frequent outages occurring on reputable CSPs [7], including
Amazon, Dropbox, Microsoft, Google Drive, etc., further
exacerbate such concerns.
To help customers recover in case of service failures,
data proliferation is conducted in the cloud where customers’ data is replicated in multiple data centers as
backups [8]. However, the distributed storage for multiple data copies may increase the risks of data breaches
and inconsistency. First, due to the heterogeneity of security settings for the multiple storage devices, the overall
security level of the data is only determined by the weakest link in the chain. Attackers can obtain the data if any
one of the storage devices is compromised. Second, the
multiple data copies need to be synchronized when customers make any data updates, including insertion, modification and deletion. The failures of data synchronization
will lead to data inconsistency. Last but not least, it is
more challenging for Cloud Service Users (CSUs) to
track the appropriateness of a CSP’s data operations. For
example, it is extremely difficult to ascertain whether the
CSP will completely delete all the data copies when such
a request is made by the CSU [8]. External auditing processes are required to supervise a CSP’s data operations.


<!-- 2) Data Storage and Transmission under Multiple -->
Regional Regulations
Due to the distributed infrastructure of the cloud, cloud
users’ data may be stored on data centers geographically
located in multiple legal jurisdictions, leading to cloud
users’ concerns about the legal reach of local regulations
on data stored out of region [9]. Furthermore, the local
laws may be violated since the dynamic nature of the
cloud makes it extremely difficult to designate a specific
server or device to be used for transborder data transmission [8].
<!-- 3) Cheap Data and Data Analysis -->
The rapid development of cloud computing has facilitated the generation of big data, leading to cheap data collections and analysis [10]. For example, many popular
online social media sites, such as Facebook, Twitter and
LinkedIn, are utilizing the cloud computing technology
to store and process their customers’ data [11]. Cloud
providers that store the data are gaining considerable
business revenue by either retrieving user information
through data mining and analysis by themselves or selling the data to other businesses for secondary usage [8].



One example is that Google is using its cloud infrastructure to collect and analyze users’ data for its advertising
network [10].
Such data usage has raised extensive privacy concerns
since the sensitive information of cloud users may be easily accessed and analyzed by unauthorized parties. The
Electronic Privacy Information Center (EPIC) asked to
shut down Gmail, Google Docs, Google Calendar, and
the company’s other Web apps until government-approved
“safeguards are verifiably established” [12]. Netflix had
to cancel its $1 million data challenge prize due to a legal
suit because it violated customers’ privacy during the
data sharing process [13]. While technologies such as
data anonymization are under investigation [8], users’
data privacy has to be fundamentally protected by standards, regulations and laws.
<!-- B. Lack of Transparency -->
In the context of cloud computing security, transparency refers to the willingness of a CSP to disclose various
details on its security readiness. Some of these relevant
details include policies on security, privacy, service level,
etc. [14]. In addition to the willingness, when measuring
transparency, it is important to observe how accessible
the security readiness data and information are. No matter how much security facts about an organization are
available, if they are not presented in an organized and
easily understandable manner for CSUs and auditors, the
transparency of the organization should still be rated relatively low.
CSUs and auditors need to know the types of security
controls put in place by CSPs for their cloud infrastructure, but CSPs are often not willing to share this information. This is partially due to the fact that some of this
information can be considered to consist of trade secret.
For example, a lot of technical knowhow is involved in
effectively storing and securing customer data, and it
takes significant time and resources to reach the acceptable level of technical sophistication.
Therefore, CSUs and CSPs should negotiate on the
information to be shared. Depending on the negotiation
results, CSUs may decide not to use the services provided
by the CSP. In fact, many CSUs choose not to use CSPs
because of the frustration associated with this negotiation
process and the resulting lack of transparency. For cloud
computing to be more widely used, this challenge of
transparency is one of the biggest obstacles to be removed.
<!-- C. Virtualization Related Issues -->
Virtualization refers to the logical abstraction of computing resources from physical constraints. One representative example of virtualization technology is the virtual
machine (VM). Virtualization can also be performed on
many other computing resources, such as operating sys




tems, networks, memory, and storage. In a virtualized
environment, computing resources can be dynamically
created, expanded, shrunk or moved according to users’
demand, which greatly improves agility and flexibility,
reduces costs and enhances business values for cloud
computing [15].
In spite of its substantial benefits, this technology also
introduces security and privacy risks in the cloud computing environment.
1) New Access Context
Virtualization brings new challenges to user authentication, authorization and accounting in terms of properly
defining roles and policies [16]. Virtualization technology enables users to access their data and applications
running on a single logical location which is usually the
integration of multiple physical or virtual devices. The
lack of security border and isolation introduces the possibility of information leakage [17]. Furthermore, such
access can be done through a single user account logged
on from diverse devices located anywhere in the world.
This new access context raises many challenges, such as
whether a user has the same privileges to access different
physical or virtual devices; whether the accounts logged
on from multiple distant geographic locations belong to
the same user. Granular separation of user roles is
required to address these challenges [16].
2) Attacks against Hypervisor
The hypervisor which manages multiple VMs becomes
the target of attacks [16]. Different from physical devices
which are independent from one another, VMs in the
cloud are usually residing in one physical device managed by the same hypervisor. The compromise of the
hypervisor therefore will put multiple VMs at risk. Furthermore, the immaturity of the hypervisor technology,
such as isolation, access control, security hardening, etc.,
provides attackers with new ways to exploit the system.
Diverse attacks against virtual machines are as follows.
VM Hijacking: When a VM is launched, the information required to invoke the VM is created and saved on
the host. In the multi-tenant scenario, this information for
all the VMs located in the same server will be stored on a
common storage system. The attackers gaining access to
this storage space will be able to break into the VMs,
which is called VM Hijacking [18].
VM Hopping: If an attacker gains access over the
hypervisor, he/she is able to manipulate the network traffic, configuration files, and even the connection status of
the VMs located on top of the hypervisor [19, 20].
VM Escape: Attackers gaining access to the host running multiple VMs are able to access the resources shared
by the VMs, and even bring down these resources and
turn off the hypervisor [20].
VM Mobility: A VM can be copied over the network or
through a USB, and the source configuration files are rec




reated when the VM is moved to a new location. This
way, the attackers are able to modify the configuration
file as well as the VM’s activities [19]. Furthermore, once
a VM is infected and readmitted to its original host, the
infection can potentially spread out to other VMs located
on the same host. Such an attack is also known as a virtual library check-out [21].
Dormant VMs: VMs can exist in either active or dormant states. Although the dormant VMs may still hold
sensitive user data, they can easily be overlooked and not
updated with latest security settings, leading to potential
information leakage [16].
<!-- D. Multi-Tenancy Related Issues -->
Multi-tenancy is defined as “the practice of placing
multiple tenants on the same physical hardware to reduce
costs to the user by leveraging economies of scale” [22].
It indicates sharing of computational resources, storage,
services and applications with other tenants, hosted by
the same physical or logical platform at the provider’s
premises [23]. While the multi-tenancy architecture allows
CSPs to maximize the organizational efficiency and significantly reduce a CSU’s computing expenses, it does
not come without costs. Adversaries taking advantage of
the co-residency opportunities may launch diverse attacks
against their co-residents, resulting in a number of security/privacy challenges [24].
Specifically, in the multi-tenant environment, different
tenants’ security controls are heterogeneous. The tenant
with less security controls or misconfigurations is easier
to compromise, which may serve as a stepping stone to
the more secured tenants located in the same host. This
could reduce the overall security level for all the tenants
to that of the least secured one [16]. Furthermore, the
security policies made by different tenants may disagree
or even conflict with one another. Such disagreements or
conflicts could introduce threats to tenants’ needs, interests or concerns [25].
Furthermore, attackers taking advantage of the multitenancy architecture may be able to launch diverse attacks
against their co-tenants, such as inferring confidential
information or degrading co-tenants’ performance.
Confidential information may be inferred via sidechannel attacks. A side-channel attack is any attack based
on information gained from the physical implementation
of a system [26]. This type of attack primarily occurs due
to covert channels with flawed access control policies
that allow unauthorized access [27]. Some typical side
channel attacks include: 1) timing attacks based on measuring the time it takes for a unit to perform operations
[28], 2) power consumption attacks where the attacker
can identify system processes by analyzing the power
consumed by a unit while performing different operations
[28], and 3) differential fault analysis where the attacker
studies the behavior of a system by injecting faults into it
[28], 4) cache usage attacks where the attacker measures
the utilization of CPU caches on its physical machine to
monitor the activities on co-residents’ activities [29], 5)
load-based co-residence detection where the attacker
measures the load variation of its co-resident to verify
whether it is co-located with the target victim [29], and 6)
estimating the traffic rates of the co-resident [29].
A co-resident’s performance may be degraded by overconsuming computing resources, such as CPU, memory,
storage space, I/O resources, etc. A Swiper attack is proposed in [30], with which the attacker uses a carefully
designed workload to incur significant delays on the coresident’s targeted application. In [31], the authors propose and implement an attack which modifies the workload of a victim VM in a way that frees up resources for
the attacker’s VM. The reason for the success of such
attacks is that an overload created by one tenant may negatively impact the performance of another tenant [32].
<!-- E. Managerial Issues -->
Most cloud-specific security and privacy challenges
have their own managerial aspect. For example, the malicious insider challenge involves the problem of effectively managing employees to detect early warning signs
and responding to policy violations in a timely manner
once malicious insider incidents occur. These managerial
challenges are non-technical in nature but also closely
related to the technical solutions that could help cope
with the corresponding technical challenges. Note that
one of the biggest managerial challenges in cloud computing security is that all these technical solutions have to
be managed eventually. Implementing a technical solution and not managing it properly are bound to introduce
vulnerabilities. For example, security management for
virtualization, which is dramatically unlike that of traditional networks, requires knowledge and skill sets
beyond the capabilities of the general network administrator, leading to increased management complexity and
risks [17]. Inappropriate VM management policies may
cause the number of VMs to continuously grow while
most of them are in the middle or sleep mode (i.e., VM
sprawling), leading to the host machine’s resource exhaustion [33]. We discuss the relationship between technical
solutions and their managerial counterparts in Section IV.
Loss of control is another example of a managerial
challenge dominating its associated technical challenges.
The main source of the problem results from the fact that
in-house managerial controls are not able to reach the
computing and data resources managed by a CSP. The
managerial challenge in this case is to develop a comprehensive and effective service level agreement (SLA) to
extend the reach of the in-house security and privacy controls into the CSP organization. Often this effort leads to
power struggles between CSUs and CSPs and becomes
highly political, which require both technical and mana



gerial expertise in order to arrive at a mutually beneficial
solution for both CSUs and CSPs.
Finally, the lack of transparency challenge has its own
strong managerial components. CSUs and CSPs must go
through elaborate negotiations to acquire and provide
essential information to ensure the security and privacy
of the cloud services. An SLA also plays an important
role in this challenge since it helps articulate and specify
what information has to be available to satisfy the security and privacy needs of the CSU and the requirements
imposed by laws and regulations.
The fact that managerial challenges are overarching
and add to the other challenges is what makes it one of
the toughest challenges to deal with. CSPs have to make
a decision on the scope of their managerial effort in order
not to exhaust their resources before all their most critical
security and privacy goals and objectives are met.