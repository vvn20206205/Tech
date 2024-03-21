```
Title: A Survey of Security and Privacy in Cloud Computing: Challenges, Solutions and Future Directions
```

```
Abstract

This survey paper gives an overview of cloud computing infrastructure, how cloud computing works, as well as how major companies around the world implement cloud computing transformation.
```

```
I. Introduction


In recent years, cloud computing has emerged as a dominant paradigm in the realm of IT infrastructure, driven by a confluence of market forces and technological advancements.
```

```
In the previous part, my group presented Abstract and Introduction.
Today, I will continue to present part II. Security and Privacy challenges
```

```
II. Security and Privacy challenges
```

```
In this section, we investigate the specific security and privacy challenges in cloud computing which pose lots of threats, risks and require the development of advanced security technologies.
```

A “threat” is an act of coercion of a potential attack to elicit negative response. It is generally an effect that can be described as anything that would tamper, destruct or interrupt of any service or item of value. The term “risk” refers to the possibility of being targeted by an attack, getting success and exposed by the attack. The term “vulnerability” refers to the security flaws in a system that allows an attack to be successful . In general, the threats exploit the vulnerabilities of a system, which leads to risk by damaging assets and causing exposure. However, threats can be identified in order to mitigate risks and countermeasure for vulnerabilities.

```

A. Loss of control
1) Data Loss and Data Theft

Data loss and data breaches were recognized as the top threats in cloud computing environments
```

in 2013. A recent survey shows that 63% of customers would be less likely to purchase a cloud service if the cloud vendor reported a material data breach involving the loss or theft of sensitive or confidential personal information.

```
Whether a C can securely maintain customers’ data has become the major concern of cloud users.
```

The frequent outages occurring on reputable CSPs , including Amazon, Dropbox, Microsoft, Google Drive, etc., further exacerbate such concerns [9].

```
Data Loss: Due to the number of interactions between known/unknown risks & challenges in the architectural or operational characteristics of Cloud Computing.
```

Accidental deletion or alteration of records without a backup; Storage on unreliable media; Loss of encoding key by customer; unauthorized access to sensitive data; operational failures; disposal challenges; risk of association; jurisdiction & political issues; data centre reliability; physical catastrophe; disaster recovery; Results: devastating business impact; damage to brand & reputation; impact stakeholders’ moral & trust; loss of property; leakage of data lead to compliance violations & legal ramifications[7].

```
Data theft: In a multitenant infrastructure, if cloud service database has error in design, a flaw in one client’s application will allow an attacker to access not only to that application data but every others’ data as well.
```

Offline backups of data to avoid catastrophic data loss will also increase the chance of exposure to data breache[7].

```
2) Data storage and tranmission through regional norms

Due to the distributed infrastructure of the cloud, cloud users’ data may be stored on data centers geographically located in multiple legal jurisdictions, leading to cloud users’ concerns about the legal reach of local regulations on data stored out of region.
```

Furthermore, the local laws may be violated since the dynamic nature of the cloud makes it extremely difficult to designate a specific server or device to be used for transborder data transmission [9].

```
3) Cheap Data Leakage and Analysis

The rapid development of cloud computing has facilitated the generation of big data, leading to cheap data collections and analysis. For example, many popular online social media sites, such as Facebook, Twitter and LinkedIn, are utilizing the cloud computing technology to store and process their customers’ data.
```

Cloud providers that store the data are gaining considerable business revenue by either retrieving user information through data mining and analysis by themselves or selling the data to other businesses for secondary usage.

```
One example is that Google is using its cloud infrastructure to collect and analyze users’ data for its advertisingnetwork.
```

```
Such data usage has raised extensive privacy concerns since the sensitive information of cloud users may be easily accessed and analyzed by unauthorized parties.
```

The Electronic Privacy Information Center (EPIC) asked to shut down Gmail, Google Docs, Google Calendar, and the company’s other Web apps until government-approved
“safeguards are verifiably established”. Netflix had to cancel its $1 million data challenge prize due to a legal suit because it violated customers’ privacy during the data sharing process. While technologies such as data anonymization are under investigation, users’ data privacy has to be fundamentally protected by standards, regulations and laws [9].

```
B. Shortage of Transparency
1) Malicious Insiders/Unauthorized Internal Access
```

Threats amplify due to the convergence of IT services under a single management domain; General lack of transparency into CSP processes & procedures; less visibility into the hiring standard and practices of cloud employees’ lead to adversary.

```
A malicious insider, such as a system administrator, in an improperly designed cloud scenario can have access to potentially sensitive information.
```

Results: Espionage; hacker; organized crime; corporate espionage; spoofing; tampering, information disclosure; nation-state sponsored intrusion; Brand damage; financial impact; productivity losses; impact on business continuity, traditional security and disaster recovery[7].

```
2) Ambiguous ownership & responsibility
```

