1-What is a Docker component?

Docker ek open-source platform hai jo containerization technology ka use karta hai. Docker containers ek lightweight, portable, and self-sufficient unit hoti hain, jisme applications aur unke dependencies encapsulate hote hain. Docker ke kuch important components hain:

Docker Engine:
Ye Docker ka core component hai, jo containers ko build, run, aur manage karta hai. Docker Engine ke do main parts hote hain:
Docker Daemon:
Background me run karne wala process, jo containers ko manage karta hai.
Docker CLI (Command Line Interface):
Command line tool jiski madad se users Docker se interact karte hain.
Docker Image:
Ye ek template hoti hai jo ek application aur uske dependencies ko container me encapsulate karti hai. Images Docker Hub ya kisi aur registry se download ki ja sakti hain, ya phir khud create ki ja sakti hain.
Docker Container:
Ye ek runtime instance hota hai ek Docker image ka. Containerization ki madad se applications ko ek isolated environment me run kiya ja sakta hai, jisme unki dependencies already include hoti hain.
Docker Compose:
Docker Compose ek tool hai jiska use multiple Docker containers ko define aur run karne ke liye kiya jata hai. Ye ek YAML file ka use karta hai jisme services, networks, aur volumes ko describe kiya jata hai.
Docker Registry:
Docker images ko store karne ke liye online repositories hote hain, jinhe Docker Registries kehte hain. Docker Hub ek public registry hai, lekin hum khud bhi apni private registry setup kar sakte hain.
Dockerfile:
Dockerfile ek text file hota hai jo Docker image ko build karne ke liye instructions provide karta hai. Ye file ko step-by-step process define karta hai, jisme base image se starting hota hai aur fir required configurations aur dependencies ko add kiya jata hai.

In components ka use karke, Docker developers ko applications ko easily deploy, scale, aur manage karne me madad karta hai, irrespective of the environment jisme ye containers run ho.

=====================================================================

2-Difference between containerization and virtual machines.

Containerization aur Virtual Machine (VM) dono hi tarah ke virtualization technologies hain, lekin inme kuch mukhya antar hote hain.
Resource Utilisation:
Containerization: Containers lightweight hote hain aur ek hi host operating system (OS) ko share karte hain. Isme, multiple containers ek hi OS kernel par chalte hain, jisse resource utilisation efficient hoti hai.
Virtual Machine: VMs ek hypervisor ke through multiple operating systems ko host operating system par run karne mein help karte hain. Har VM apna khud ka OS kernel hota hai, isliye ye zyada resources consume karte hain.
Performance:
Containerization: Containers quickly start hote hain aur kam memory space aur time mein deploy ho sakte hain.
Virtual Machine: VMs thoda slow hote hain start hone mein, aur zyada resources ki zarurat hoti hai.
Isolation:
Containerization: Containers ek dusre se isolated hote hain, lekin same host OS kernel ko share karte hain.
Virtual Machine: VMs puri tarah se isolated hote hain, alag-alag OS kernel par chalte hain, jisse security level zyada hota hai.
Deployment:
Containerization: Containers ko kisi bhi environment mein aasani se deploy kiya ja sakta hai, kyunki ve khud-sustain karne wale hote hain.
Virtual Machine: VMs ko deploy karne mein thoda complex hota hai, kyon ki ve puri tarah se ek virtualized environment ko require karte hain.
Size:
Containerization: Containers small size ke hote hain kyunki ve host OS kernel ko share karte hain.
Virtual Machine: VMs zyada size ke hote hain kyunki har ek VM apna khud ka OS aur kernel lekar aata hai.Containerization aur Virtual Machine (VM) dono hi tarah ke virtualization technologies hain, lekin inme kuch mukhya antar hote hain.
In summary, containerization zyada lightweight aur flexible hoti hai, jabki virtual machines isolation aur security mein zyada powerful hote hain. Har ek ka use case alag hota hai, aur vyavsayik requirements ke hisab se ek technology ko choose kiya jata hai.

=====================================================================

3-Why do we use containerization?

Containerization ko use karne ke kai reasons hain jo modern software development and deployment practices ko support karte hain. Yeh kuch mukhya reasons hain jinse containerization popular hai:

Portability:

Containers encapsulate applications aur unke dependencies ko, jo unhe portable banata hai. Ek bar containerize kiya gaya application kisi bhi environment mein consistent taur par run kar sakta hai, chahe woh development machine ho, testing server ho, ya production environment.

