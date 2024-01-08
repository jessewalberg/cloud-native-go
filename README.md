# cloud-native-go

## What is a cloud native application?

If you are working at a company most likely you are or have been hearing the term cloud native.
For most of us including myself and in my company people would say it and I would have no idea what it meant
I don't think they did either

The cloud native computing foundation is a subfoundation of the linux foundation. -> [Cloud Native Definition](https://github.com/cncf/toc/blob/main/DEFINITION.md)

A cloud native application does'nt just live in the cloud. They are *Scalable*, *loosely coupled*, *resilient*, *manageable*, and *observable*

Now we have more things to define. What are those?

### Scalable
Scalability is "the ability of a system to continue to behave as expected in the face of significant upward or downward changes in demand" another way to say it is that the system can maintain its operating state no matter the load on the system. There are two different ways to scale a system. Vertically and Horizontally.

Vertical scaling means addign more resources to a current machine. This is generally more simple than horizontal scaling.

Horizontal scaling means creating more instances of the application/service. Horizontal scaling has the benefits of redundancy there is no theoretical cap on the resources of the machine because you could just add another machine
but for vertical scaling a machine can only be so powerful. However horizontal scaling adds complexity you have to manage state between different instances of the service along with growing management of the instances.

### Loosely Coupled

I dont care about you. You dont care about me. That is the general gist of loosely coupled. If I have two components that interact they should have minimal knowledge of the other. Changes to one should not require changes in the other.

### Resilient

How well can you handle errors and recover from faults?
No not you the computer! "A system can be considered resilient if it can continue operating correctly possible at a reduced level rather than failing completely when some part of the system fails"

### Manageability
"A systems manageability is the ease (or lack thereof) with which its behavior can be modifed to keep it secure, running smoothly, and compliant with changing requirements. A system can be considered manageable if its possible to sufficiently alter its behavior without having to alter its code."

### Observability
"The observability of a system is a measure of how well its internal states can be inferred from knowledge of its external outputs. A system can be considered observable when its possible to quickly and consistently ask novel questions about it with minimal prior knowledge and without having to reinstrument or build new code."

## Why go Rules the Cloud Native World

Features for a cloud native world and why go was the solution

Frustrations by the authors of the language were but not limited to
  - Low program comprehensibility
    - Code had become to hard to read. Unnecessary bookkeeping and repetition was compunded by functionally overlapping features that often encouraged cleverness over clarity.
  - Slow builds
    - Language construction and years of feature creep resulted in build times that ran for minutes or hours even on large build clusters.
  - Inefficiency
    - Many programmers responded to the aforementioned problems by adopting more fluid, dynamic languages, effectively trading efficiency and type safety for expressiveness
  - High Cost of Updates
    - Incompatibilities between even minor versions of a language, as well as any dependencies it may have often made updating an exercise in frustration


## Cloud Native Go Constructs
Gos basic data types are the building blocks from which more complext types are constructed
  - Booleans
  - Numeric Types
  - Strings
Go has 3 first class container types that can be used to store collections of element values
 - ArrayArray ( a fixed length sequence of zero or more elements of a particular type)
 - Slice (an abstraction around an array that can be resized at runtime)
 - Map (an associative data structure that allows distinct keys to be arbitrarily pairs with or mapped to values)

Go has one and one only loop structure...the for loop you can accomplish a while/do-while loop using the for loop
