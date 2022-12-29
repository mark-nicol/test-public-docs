Overview of the Next Generation Observing Tool (ngOT)
=====================================================
The Next Generation OT consists of the following parts

.. uml:: ./diagrams/container view.puml

+--------------------------+-------------------------------------------------------------------------------------------+
| Component                | Description                                                                               |
+==========================+===========================================================================================+
| Users                    | There are two main groups of users of the ngOT:                                           |
|                          |                                                                                           |
|                          | * Astronomers wishing to create a proposal for                                            |
|                          |   the ALMA OT"                                                                            |
|                          |                                                                                           |
|                          | * Staff at the ALMA Observatory managing accepted                                         |
|                          |   observing proposals through their proposal lifecycle                                    |
+--------------------------+-------------------------------------------------------------------------------------------+
| ng Observing Tool        |  The Next Generation Observing Tool - the system being developed                          |
+--------------------------+-------------------------------------------------------------------------------------------+
| ngOT Client Application  | GUI created using Angular (a Typescript based framework)  with Data Driven Documents (D3) |
|                          | for more visual components.                                                               |
+--------------------------+-------------------------------------------------------------------------------------------+
| ngOT Services            | Java / Spring Boot based services running in docker containers orchestrated using Netflix |
|                          | developed services ( Eureka for service discovery and Zuul as a gateway)                  |
+--------------------------+-------------------------------------------------------------------------------------------+
| User  Store              | Storage for projects currently being created or edited by users within the ngOT           |
|                          | within a Redis database                                                                   |
+--------------------------+-------------------------------------------------------------------------------------------+
