# Multi Stage Docker Build

The main purpose of choosing a golang based applciation to demostrate this example is golang is a statically-typed programming language that does not require a runtime in the traditional sense. Unlike dynamically-typed languages like Python, Ruby, and JavaScript, which rely on a runtime environment to execute their code, Go compiles directly to machine code, which can then be executed directly by the operating system.

So the real advantage of multi stage docker build and distro less images can be understand with a drastic decrease in the Image size.


With distro less images we only not reduce the size of our docker image but we also make it more secure.

A multi-stage build in Docker is a feature that allows you to create more efficient and smaller Docker images by using multiple "stages" within a single Dockerfile. Each stage represents a phase in the build process, and Docker allows you to copy artifacts or intermediate files from one stage to another.
Benefits of using multi-stage builds include:

Smaller Image Sizes: By separating the build environment from the runtime environment, you can significantly reduce the size of your final Docker image.

Reduced Attack Surface: Since only necessary files and dependencies are included in the final image, the attack surface is minimized.

Simpler Build Process: Multi-stage builds can make your Dockerfile easier to understand and maintain by separating different phases of the build proces