Efficiency and Resource Utilization:

Containers lightweight hote hain aur host operating system ka kernel share karte hain. Isse resource utilization improve hoti hai, aur multiple containers ek hi host par run kar sakte hain bina significant resource overhead ke.

Rapid Deployment:

Containers ke startup aur shutdown times bahut tez hote hain, jisse applications ko jaldi deploy kiya ja sakta hai. Isse development aur testing cycles me bhi tezi aati hai.

Scaling:

Container orchestration tools jaise ki Kubernetes ki madad se, containers ko easily scale kiya ja sakta hai. Applications ko demand ke hisaab se horizontally scale karna (multiple instances run karke) aasan ho jata hai.

Microservices Architecture:

Containerization microservices architecture ke sath achha fit hota hai. Alag-alag components ko alag containers me run karke, unhe independently develop aur deploy kiya ja sakta hai. Isse scalability aur maintainability improve hoti hai.

Isolation:

Containers provide process-level isolation. Each container has its own file system, network, and process space, making it isolated from other containers on the same host. Isolation improves security and helps prevent conflicts between applications.

Consistency Across Environments:

Containers ensure consistency across different environments, eliminating the “it works on my machine” problem. Developers can package their applications and dependencies together, reducing the chances of environment-related issues.

Version Control and Rollback:

Docker images, which are used to create containers, can be version-controlled. This allows for easy rollback to a previous version in case of issues or for testing different versions of an application.

DevOps Practices:

Containerization is a key enabler of DevOps practices. It supports continuous integration (CI) and continuous deployment (CD) workflows, allowing for faster and more reliable software delivery.

Resource Efficiency in Cloud Environments:

In cloud environments, where resources are billed based on usage, containers allow for more efficient resource utilization. They can be quickly started and stopped, allowing for cost savings.

Containerization, particularly using tools like Docker, has become a fundamental part of modern software development and deployment pipelines due to these advantages. It enables agility, scalability, and consistency in software delivery.

=========================================================

4-Difference between Container and Pod.

Container:

Definition: Container ek lightweight, standalone, and executable software package hai, jisme application aur uske dependencies encapsulate hote hain.
Isolation: Containers provide process-level isolation. Each container runs as an isolated process on the host operating system.
Resource Sharing: Containers share the host operating system's kernel but have their own user space, file system, and network.
Portability: Containers are portable and can run consistently across different environments, thanks to their encapsulation of dependencies.
Pod:

Definition: Pod ek abstraction layer hai jo ek ya multiple containers ko group mein rakhta hai aur unhe shared context provide karta hai. Pod ek Kubernetes concept hai.
Isolation: Containers inside a pod share the same network namespace and can communicate with each other using localhost. They are scheduled together on the same node.
Resource Sharing: Containers within a pod can easily communicate with each other using localhost. They share the same IP address and port space.
Portability: While individual containers are portable, the concept of a pod is specific to Kubernetes, making it a higher-level abstraction.
Key Differences:

Scope of Abstraction:
    Container focuses on packaging and running a single application and its dependencies.
    Pod is a higher-level abstraction that groups one or more containers together and provides a shared network namespace.

Networking:
    Containers within a pod share the same network namespace, allowing them to communicate using localhost.
    Containers in different pods have their own network namespaces and typically communicate over the network.

Use Case:
    Containers are used for encapsulating and running individual applications.
    Pods are used for deploying and managing groups of containers that need to work together, share data, or communicate closely.

Kubernetes Specific:
    Containers are a general concept and can be used outside of Kubernetes.
    Pods are specific to Kubernetes and are used to deploy and manage containers within a Kubernetes cluster.
In summary, a container is a standalone unit that encapsulates an application and its dependencies, while a pod is a higher-level abstraction in Kubernetes that groups one or more containers together for common networking and shared context. Containers are a fundamental concept, and pods are a Kubernetes-specific construct for managing and orchestrating containers.

=========================================================

5-How Docker storage and network work.

Docker storage aur networking, Docker containers ko deploy, manage, aur communicate karne mein important roles play karte hain. Niche Docker storage aur networking ke basic concepts hain:
Docker Storage:

Image Storage:
    Docker images, jo containers ke base hote hain, stored hote hain registries mein. By default, images Docker Hub jaise public registries se download hote hain, lekin aap apna private registry bhi use kar sakte hain.
    Local storage par Docker images cache bhi hoti hai, taki frequently used images ko local storage se retrieve kiya ja sake.

