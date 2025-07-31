# Ensuring Compliance with Azure Policies


<h2>Project Details</h2>
This lab focused on implementing Azure Policy to enforce governance and ensure resource compliance within an Azure environment. Acting as an Azure security engineer, I explored how to assign policies that enforce tagging standards and automate tag inheritance. The lab provided hands-on experience in policy assignment, resource deployment, and remediation, reinforcing best practices for organizational compliance and cost management.<br />
<br />

**Tasks Breakdown:**

**Task 1: Assigning a Policy to Require Cost Allocation Tags on Resource Groups**

A policy was assigned to enforce the presence of a "Cost Allocation" tag on all resource groups. This ensures that financial reporting and chargeback mechanisms are consistently applied across the organization.

**Task 2: Assigning a Policy to Inherit Tags from Resource Groups**

A second policy was configured to automatically inherit the "Cost Allocation" tag from the parent resource group to any child resources. This included setting up a user-assigned managed identity to support remediation tasks.

**Task 3: Tagging the Resource Group**

The resource group used in the lab was manually tagged with the "Cost Allocation" tag, with a value of "IT", to comply with the newly assigned policies.

**Task 4: Creating a Non-Compliant Virtual Network**

A virtual network named PolicyVnet2 was created without a "Cost Allocation" tag to test the effectiveness of the inheritance policy. The resource was deployed in the same region as the resource group.

**Task 5: Observing Policy Behavior**

The lab demonstrated how PolicyVnet2 automatically inherited the "Cost Allocation" tag from its parent resource group, while PolicyVnet1, created before the policy assignment, remained non-compliant.

**Task 6: Remediating Existing Resources**

A remediation task was initiated to bring PolicyVnet1 into compliance. After completion, the resource successfully inherited the required tag, validating the policy's remediation capabilities.

<br />

**Key Takeaways:**

This lab provided a practical overview of Azure Policy for resource governance. Key skills developed include:

- Assigning and configuring Azure policies
- Enforcing tagging standards for cost management
- Automating tag inheritance across resources
- Remediating non-compliant resources
- Strengthening compliance and governance in cloud environments

These capabilities are essential for cloud security engineers, IT administrators, and compliance officers managing large-scale Azure deployments.

<br />


<h2>Softwares and Utilities Used</h2>

- <b>Microsoft Azure Portal: Used for policy assignment, resource provisioning, and remediation.</b>
- <b>Azure Policy: Central tool for defining and enforcing compliance rules.</b>
- <b>Azure Virtual Networks: Target resources for policy testing and validation.</b>

  

<h2>Environments Used </h2>

- <b>Azure Cloud Environment: All tasks were performed within the Azure ecosystem, leveraging native tools for policy management, identity configuration, and resource deployment.

</b>

<h2>Program walk-through:</h2>




<p align="center">
Task 1: Assigning a Policy to Require Cost Allocation Tags on Resource Groups <br/>
<br />
<br />
<img src="https://i.imgur.com/bunTCG9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/6bno691.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/yHTYJVc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/QZ1xfUh.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/u3VcVn9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/GuzRJMy.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/B9LmAz7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/s6Ayb9M.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/Jar8smX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/nH9QTjP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<p align="center">
Task 2: Assigning a Policy to Inherit Tags from Resource Groups <br/>
<br />
<br />
<img src="https://i.imgur.com/7gYcqN5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/zcnha3F.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/LgGNFlI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/zqDl8ZT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/jm2DpfW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/CpB4Z0r.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/oFaGr3n.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<br />
  
<p align="center">
Task 3: Tagging the Resource Group <br/>
<br />
<br />
<img src="https://i.imgur.com/TOt3A6E.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/IAVVOPO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/jEuyj7h.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<br />
<br />
<br />
Task 4: Creating a Non-Compliant Virtual Network  <br/>
<br />
<img src="https://i.imgur.com/TVGjaJ4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/3UvCpr8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/jkewm6W.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/fJltL1I.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/ETlsmvk.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/EO8GSSk.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/rd08Ham.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/M0flrrZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/gyKwslc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />


<br />
<br />
Task 5: Observing Policy Behavior  <br/>
<br />
<img src="https://i.imgur.com/2oPtWAi.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/5Xk5EfH.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/excau2L.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/YNuEbeQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/8gNZuA2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/Sf8VLyn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/I8xSB4k.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/F8i29yC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/QD4PTBY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<br />
<br />
<br />
Task 6: Remediating Existing Resources  <br/>
<br />
<img src="https://i.imgur.com/xZTaHiw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br />
<img src="https://i.imgur.com/HD3uy3S.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br />
<img src="https://i.imgur.com/3hRAGcs.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br />
<img src="https://i.imgur.com/jdPE6NZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br />
<img src="https://i.imgur.com/c4vg2fl.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br />
<img src="https://i.imgur.com/G6oxNWP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br />
<img src="https://i.imgur.com/wmWxSQo.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br />
<img src="https://i.imgur.com/i2ULaA8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br />
<img src="https://i.imgur.com/2F4kOeb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br />
<img src="https://i.imgur.com/FfGGiFL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br />
<img src="https://i.imgur.com/4JcAbcY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br />
<img src="https://i.imgur.com/D6eTdnB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br />
<img src="https://i.imgur.com/akXlqzZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br />
<img src="https://i.imgur.com/5d4K8Ln.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br />
<img src="https://i.imgur.com/hP6JJR2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br />
<img src="https://i.imgur.com/FtrzrqN.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br />
<img src="https://i.imgur.com/Ic9WOca.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br />
<img src="https://i.imgur.com/SrQTyb1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


<br />
<br />
<br />
<br />
<br />
<img src="https://i.imgur.com/OzWZ6Oh.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />










<br />
<br />

</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
