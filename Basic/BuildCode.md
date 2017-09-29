
 
A - Alpha
E - Echo
D - Delta
T - Tango


# Building the Code
• The compilation of source code to native code or virtual machine bytecode, depending on our production platform. 
• Linting of the code: checking the code for errors and generating code quality measures by means of static code analysis. The term "Linting" originated with a program called Lint, which started shipping with early versions of the Unix operating system. The purpose of the program was to find bugs in programs that were syntactically correct, but contained suspicious code patterns that could be identified with a different process than compiling. 
• Unit testing, by running the code in a controlled manner. 
• The generation of artifacts suitable for deployment. 

#  faces of build systems 
• For Java, there is Maven, Gradle, and Ant 
• For C and C++, there is Make in many different flavors 
• For Clojure, a language on the JVM, there is Leiningen and Boot apart  from Maven 
• For JavaScript, there is Grunt 
• For Scala, there is sbt 
• For Ruby, we have Rake 
• Finally, of course, we have shell scripts of all kinds

##  Jenkins build server 


## Managing build dependencies 


## Build slaves 
To reduce build queues, you can add build slavMany build tools have the concept of a build tree where dependencies are built in the order required for the build to complete, since parts of the build might depend on other parts. es. The master server will send  builds to the slaves based on a round-robin scheme or tie specific builds to specific build slaves. The reason for this is usually that some builds have certain requirements on the host operating system. Build slaves can be used to increase the efficiency of parallel builds. They can also be used to build software on different operating systems. For instance, you can have a Linux Jenkins master server and Windows slaves for components that use Windows build tools. To build software for the Apple Mac, it's useful to have a Mac build slave, especially since Apple has quirky rules regarding the deployment of their operating system on virtual servers


## Triggers 
• Git repository polling can be used most of the time so that every check in triggers a build. 
• Nightly builds can be triggered, which are more stringent than continuous builds, and thus take a longer time. Since these builds happen at night when nobody is supposed to work, it doesn't matter if they are slow. 
• An upstream build can trigger a downstream build.


## Build servers and infrastructure as code 


## Building by dependency order
Many build tools have the concept of a build tree where dependencies are built in the order required for the build to complete, since parts of the build might depend on other parts. 


## Collating quality measures 


https://blog.axosoft.com/gitflow/
https://www.atlassian.com/git/tutorials/comparing-workflows
https://danielkummer.github.io/git-flow-cheatsheet/
https://datasift.github.io/gitflow/IntroducingGitFlow.html
http://nvie.com/posts/a-successful-git-branching-model/
https://datasift.github.io/gitflow/IntroducingGitFlow.html

https://www.git-tower.com/learn/git/ebook/en/desktop-gui/advanced-topics/git-flow