Container Storage:
    Har ek container apne khud ke file system layer ke sath aata hai. Har container, image se derive hota hai, lekin usmein read-write layer bhi hota hai, jise container ke runtime changes store karne ke liye use kiya jata hai.
    Containers ephemeral hote hain, iska matlab hai ki jab container stop hota hai, uski file system changes bhi lost ho jati hain. Isko persist karne ke liye volumes ka use kiya jata hai.

Volumes:
    Volumes, Docker containers ke liye persistent storage provide karte hain. Ye data ko host system ya external storage solution se map karte hain, jisse data survive karta hai even if the container is stopped or removed.
    Volumes allow data sharing between containers and can be used to store configuration files, databases, or any other data that needs to persist across container instances.
Docker Networking:

Bridge Networking:
    By default, Docker uses bridge networking, where each container is connected to a private internal network. Containers can communicate with each other using their IP addresses.
    Docker creates a bridge network (docker0) on the host, and each container gets its own IP address on this bridge.

Port Mapping:
    Containers can expose specific ports, and these ports can be mapped to ports on the host machine. This allows external processes to communicate with the containerized application.

Host Networking:
    Docker containers can use the host's network namespace, allowing them to directly access the host's network interfaces. This can be useful for performance-critical applications.

Overlay Networking:
    Docker supports overlay networks for multi-host communication. This is crucial in a Docker swarm or Kubernetes cluster, where containers on different hosts need to communicate.
    Overlay networks use encapsulation techniques to enable communication between containers running on different hosts.

Macvlan Networking:
    Macvlan allows containers to have their own MAC addresses, making them appear as physical devices on the network. This can be useful for scenarios where containers need to be directly on the local network.

Custom Bridge Networks:
    Docker allows the creation of custom bridge networks, which can be used to connect containers within a specific application or service. Containers on the same custom bridge network can communicate with each other.
Docker networking enables containers to communicate with each other and with the external world. It provides flexibility in configuring how containers access and expose services. Docker storage mechanisms, including images, containers, and volumes, ensure that data is managed efficiently and can persist beyond the lifecycle of individual containers.

=========================================================

6-Difference between Low Level and High Level and what are the differences between types.
Docker runtime ko do categories mein baat kiya ja sakta hai - Low Level Runtime aur High Level Runtime. Ye dono runtimes Docker container ko host machine par run karne mein madad karte hain, lekin unke kaam karne ke tareekon mein kuch antar hote hain.
Low Level Runtime:
Low Level Runtime, container ki execution ko manage karta hai. Isme, container ke individual processes ko control kiya jata hai. Kuch pramukh Low Level Runtimes hain:
runC (OCI Runtime): Ye Open Container Initiative (OCI) ka hissa hai aur Docker containers ko run karne ke liye use hota hai. Ye ek standard interface provide karta hai jo container runtimes ko interact karne mein help karta hai.
High Level Runtime:
High Level Runtime, container ko orchestrate karne aur uske lifecycle ko manage karne mein help karta hai. Isme, multiple containers ko ek sath deploy aur manage kiya ja sakta hai. Kuch pramukh High Level Runtimes hain:
Dockerd (Docker Daemon): Docker daemon, containers ko create, deploy, aur manage karta hai. Ye High Level Runtime ke roop mein kaam karta hai aur user ko ek simplified interface provide karta hai containers ko operate karne ke liye.
Types of Runtimes:
Low Level Runtimes:
runC: Ye ek command line tool hai jo containers ko run karne ke liye use hota hai. Ye OCI standard follows karta hai aur container ko ek low-level isolation environment provide karta hai.
High Level Runtimes:
containerd: Ye ek daemon hai jo container runtime (runC) ko orchestrate karta hai. Docker daemon (dockerd) containerd ka use karta hai apne containers ko manage karne ke liye.
Docker Swarm: Ye ek orchestration tool hai jo multiple containers ko ek sath deploy, manage, aur scale karta hai.
Difference:
Low Level Runtimes: Ye containers ke individual processes ko control karte hain, aur unhe runC ke through execute karte hain. (It describes a detailed description of each and every module )
High Level Runtimes: Ye containers ke orchestration aur management ke liye responsible hote hain. Ye tools jaise ki Docker Daemon aur Docker Swarm ke roop mein aate hain. (Yeh application ka overall description ya architecture ko describe krta hai.)
In dono runtimes ka combination ek complete containerization solution provide karta hai, jisme Low Level Runtime container execution ko handle karta hai, aur High Level Runtime multiple containers ko orchestrate aur manage karta hai.

