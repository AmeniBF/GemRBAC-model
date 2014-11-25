GeRBAC-model
============

In this project, we present the implementation of the GeRBAC model, a generalized RBAC model that supports the following RBAC policies:
* Prerequisite constraint
* Cardinality constraint
* Precedence and dependency constraint
* Role hierarchy constraint
* Separation of duty constraint (SoD)
* Binding of duty constraint (BoD)
* Role delegation and revocation constraint
* Context constraint

#Content
This project contains:

1. The GeRBAC model: RBACmodel.ecore
2. The formalization of RBAC policies as OCL constraints: constraints.ocl
3. An instance that satisfies all the RBAC policies: validModel.xmi
4. For each RBAC policy, an instance that violates it.

#Requirements
* Ecore Tools (http://download.eclipse.org/ecoretools/updates/)
* OCL Tool
