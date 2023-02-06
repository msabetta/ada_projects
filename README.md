# ada_projects
Sample projects in ada code on the job

# Installation (using CentOS 7)

$ sudo yum update
$ sudo yum group install "Development Tools"

# Display versions (gcc, gnatmake, git)

$ gcc --version
$ gnatmake --version
$ git --version


# Clone Ada projects

$ git clone https://github.com/msabetta/ada_projects.git
$ cd ada_projects/hello

# Compile Ada project
$ gcc -c helloworld.adb
$ gnatmake helloworld.adb

# Execute helloworld binary
$ ./helloworld

