# vRealize Suite Lifecycle Manager 2.0

vRealize Suite Lifecycle Manager automates install, configuration, upgrade, patch, configuration management, drift remediation and health from within a single pane of glass, thereby freeing IT Managers/Cloud admin resources to focus on business-critical initiatives, while improving time to value (TTV), reliability and consistency. Automates Day 0 to Day 2 operations of the entire vRealize Suite, enabling simplified operational experience for customers.

**What's new in 2.0?**
   1. Certificates
   2. Patching
   3. Filtering in content management
   4. vRops
   5. Notifications
   
   ![alt vRealize Suite Lifecycle Manager 2.0](https://raw.githubusercontent.com/Dipeshpal/vRealize-Suite/master/Raw/vRLCM.PNG)



**[Download  VMware vRealize Suite](https://my.vmware.com/group/vmware/info?slug=infrastructure_operations_management/vmware_vrealize_suite/2018)**

[Installation PDF](https://docs.vmware.com/en/VMware-vRealize-Suite-Lifecycle-Manager/2018/vrealize-lifecycle-manager-20-installation-upgrade-and-management.pdf)

## Deploy the vRealize Suite Lifecycle Manager Appliance-

   Deploy the vRealize Suite Lifecycle Manager appliance to begin using vRealize Suite Lifecycle Manager.
   To create the appliance, you use the vSphere Client to download and deploy a partially configured virtual machine from a template.

#### **Prerequisites**

  - Log in to the vSphere Client with an account that has permission to deploy OVF templates to the inventory.

  - [Download](https://my.vmware.com/group/vmware/details?downloadGroup=VRSLCM-200&productId=787&rPId=28204) vRealize Suite Lifecycle Manager .ovf or .ova file from My VMware to a location accessible to the vSphere Client.

#### Procedure-

1. Select the vSphere Deploy OVF Template.
2. Enter the path to the vRealize Suite Lifecycle Manager appliance .ovf or .ova file.
3. Read and accept the end-user license agreement.
4. Enter an appliance name and inventory location.
    Always deploy vRSLCM appliance with unique name and do not include non-alphanumeric characters such as underscores ( _ ) in the names.

5. Select the host and cluster in which the appliance will reside.
6. Review the template details.
7. Select the resource pool in which the appliance will reside.
8. Select a deployment configuration.
 
   Note: Enable this feature if you want to use content management, where the VA is deployed with 4 CPUs.
   Typically, there is an option to include or exclude content management. You can select a configuration and mention the change in the number of CPU that is required.

9. Select the storage that will host the appliance.

10. Select Thick as the disk format.
    Format does not affect appliance disk size. If an appliance needs more space for data, increase disk size by using vSphere after deploying.

11. From the drop-down menu, select a Destination Network.
12. Complete the appliance properties.
    - For Hostname, enter the appliance Fully Qualified Domain Name (FQDN).
    - (Optional) Enter the certificate properties.
    - In Network Properties, when using static IP addresses, enter the values for gateway, Netmask, and DNS servers. You must also enter the IP address, FQDN, and domain for the appliance itself.
    
    Note: vRealize Suite Lifecycle Manager does not verify the revocation status of the SSL certificates. You must verify the status manually before accepting the certificate.

13. Depending on your deployment, vCenter Server, and DNS configuration, select one of the following ways of finishing deployment and powering up the appliance.
    - If you deployed to vSphere, and Power on after deployment is available on the Ready to Complete page, take the following steps.

      - Select Power on after deployment and click Finish.

      - After the file finishes deploying into vCenter Server, click Close.

      - Wait for the virtual machine to start, which might take up to 5 minutes.

    - If you deployed to vSphere, and Power on after deployment is not available on the Ready to Complete page, take the following steps.

      - After the file finishes deploying into vCenter Server, click Close.

      - Power on the vRealize Suite Lifecycle Manager appliance.

      - Wait for the virtual machine to start, which might take up to 5 minutes.

14. Verify that the vRealize Suite Lifecycle Manager appliance is deployed by pinging its FQDN. If you cannot ping the appliance, restart the virtual machine.

    Wait for the virtual machine to start, which might take up to 5 minutes.

15. Verify that the vRealize Suite Lifecycle Manager appliance is deployed by pinging its FQDN.

Results

16. Log in to vRealize Suite Lifecycle Manager using a supported Web browser. 

