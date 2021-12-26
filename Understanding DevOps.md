# Understanding DevOps

Source : https://www.redhat.com/en/topics/devops#overview

---

DevOps means linking legacy apps with newer cloud-native apps and infrastructure.
 ### What is DevOps ?
 The **_"DevOps"_** is a combination of two words **"development"** and **"operations"** but it represents a set of ideas and practices much larger than those two terms alone, or together. DevOps includes security, collaborative ways of working, data analytics, and many other things.
 
### What do containers have to do with DevOps? 
DevOps speeds up how an idea goes from development to deployment. At its core, DevOps relies on automating routine operational tasks and standardizing environments across an app’s lifecycle. **Containers** can offer **standardized environments** , but you need a platform to manage them that also offers built-in automations and support for any infrastructure.

### DevOps process
 just changing your development and operations processes isn’t enough. You’ll need to apply systems thinking to really optimize the way you deliver software. This means DevOps will lead to changes in the business units that request dev work and in the groups that support the end users. A continuous cycle of feedback from end users to the business is the key.
 DevOps teams will often build their software using a microservices architecture and link these services together with APIs. Teams deliver faster by focusing on creating smaller pieces of functionality so you’ll have to focus on how those services and APIs are managed and have a strategy, like agile integration, for bringing it all together

### DevOps platform & tools
Selecting tools that support your processes is critical for DevOps to be successful. If your operations are going to keep pace with rapid development cycles they’ll need to use highly flexible platforms and treat their infrastructure like dev teams treat code.
Platform provisioning and deployment can be simplified through automation. **Site reliability engineering (SRE)** takes these manually operations tasks and manages them using software and automation. An SRE approach can further support the goals of a DevOps team.
Containers make it easier to move applications between development, testing, and production environments. Using containers lets developers package and isolate their apps with everything they need to run, including application files, runtime environments, dependent libraries and configurations https://www.redhat.com/en/topics/containers

### DevOps and Kubernetes
**The DevOps approach** goes hand-in-hand with Linux® containers, which give your team the underlying technology needed for a cloud-native development style. Containers support a unified environment for development, delivery, integration, and automation.
And **Kubernetes** is the modern way to automate Linux container operations. Kubernetes helps you easily and efficiently manage clusters running Linux containers across public, private, or hybrid clouds. 