Difference between High Level Design and Low Level Design :
S.No.
HIGH LEVEL DESIGN
LOW LEVEL DESIGN

High Level Design is the general system design means it refers to the overall system design.
Low Level Design is like detailing HLD means it refers to component-level design process.

High Level Design in short is called HLD.
Low Level Design in short is called LLD.

It is also known as macro level/system design.
It is also known as micro level/detailed design.

It describes the overall description/architecture of the application.
It describes a detailed description of each and every module.

High Level Design expresses the brief functionality of each module.
Low Level Design expresses detailed functional logic of the module.

It is created by a solution architect.
It is created by designers and developers.

Here in High Level Design the participants are the design team, review team, and client team.
Here in Low Level Design participants are design team, Operation Teams, and Implementers.

It was created first before Low Level Design.
It is created as a second means after High Level Design.

In HLD the input criteria is Software Requirement Specification (SRS).
In LLD the input criteria is reviewed by High Level Design (HLD).

High Level Solution converts the Business/client requirement into High Level Solution.
Low Level Design converts the High Level Solution into Detailed solution.

In HLD the output criteria is database design, functional design and review record.
In LLD the output criteria is program specification and unit test plan.

========================================================================

7-Difference between Podman and Docker and how Podman manages containers.

Podman vs Docker :
S.NO
PODMAN
DOCKER
1
Daemanless ( jisme koi service file nahi hoti )
Root by default
2
Rootless
Root by default
3
Can manage pods
Less secure
4
More secure (maintain better security through audit logging)
Less secure (can’t trace & maintain correctly by audit logging )
5
Separate container process by user
Maintain all container & process with the same user

Podman aur Docker dono containerization tools hain jo containers create, manage, aur run karne mein madad karte hain, lekin inme kuch differences hain. Niche main aapko bataunga Podman aur Docker ke beech kuch mukhya antar aur Podman ke container management ke tareeke:
Podman aur Docker ke Antar:

Daemon-less (No Docker Daemon):
    Docker: Docker ek client-server architecture pe based hai, jisme Docker Daemon continuously run karta hai. Docker CLI Docker Daemon se communicate karta hai.
    Podman: Podman daemon-less architecture pe based hai. Har command ek naya container process create karta hai, isliye Podman ko daemon run karne ki zarurat nahi hoti.

User Permissions:
    Docker: Docker commands run karne ke liye user ko typically docker group mein add karna padta hai, jisse elevated permissions milte hain.
    Podman: Podman container processes user ke context mein run hote hain, isliye elevated permissions ki zarurat nahi hoti.

Rootless Containers:
    Docker: Rootless Docker support karta hai, lekin iske liye specific configuration ki zarurat hoti hai.
    Podman: Rootless containers Podman ka in-built feature hai, aur ye out-of-the-box support karta hai.

Storage:
    Docker: Docker storage driver ka use karta hai, jo host machine ke storage subsystem ke upar depend karta hai.
    Podman: Podman overlayfs ka use karta hai, jo ek Linux kernel feature hai. Isme storage driver Docker se alag hota hai.

Networking:
    Docker: Docker default bridge network ka use karta hai. Additional networks ko create karne ke liye Docker CLI ka use hota hai.
    Podman: Podman bhi default bridge network ka use karta hai. Lekin, Podman ke alag commands se aap easily custom networks create kar sakte hain.
Podman Container Management:

Podman containers Docker ki tarah hi manage karta hai, lekin kuch command ke tareeke alag hote hain:

Container Create:
    Docker: docker create
    Podman: podman create

Container Run:
    Docker: docker run
    Podman: podman run

List Containers:
    Docker: docker ps -a
    Podman: podman ps -a

Stop Container:
    Docker: docker stop
    Podman: podman stop

Remove Container:
    Docker: docker rm
    Podman: podman rm

Inspect Container:
    Docker: docker inspect
    Podman: podman inspect

Logs:
    Docker: docker logs
    Podman: podman logs
Podman ka use karke bhi aap containers create, run, stop, remove, aur manage kar sakte hain, lekin Podman ka approach daemon-less hai, aur isme user permissions aur rootless containers ke liye better support hai. Ye ek alternative option hai Docker ke liye, especially agar aap daemon ki zarurat nahi chahte ya rootless environment mein work karna chahte hain.

