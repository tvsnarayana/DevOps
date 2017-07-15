# Revision control system / source code management 

The revision control system is heart of the development environment.
The code that forms the organization's software products is stored here.
It is also common to store the configurations that form the infrastructure here. 
If you are working with hardware development, the designs might also be stored in the revision control system. 

##  need for source code control 
 The applications that we build 
 • The infrastructure that hosts our applications 
 • The documentation that documents our products 
Code and scripts for building the application.
•	Code and scripts for unit testing the application.
•	Code and scripts for acceptance testing the application.
•	Code and scripts for deploying the application.
•	Code and script conﬁguration options for conﬁguring the application for different target environments. 
Code and scripts for programming the attributes and “behavior” of the 	target environment.

# The Eight Commandments of Source Code Control
1. You shall check in early and check in often. You anger your coworkers when you check out a file and insist on keeping it checked out until some future point in time that is measured using variables that exist solely in your brain.
2. You shall never check in code that breaks the build. If you code does not compile, it does not belong in the source control repository.
3. You shall not go home for the day with files checked out, nor shall you depart for the weekend or for a vacation, with files checked out.
4. You shall leave a descriptive comment when checking in your code. You need not include your name or the date in the comment as that information is already tracked.
5. You shall use the 'Undo Checkout' option if you check out a file and do not make any changes. It displeases your coworkers when you check in code that has not changed at all from the original.
6. You shall not use comments to 'save' defunct code. Fear not, for the code you delete still exists in the source control code history and can be retrieved if needed.
7. You shall use source control for more than archiving just code. The source code control repository makes an excellent storage for technical docs, SQL scripts, and other documents and files related to the project.
8. You shall religiously backup your source code control database on a regular basis and store a copy in an off-site location.


# Choosing a branching strategy 
A branching strategy is a convention, or a set of rules, that describes when branches are created, how they are to be named, what use branches should have, and so on. Branching strategies are important when working together with other people and are, to a degree, less important when you are working on your own, but they still have a purpose.
Vincent Driessen formalized a branching strategy called Git flow, which has many good features


Git flow looks complex, so let's have a brief look at what the branches are for: 
• The **master** branch only contains finished work. All commits are tagged, since they represent releases. All releases happen from master. 
• The **develop** branch is where work on the next release happens. When work is finished here, develop is merged to master. 
• We use separate **feature** branches for all new features. Feature branches are merged to develop. 
• When a devastating bug is revealed in production, a **hotfix** branch is made where a bug fix is created. The hotfix branch is then merged to master, and a new release for production is made. 


Git flow is a centralized pattern, and as such, it's reminiscent of the workflows used with Subversion, CVS, and so on. The main difference is that using Git has some technical and efficiency-related advantages. Another strategy, called the forking pattern, where every developer has a central repository, is rarely used in practice within organizations, except when, for instance, external parties such as subcontractors are being employed. 

# Artifact version naming 
This usually translates to a version number with three or four parts: ° The first is major—changes here signal major changes in the code ° The second is for minor changes, which are backward API compatible ° The third is for bug fixes ° The fourth can be a build number While this might seem simple, it is a sufficiently complex area to have created a standardization effort in the form of SemVer, or Semantic Versioning. The full specification can be read at http://semver.org. 

Some tools don't work this way. Maven, the Java build tool, supports a snapshot release number. A snapshot can be seen as a version with a fuzzy last part. Snapshots have a couple of drawbacks, though; for instance, you can't immediately see which source code tag the artifact corresponds to. This makes debugging broken installations harder


# Code Review













# Build Server

Build server listen to changes in the revision control system. 
When a change is noticed, the build server updates its local copy of the source from the revision control system.
Then, it builds the source and performs optional tests to verify the quality of the changes. 
This process is called Continuous Integration. 
Unlike the situation for code repositories, there hasn't yet emerged a clear winner in the build server field. 


# Artifact repository 
When the build server has verified the quality of the code and compiled it into deliverables, it is useful to store the compiled binary artifacts in a repository.  
This is normally not the same as the revision control system. 
In essence, these binary code repositories are filesystems that are accessible over the HTTP protocol. 
Normally, they provide features for searching and indexing as well as storing metadata, such as various type identifiers and version information about the artifacts. 
In the Java world, a pretty common choice is Sonatype Nexus. Nexus is not limited to Java artifacts, such as Jars or Ears, but can also store artifacts of the operating system type, such as RPMs, artifacts suitable for JavaScript development, and so on. 
Amazon S3 is a key-value datastore that can be used to store binary artifacts. 
Some build systems, such as Atlassian Bamboo, can use Amazon S3 to store artifacts. 
The S3 protocol is open, and there are open source implementations that can be deployed inside your own network. 
One such possibility is the Ceph distributed filesystem, which provides an S3-compatible object store. 


# Package managers 
Linux servers usually employ systems for deployment that are similar in principle but have some differences in practice.
Red Hat-like systems use a package format called RPM. Debian-like systems use the .deb format, which is a different package format with similar abilities. The deliverables can then be installed on servers with a command that fetches them  from a binary repository. These commands are called package managers. On Red Hat systems, the command is called yum, or, more recently, dnf.  On Debian-like systems, it is called aptitude/dpkg. The great benefit of these package m
anagement systems is that it is easy to install and upgrade a package; dependencies are installed automatically. 

Directory structure conventions 
Branching strategy 
Release management 

 
 
 
 
 
 
 
 
 
 
 
 
 
 
