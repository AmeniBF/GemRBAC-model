GemRBAC
============
This project has been developed at the [SVV lab](http://www.svv.lu) of the [University of Luxembourg](http://wwwen.uni.lu) by [Ameni Ben Fadhel](http://wwwen.uni.lu/snt/people/ameni_ben_fadhel).

GemRBAC is a generalized model for Role-based Access Control that supports various types of RBAC authorization constraints.

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
  * Prerequisite constraint:
    * Prerequisite role: PreqPerm.xmi
    * Prerequisite permission: PreqRole.xmi
  * Cardinality constraint: CardUser.xmi
  * Precedence and dependency constraint: PrecEnabling.xmi, RoleActivationPrecedence.xmi
  * Role hierarchy constraint: RoleHierarchy.xmi, RoleHierarchyPermlevel.xmi
  * Separation of duty constraint (SoD):
    * Static SoD conflicting users: SSoDCU.xmi
    * Static SoD conflicting roles: SSoDCR.xmi
    * Static SoD permissions: SSoDCP1.xmi, SSoDCP2.xmi
    * Dynamic DSoD: DSoD.xmi
    * Object-based DSoD: ObjectDSoD.xmi
    * Operational-based DSoD: OpDSoD.xmi
    * Operational object-based DSoD: HistoryDSoD.xmi
  * Binding of duty constraint (BoD):
    * Role-based BoD: RoleBoD.xmi
    * Subject-based BoD: SubjectBoD.xmi
  * Role delegation and revocation constraint:
    * Strong transfer delegation: StrongTransfer.xmi
    * Static weak transfer: StaticWeakTransfer.xmi
    * Dynamic weak transfer: DynamicWeakTransfer.xmi
    * Total/partial delegation: PartialDelegation.xmi, TotalDelegation.xmi
    * Strong/weak revocation: StrongRevocation.xmi
    * Cascading/non cascading revocation: CascadingRevocation.xmi
    * Grant-dependent/ grant-independent revocation: Dependentrevocation.xmi

#Requirements
* Ecoretools (http://eclipse.org/ecoretools/)
* Eclipse OCL (http://www.eclipse.org/modeling/mdt/?project=ocl)