=========================================================

8-How to run a rootless Podman container and how it works.

Rootless Podman ka use karke aap containers ko run kar sakte hain bina root (superuser) ke. Isse aapko security aur permission concerns me flexibility milti hai. Niche main aapko step-by-step guide dunga rootless Podman container run karne ke liye:

Step 1: Podman Install karein:

Sabse pehle toh aapko Podman install karna hoga. Aap apne system ke operating system ke package manager ka use karke Podman ko install kar sakte hain. Jaise ki:



# Ubuntu/Debian
sudo apt-get install -y podman

# CentOS/RHEL
sudo dnf install -y podman
Step 2: User Namespace Enable karein:

Rootless containers ke liye, user namespace enable hona chahiye. Iske liye aapko kernel parameter set karna padta hai. Aap /etc/sysctl.conf ya /etc/sysctl.d/ me jakar user.max_user_namespaces ko update kar sakte hain ya fir directly sysctl command se apply kar sakte hain.



sudo sysctl -w kernel.unprivileged_userns_clone=1
Step 3: Rootless Podman Run karein:

Ab aapko Podman ka use bina root ke containers run karne ke liye ready hain. Aap kisi bhi Podman command ko run kar sakte hain bina sudo ke, jaise ki:



podman run -it --rm alpine sh

Yeh command ek Alpine Linux container ko run karega aur aapko uske shell me le jayega.
Kaise Kaam Karta Hai:

Jab aap rootless Podman ka use karte hain, toh user namespace ka use hota hai. User namespace ek security feature hai jo user ko ek isolated user space provide karta hai, jisse container root user bhi host root user se alag hota hai.
Rootless Podman container processes host system ke user ke context me run hote hain, lekin ye containerized environment provide karte hain jisse host system ke files aur resources ko protect kiya ja sake.
Isme kisi bhi containerized process ka access host system ke processes ya files tak limited hota hai, jisse security enhanced hoti hai.
Rootless Podman ka use karke aap containers ko bina root permissions ke easily manage aur run kar sakte hain, aur isse aapko better security aur isolation milti hai.

=========================================================

9-How Kubernetes runs containers and pods.

Kubernetes ek container orchestration platform hai jo applications ko scale, manage, aur deploy karne mein madad karta hai. Kubernetes containers aur pods ko manage karne ke liye kuch key concepts provide karta hai. Niche main aapko kuch basic steps bata raha hoon jo Kubernetes mein containers aur pods run karne mein involved hote hain:
Containers Kubernetes Mein Kaise Run Hote Hain:

Container Image Create karein:
    Sabse pehle, aapko apne application ke liye ek Docker container image create karna hoga. Is image mein aapke application aur uske dependencies hote hain.

Docker Image Ko Registry Mein Push karein:
    Aapko apne Docker image ko kisi container registry mein push karna hoga, jaise ki Docker Hub, Google Container Registry, Amazon ECR, etc.

Kubernetes Manifest File Create karein:
    Ek YAML file create karein jise Kubernetes manifest file kehte hain. Is file mein aap define karenge ki aap kis container image ko kahan aur kaise run karna chahte hain.

Manifest File ko Kubernetes Cluster Mein Apply karein:
    Kubernetes cluster mein jayein aur apne manifest file ko apply karein, jisse Kubernetes apne resources ko manage karna shuru karega.

Kubernetes Pods ki Status Check karein:
    Aap apne pods ki status ko kubectl command ka use karke check kar sakte hain.


    kubectl get pods
Pods Kubernetes Mein Kaise Run Hote Hain:

Pod Definition File Create karein:
    Ek YAML file create karein jise pod definition file kehte hain. Is file mein aap ek ya multiple containers define kar sakte hain, jo ek hi pod mein run karenge.

Pod Definition File ko Kubernetes Cluster Mein Apply karein:
    Apne pod definition file ko Kubernetes cluster mein apply karein, jisse Kubernetes pod ko create karega aur uske andar specified containers ko run karega.


kubectl apply -f pod-definition.yaml
Pod ki Status Check karein:

Aap apne pods ki status ko kubectl command ka use karke check kar sakte hain.


kubectl get pods
Pod Logs Check karein:

Aap kisi specific pod ka log check karne ke liye kubectl logs command ka use kar sakte hain.


    kubectl logs pod-name

Pod ke Andar Containers ke beech Communication:
    Pods ke andar ke containers ek hi network namespace mein hoti hain, jisse unke beech communication local network ke through ho sakti hai.