Lack of clear ownership and defined responsibilities for data protection may responsibility result in failure of meeting regulatory and of data legal obligations[7].
Authentication & Authorization:

```
Cloud building organizations has to authenticate each and every person who is using the cloud from the cloud utilizing organization. They will provide authorizations to the users based on the service usage and payment. The cloud building organization has to prevent unauthorized users by checking authorization.
```

The cloud utilizing organization has to remove or disable accounts of the ex-employees on day-to-day basis[28].

```
C.Virtual Machine Related Challenges

Virtualization refers to the logical abstraction of computing resources from physical constraints. One representative example of virtualization technology is the virtual machine
```

(VM). Virtualization can also be performed on many other computing resources, such as operating system, networks, memory, and storage. In a virtualized environment, computing resources can be dynamically created, expanded, shrunk or moved according to users’ demand, which greatly improves agility and flexibility, reduces costs and enhances business values for cloud computing.
Despite of its substantial benefits, this technology also introduces security and privacy risks in the cloud computing environment.

```
1- Security threats sourced from host

Monitoring VMs from host The control point in virtual environment is the host machine there are implications that allow the host to monitor and communicate with VM applications up running.
```

Therefore, it is more necessary to strictly protect the host machines than protecting distinctive VMs . VM-level protection is crucial in cloud computing environment. The enterprise can co-locate applications with different trust levels on the same host and can defend VMs in a shared multi-tenant environment. This enables enterprises to maximize the benefits of virtualization. VM-level protection allows VMs to stay secure in today’s dynamic data centers. Also, as VMs travel between different environments – from on-premise virtual servers to private clouds to public clouds, and even between cloud vendors[6].

Communications between VMs and host The data transfer between VMs and the host flow between VMs shared virtual resources; in fact the host can monitor the network traffic of its own hosted VMs. This can be considering useful features for attackers and they may use it such as shared clipboard which allows data to transfer between VMs and the host using cooperating malicious program in VMs . It is not generally considered a bug or limitation when one can initiate monitoring, change, or communication with a VM application from the host. The host environment needs to be more strictly secured than the individual VMs.

```
The host can influence the VMs in the following ways[6]:

• The host can Start, shutdown, pause, and restart VMs.
• Monitoring and configuration of resources which are available to the VMs, these include: CPU, memory, disk, and network usage of VMs.
• Adjust the number of CPUs, the amount of memory, the amount and number of virtual disks, and a number of virtual network interfaces which are available to a VM.
• Monitoring the applications which are running inside the VM.
• View, copy, and possibly modify, data stored on the VM's virtual disks. Unfortunately, the system admin or any authorized user who has privileged control over the backend can misuse these procedures.
```

```
2- Security threats sourced from other VM

Monitoring VMs from other VM Monitoring VMs could violate security and privacy,
```

but the new architecture of CPUs, integrated with a memory protection feature, could prevent security and privacy violation. A major reason for adopting virtualization is to isolate security tools from an untrusted VM by moving them to a separate trusted secure VM.

```
Communication between VMs: One of the most critical threads that threaten exchanging information between virtual machines is how it's deployed.
```

Sharing resources between VMs may strip security of each VM for instance collaboration using application such as shared clipboard that allow exchanging data between VMs and the host assisting malicious program in VMs, this situation violate security and privacy.

Also, a malicious VM can has chance to access other VMs through shard memory .

```
Denial of Service (DoS): A DoS attack is a trying to denial services that provide to authorize users.    For example when trying to access site we see that due to overloading of the server with the requests to access the site, we are unable to access the site and observe an error.
```

This happens when the number of requests that can be handled by a server exceeds its capacity, the Dos attack marking carting part of clouds inaccessible to the users. Usage of an Intrusion Detection System (IDS) one of the useful method of defense against this type of attacks.

```
D. Managerial Issues

Most cloud-specific security and privacy challenges have their own managerial aspect.
```

For example, the malicious insider challenge involves the problem of effectively managing employees to detect early warning signs and responding to policy violations in a timely manner once malicious insider incidents occur. These managerial challenges are non-technical in nature but also closely related to the technical solutions that could help cope with the corresponding technical challenges.

```
Implementing a technical solution and not managing it properly are bound to introduce vulnerabilities.
```

For example, security management for virtualization, which is dramatically unlike that of traditional networks, requires knowledge and skill sets beyond the capabilities of the general network administrator, leading to increased management complexity and risks.

```
Inappropriate VM management policies may cause the number of VMs to continuously grow while most of them are in the middle or sleep mode leading  to the host machine’s resource exhaustion.
```

The fact that managerial challenges are overarching and add to the other challenges is what makes it one of the toughest challenges to deal with. CSPs have to make a decision on the scope of their managerial effort in order not to exhaust their resources before all their most critical security and privacy goals and objectives are met [9].
