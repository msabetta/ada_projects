# ada_projects
Sample projects in ada code on the job

# Installation (using CentOS 7)

$ sudo yum update <br>
$ sudo yum group install "Development Tools" <br>

# Display versions (gcc, gnatmake, git)

$ gcc --version <br>
$ gnatmake --version <br>
$ git --version <br>


# Clone Ada projects

$ git clone https://github.com/msabetta/ada_projects.git <br>
$ cd ada_projects/hello <br>

# Compile Ada project
$ gcc -c helloworld.adb <br>
$ gnatmake helloworld.adb <br>

# Execute helloworld binary
$ ./helloworld 