Kubernetes ke abstractions, jaise ki Pods, Deployments, Services, etc., aapko containers ko efficiently manage aur orchestrate karne mein madad karte hain. Ye concepts aapko scalability, reliability, aur flexibility provide karte hain jab aap apne applications ko production environment mein deploy karte hain.

=========================================================

10-What are OCI, CRI, and CRI-O?

OCI (Open Container Initiative), CRI (Container Runtime Interface), aur CRI-O, ye teeno technologies containerization aur container orchestration ecosystem mein mukhya roles play karte hain. Chaliye in teeno ko thoda detail mein samajhte hain:

OCI (Open Container Initiative):

Definition: OCI ek open standard specification hai jise maintain karne ke liye Linux Foundation ke under ek project hai. Iska goal container formats aur runtime ko standardise karna hai.

Container Format (Image): OCI ki specification ke hisaab se container image format define hota hai. Docker ne initially apne image format ko donate kiya tha, jise OCI ne accept kiya.

Runtime Specification: OCI specification container runtime ke liye bhi guidelines provide karta hai, jisse ek container runtime, jaise ki Docker ya containerd, OCI compliant ho sakta hai.

Interoperability: OCI ke standards ke karan, alag-alag container runtimes aur orchestrators (jaise ki Kubernetes) aapas mein interoperable hote hain. Aap ek OCI compliant container image ko kisi bhi OCI compliant runtime par run kar sakte hain.

Docker Daemon Start Hota Hai:
Docker Images Check Hote Hain:
Container Create Hota Hai:
OCI Runtime (runC) Ka Use Hota Hai:
Namespace Aur cgroups Create Hote Hain:
Container Start Hota Hai:
Application Run Hota Hai:
Logs Aur Output Display Hote Hain:
Container Background Mein Run Hota Hai (if specified):

CRI (Container Runtime Interface):

Definition: CRI ek Kubernetes project hai jo Kubernetes aur container runtimes ke beech ka communication standardise karta hai.

Kubernetes and Runtimes Communication: CRI allows Kubernetes to communicate with container runtimes without having direct dependencies on a specific container runtime implementation. This separation of concerns helps in better maintainability and flexibility.

Abstraction: CRI provides a clear abstraction between Kubernetes and container runtimes, enabling Kubernetes to support multiple container runtimes seamlessly.

Adaptability: Kubernetes can support various container runtimes like Docker, containerd, CRI-O, etc., through the CRI standard.

CRI-O:

Definition: CRI-O ek lightweight, OCI-compliant container runtime hai jo specifically Kubernetes ke liye design kiya gaya hai.

Focus on Kubernetes: CRI-O ka primary focus Kubernetes ke sath seamless integration aur collaboration hai. Ye ek dedicated container runtime hai jise sirf Kubernetes ke liye develop kiya gaya hai.

Reduced Complexity: CRI-O ki design philosophy ye hai ki ye lightweight aur simplified ho, jisse isme unnecessary features na hon aur isme security aur performance ko focus kiya ja sake.

OCI Compliance: CRI-O OCI standards ka palan karta hai, iska matlab hai ki aap CRI-O ke through OCI-compliant container images ko run kar sakte hain.

In teeno technologies ka combination aapko containerization ecosystem mein flexibility aur interoperability provide karta hai. OCI standard container formats aur runtimes ko standardise karta hai, CRI container runtimes aur Kubernetes ke communication ko standardise karta hai, aur CRI-O ek lightweight, OCI-compliant container runtime hai jo specifically Kubernetes ke liye design kiya gaya hai.

====================================================================
CMD
CMD command, Docker container run hone par execute hone wale default command ko specify karta hai. Ye default command container run karte waqt command line arguments ke roop mein override kiya ja sakta hai.
Example:
dockerfile
FROM ubuntu:latest
RUN apt-get update && apt-get install -y python
RUN echo “Hello, Docker!” > /app/message.txt
CMD [“python”, “/app/my_script.py”]

    Yahan, CMD command ke andar diya gaya array ek command hai jo container run hone par execute hoga. Agar user ne koi command specify nahi kiya to, yeh default command run hoga. For example, my_script.py file ko run karne ke liye Python interpreter ka use kiya jayega.
