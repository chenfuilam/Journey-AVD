# Pre-requisites to deploy Azure Virtual Desktop

- To deploy Azure Virtual Desktop environment, we need a Windows Active Directory (for example: contoso.com). This can be achieved using one of the following ways:

    1. Azure Active Directory Domain Services(AADDS) - you may refer to this ARM template in deploying AADDS, https://github.com/Azure/azure-quickstart-templates/tree/master/quickstarts/microsoft.network/aad-domainservices
    2. Windows Active Directory - you may refer to this ARM template in deploying ADDS, https://github.com/PeterR-msft/M365AVDWS/tree/master/AAD-Hybrid-Lab


- The domain name will be the suffix of your lab user account (for example: If your lab user account is ***odl_user_189588@azurehol1057.onmicrosoft.com***, the domain will be ***azurehol1057.onmicrosoft.com***.) 

- When you provision Azure ADDS, it creates a group named "AAD DC Administrators" in Azure Active Directory. Members of this group are allowed to be able to join AVD Sessions Hosts to Azure ADDS.  Your lab account is already a member of this group. 


