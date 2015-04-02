naoqi-nao-development
=====================

Development journal for nao robots (with Dr. Flores). This project aims to learn and implement as much of the NAOqi SDK as possible.

###Downloads

- [Download the SDK](https://community.aldebaran.com/en/resources/software)

###Resources

- [NAOqi SDK](http://doc.aldebaran.com/2-1/ref/index.html)
- [NAOqi Python SDK](http://doc.aldebaran.com/2-1/dev/python/index.html)
- [NAOqi Java SDK](http://doc.aldebaran.com/2-1/dev/java/index_java.html)
- [Hello World (C++)](http://doc.aldebaran.com/2-1/dev/cpp/examples/core/helloworld/example.html)
- [Capturing audio and video](http://doc.aldebaran.com/2-1/dev/cpp/examples/audiovideocapture/audiovideocapture.html#cpp-examples-audiovideocapture)

### Modules list

The following, are `C++` modules that have been completed by the team so far.

- `hello`
- `face`
- `video` (work in progress)

### Running Modules

This repo comes with a few `C++` modules, `hello` and `face` are two of them. To get started, make sure you have `naoqi-sdk-2.1.2.17` installed, and your `qitoolchain` is configured to use it.

- Make sure you have `qibuild` and `qisrc` installed. Clone this repository, and `cd` into it.
- Then, add the two modules (that should already be present in your current folder) to the `worktree` by typing `qisrc add <module_name>`
- Then, link all dependencies to the module by typing `qibuild configure <module_name>`
- Finally, build the module by typing `qibuild make <module_name>`

To run a module, simply type `qibuild run <module_name>`. Please note that if the module is a remote module (pretty much all of them are), you will need to pass arguments to it when running it, specifying the **IP address** of the robot. To do so, run it by typing `qibuild run <module_name> -- --pip <IP_ADDRESS>`. 

A detailed guide on setting up your work environment, and builing modules from scratch will be posted in the `docs` soon.

###Project members

- Juan Vallejo
- Jake Hayhurst
- Amanda Lee