Note: CMD aur RUN commands Dockerfile mein ek se zyada baar aayenge, lekin CMD keval ek hi baar aayega aur wo bhi Dockerfile ke end mein. RUN commands jitne baar aayenge, utne layers create honge Docker image mein, jabki CMD command keval default command ko specify karta hai.

====================================================================
Dockerfile:
Docker container build karne ke liye use kiya jata hai. Dockerfile ke through aap define karte hain ki container ke build process mein kis tarah ke steps honge, kis tarah ke dependencies install kiye jayenge, aur container ke runtime behaviour ko kaise configure kiya jayega.
====================================================================

Namespace: set of process
Definition: Namespace ek Linux kernel feature hai jo processes aur unke resources ko isolate karne mein madad karta hai. Har namespace ek specific resource type ko represent karta hai.
Types of Namespaces:
PID Namespace: Isolates process IDs (PIDs), allowing processes in different namespaces to have the same PID.
Network Namespace: Isolates network resources, such as network interfaces, IP addresses, and routing tables.
Mount Namespace: Isolates file system mount points.
UTS Namespace: Isolates the hostname and NIS domain name.
IPC Namespace: Isolates Inter-Process Communication resources like message queues and semaphores.
User Namespace: Isolates user and group IDs.
Namespace, containers ko ek dusre se alag karke, har container ko apne isolated environment mein run karne ki anumati deta hai.
Control Group (cgroup): container ko resource allocate karta hai
Definition: Cgroup, resources ko control aur limit karne ke liye use hota hai. Yeh ek mechanism hai jiska use CPU, memory, disk I/O, network bandwidth, aur dusre resources ke management mein hota hai.(cgroup ka kaam hota haoi jo bhi resource chahiye jasie cpu memory disk network bandwidth allocate karta hai)
Capabilities:
Resource Limiting: Cgroup allows you to set limits on resource usage for a group of processes.
Prioritization: You can prioritize resource allocation among different cgroups.
Accounting: It helps in tracking resource usage by processes within a cgroup.
Isolation: Cgroups isolate resources, preventing one set of processes from affecting others.
Cgroup, kisi bhi set of processes ke liye specific resource constraints set karne ka ek powerful tareeka hai, jisse overall system performance aur stability improve hoti hai.
In dono concepts ka use, particularly containers jaise technologies mein hota hai jisse applications ko ek isolated aur manageble environment milta hai.

=======================================================================

###How to create Docker registry in Nexus

Nexus Repository Manager, Sonatype ka ek open-source repository manager hai, jise organizations apne artifacts aur dependencies ko manage karne ke liye use karte hain. Nexus Professional Edition me Docker Registry support hota hai. Yahan main aapko Nexus Repository Manager 3 ke Docker Registry setup ke kuch steps provide kar raha hoon:
Step 1: Nexus Repository Manager Install Kare:
Nexus Repository Manager 3 download kare aur install kare.
Nexus ko start kare.
Step 2: Nexus Web Interface Access Kare:
Browser me http://localhost:8081/ open kare.
Nexus Web Interface me login kare. Default credentials hote hain:
Username: admin
Password: admin123
Step 3: Docker Registry Enable Kare:
Nexus Dashboard par jaye.
“Settings” icon par click kare (upar right corner me gear icon).
“Repositories” option select kare.
Left sidebar se “Repositories” section me “docker (group)” ko select kare.
Uske baad, “Enable Docker Support” option ko check kare.
Changes save kare.
Step 4: Docker Registry Repository Create Kare:
Dashboard par jaye.
Left sidebar se “Repositories” section me “Repositories” option par click kare.
“+” icon par click kare.
Choose a recipe me “docker (hosted)” select kare.
Fill out the repository details, jaise ki Name, HTTP Port, Docker V1/V2 Compatibility, Blob Store, etc.
Save kare.
Step 5: Docker Client Configuration:
Docker client ko configure kare, taaki vo Nexus Docker Registry se communicate kar sake.
Docker client ke configuration file (~/.docker/config.json) me authentication details add kare. Nexus Repository Manager ke Web Interface se milenge.
Example:
json
{
“auths”: {
“your-nexus-registry-url”: {
“auth”: “your-base64-encoded-username-and-password”
}
}
}
Base64-encoded username and password nikalne ke liye aap online tools ka use kar sakte hain ya khud encode kar sakte hain.
Docker client se Nexus Docker Registry me login kare:
bash
docker login your-nexus-registry-url

Step 6: Docker Image Push Kare:
Docker image ko build kare.
Usko Nexus Docker Registry par push kare:
bash
docker tag your-image your-nexus-registry-url/your-image
docker push your-nexus-registry-url/your-image