Kubernetes (also known as k8s or “kube”) is an open source container orchestration platform that automates many of the manual processes involved in deploying, managing, and scaling containerized application
#### Build applications and manage containers using Kubernetes
Kubernetes is an open source container orchestration platform that helps manage _distributed, containerized applications at massive scale_. You tell **Kubernetes** where you want your software to run, and the platform takes care of almost everything else.
detail shows how Kubernetes helps organizations build applications and manage containers on site and across hybrid cloud environments. It provides:
- The origin, functions, and benefits of Kubernetes.
- Basics of modern application development and container management and orchestration.
- A look at basic Kubernetes architecture.
- Factors for you to consider when adopting Kubernetes.
- Information about how Red Hat® OpenShift® can help you simplify and scale Kubernetes applications.
[kubernete.pdf](https://github.com/akshaysinhparmar/Understanding-DevOps/files/7777008/kubernete.pdf)

#### What are Kubernetes clusters?
You can cluster together groups of hosts running **Linux® containers**, and Kubernetes helps you easily and efficiently manage those clusters.

Kubernetes clusters can span hosts across _on-premise, public, private, or hybrid clouds_. For this reason, Kubernetes is an ideal platform for hosting cloud-native applications that require **rapid scaling**, like **real-time data streaming** through **_Apache Kafka_**.

### DevOps helps you scale through continuous deployment
A major outcome of implementing DevOps is a ***continuous integration and continuous deployment pipeline (CI/CD)***. CI/CD helps you deliver apps to customers frequently and validate software quality with minimal human intervention.

Specifically, CI/CD introduces ongoing automation and continuous monitoring throughout the lifecycle of apps, from integration and testing phases to delivery and deployment, so you can quickly identify and correct problems and defects. Taken together, these connected practices are often referred to as a "CI/CD pipeline" and are supported by development and operations teams working together in an agile way
#### What is CI/CD?
CI/CD is a method to frequently deliver apps to customers by introducing automation into the stages of app development. The main concepts attributed to CI/CD are continuous integration, continuous delivery, and continuous deployment. CI/CD is a solution to the problems integrating new code can cause for development and operations teams (AKA "integration hell").
Specifically, CI/CD introduces ongoing automation and continuous monitoring throughout the lifecycle of apps, from integration and testing phases to delivery and deployment. Taken together, these connected practices are often referred to as a "CI/CD pipeline" and are supported by development and operations teams working together in an agile way with either a DevOps or site reliability engineering (SRE) approach.
#### What's the difference between CI and CD (and the other CD)?
The "CI" in CI/CD always refers to continuous integration, which is an automation process for developers. Successful CI means new code changes to an app are regularly built, tested, and merged to a shared repository. It’s a solution to the problem of having too many branches of an app in development at once that might conflict with each other.

The "CD" in CI/CD refers to continuous delivery and/or continuous deployment, which are related concepts that sometimes get used interchangeably. Both are about automating further stages of the pipeline, but they’re sometimes used separately to illustrate just how much automation is happening.

Continuous delivery usually means a developer’s changes to an application are automatically bug tested and uploaded to a repository (like GitHub or a container registry), where they can then be deployed to a live production environment by the operations team. It’s an answer to the problem of poor visibility and communication between dev and business teams. To that end, the purpose of continuous delivery is to ensure that it takes minimal effort to deploy new code.

Continuous deployment (the other possible "CD") can refer to automatically releasing a developer’s changes from the repository to production, where it is usable by customers. It addresses the problem of overloading operations teams with manual processes that slow down app delivery. It builds on the benefits of continuous delivery by automating the next stage in the pipeline.
![image](https://user-images.githubusercontent.com/48562260/147413307-11937b29-192a-4842-a9dc-75bfe39fff5a.png)

It’s possible for CI/CD to specify just the connected practices of continuous integration and continuous delivery, or it can also mean all 3 connected practices of continuous integration, continuous delivery, and continuous deployment. To make it more complicated, sometimes "continuous delivery" is used in a way that encompasses the processes of continuous deployment as well.
CI/CD is really a process, often visualized as a pipeline, that involves adding a high degree of ongoing automation and continuous monitoring to app development.

#### What are some common CI/CD tools?
CI/CD tools can help a team automate their development, deployment, and testing. Some tools specifically handle the integration (CI) side, some manage development and deployment (CD), while others specialize in continuous testing or related functions.
One of the best known open source tools for CI/CD is the automation server** Jenkins**. Jenkins is designed to handle anything from a simple CI server to a complete CD hub.

Deploying Jenkins on Red Hat OpenShift 
https://cloud.redhat.com/blog/deploying-jenkins-on-openshift-part-1?extIdCarryOver=true&intcmp=7013a000002wBnmAAE&sc_cid=7013a000002DgC5AAK%27]]

Tekton Pipelines is a CI/CD framework for Kubernetes platforms that provides a standard cloud-native CI/CD experience with containe

Beyond Jenkins and Tekton Pipelines, other open source CI/CD tools you may wish to investigate include:
- Spinnaker, a CD platform built for multicloud environments.
- GoCD, a CI/CD server with an emphasis on modeling and visualization.
- Concourse, "an open-source continuous thing-doer."
- Screwdriver, a build platform designed for CD.

Teams may also want to consider **managed CI/CD tools,** which are available from a variety of vendors. The major public cloud providers all offer CI/CD solutions, along with GitLab, CircleCI, Travis CI, Atlassian Bamboo, and many others.
Additionally, any tool that’s foundational to DevOps is likely to be part of a CI/CD process. Tools for configuration automation (such as Ansible, Chef, and Puppet), container runtimes (such as Docker, rkt, and cri-o), and container orchestration (Kubernetes) aren’t strictly CI/CD tools, but they’ll show up in many CI/CD workflows

### DevOps and Security
DevOps isn’t just about development and operations teams. In order to take full advantage of a DevOps approach, organizations must consider how security plays a role in the life cycle of their apps. This means thinking about core security from the planning phase onward. It also means automating some security features to keep the DevOps workflow from slowing down. Selecting the right tools to integrate security can help meet your DevOps security goals.

But effective DevOps security requires more than new tools—it builds on the cultural changes of DevOps to integrate the work of security teams sooner rather than later. DevOps speeds things up by closing the gap between development and operations, but the speed gained can be undermined by poor security planning.

Security used to be the exclusive responsibility of an isolated team—tacked on in the final stage of development. Now, in a collaborative DevOps framework, security is a shared responsibility, integrated from the start.
https://youtu.be/FLAWDU6hpGM
