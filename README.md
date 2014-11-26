GemRBAC
============
This project has been developed at the [SVV lab](http://www.svv.lu) of the [University of Luxembourg](http://wwwen.uni.lu) by [Ameni Ben Fadhel](http://wwwen.uni.lu/snt/people/ameni_ben_fadhel).

GemRBAC is a generalized model for Role-based Access Control that supports various types of RBAC authorization constraints:

* Prerequisite constraint
* Cardinality constraint
* Precedence and dependency constraint
* Role hierarchy constraint
* Separation of duty constraint (SoD)
* Binding of duty constraint (BoD)
* Role delegation and revocation constraint
* Context constraint

More information on GemRBAC is available in this technical report:

> Ameni Ben Fadhel, Domenico Bianculli, and Lionel Briand. __A
> Comprehensive Modeling Framework for Role-based Access Control
> Policies__. Technical Report TR-SnT-2014-15, SnT Centre - University
> of Luxembourg, November 2014.  Available online at http://hdl.handle.net/10993/18874

#Content
The project contains:

* The Ecore version of the GemRBAC model (*model/GemRBAC.ecore*)
* The formalization of the RBAC policies as OCL constraints (*model/constraints.ocl*)
* An instance of the GemRBAC model that satisfies all the RBAC policies (*satisfying-instance/validInstance.xmi*)
* For each RBAC policy, an instance that violates it (folder *violating-instances*)

#Requirements
* Ecoretools (http://eclipse.org/ecoretools/)
* Eclipse OCL (http://www.eclipse.org/modeling/mdt/?project=ocl)