Yeh steps aapko Nexus Repository Manager me Docker Registry setup karne me madad karenge. Dhyan rahe ki actual steps thode alag ho sakte hain, isliye Nexus ke documentation ko bhi refer kare.

==**************************************=

==**************************************=

COPY Command:
COPY command files aur directories ko host system se container mein copy karne ke liye use hota hai. Iska basic syntax:
Dockerfile
COPY <source> <destination>

<source> host system par ya Docker build context mein specified file ya directory ka path hota hai, aur <destination> container ke file system mein copy hone wala path hota hai.
Dockerfile
COPY ./app /app

Example mein, host system par ./app directory ko container ke /app directory mein copy karega.
ADD Command:
ADD command bhi files aur directories ko copy karne ke liye use hota hai, lekin isme kuch extra features hote hain. Iska basic syntax:
Dockerfile
ADD <source> <destination>

ADD command files aur directories ko copy karne ke sath-sath URLs se data download karne aur TAR files extract karne ke liye bhi use hota hai.
Dockerfile
ADD http://example.com/file.txt /app/file.txt

Example mein, http://example.com/file.txt se data download karke container ke /app/file.txt mein save karega.

========================================================================

========================================================================

========================================================================

Extra Notes:

Docker run karne se lekar container up hone tak ke process ka flow kuch iss tarah hota hai:
Docker Daemon Start Hota Hai:
Jab aap docker run command execute karte hain, to Docker daemon start hota hai. Docker daemon ek background process hota hai jo Docker commands ko handle karta hai.
Docker Images Check Hote Hain:
Docker daemon Docker Hub ya local registry se specified image ko check karta hai. Agar woh image local system mein available nahi hoti hai, to use pull karke local cache mein save karta hai.
Container Create Hota Hai:
Docker daemon ab container create karta hai, jisme image se ek instance banaya jata hai. Is container mein runtime environment aur file system hota hai.
OCI Runtime (runC) Ka Use Hota Hai:
Docker daemon container ke liye runC (Open Container Initiative) ya kisi aur runtime engine ka use karta hai. RunC ek low-level runtime tool hai jo containers ko create, run, aur manage karta hai.
Namespace Aur cgroups Create Hote Hain:
Docker daemon namespaces aur cgroups ka use karke container ke liye isolation create karta hai. Ye isolation, container ko host system se alag karke ek independent environment provide karta hai.
Container Start Hota Hai:
Runtime engine (jaise runC) container ko start karta hai. Is process mein container ke specified commands, entrypoints, aur runtime configurations ko execute kiya jata hai.
Application Run Hota Hai:
Container ke andar specified commands ya entry points execute hote hain. Containerized application run hone lagta hai.
Logs Aur Output Display Hote Hain:
Container ke output aur logs Docker daemon ke through capture kiye jate hain. Aap docker logs command ka use karke in logs ko dekh sakte hain.
Container Background Mein Run Hota Hai (if specified):
Agar aapne container ko background mode mein run karne ke liye configure kiya hai, toh woh process background mein chalta rahega.
Yeh steps general flow hain, lekin har step ke beech mein detailed process aur interactions hote hain. Docker daemon, runtime engine (runC or other), namespaces, cgroups, aur containerized application ke beech mein complex interactions hoti hain jo containerization aur isolation ko ensure karte hain.

========================================================

Feature
Volume Mounts
Bind Mounts
tmpfs Mounts
Data Persistence
Persists data even if the container is removed.
Depends on the host filesystem. Persists data.
Data is temporary and does not persist.
Lifecycle
Data persists beyond the container’s lifecycle.
Depends on the host filesystem. Tied to the container’s lifecycle.
Data is temporary and exists only as long as the container is running.
Management
Managed by Docker. Easy to name and reference.
Easy to manage. Named volumes improve readability and usability.
Managed by Docker. No need for explicit naming.
Sharing Data
Can be easily shared between multiple containers.
Can be shared between containers and the host machine. Changes in one reflect in the other.
Not suitable for sharing data between containers or with the host.
Use Cases
Ideal for data that needs to persist between container restarts or be shared among multiple containers.
Useful for development environments, sharing code, or configurations.
Suitable for temporary storage needs within the container.
Syntax
docker run -v volume_name:/container/path …
docker run -v /host/path:/container/path …
docker run --tmpfs /container/path …
