# Install and Setup Overview

The installation and the setup of API Manager involve installing the product, deploying it in the method that is best suited for your requirements, and setting it up to run in the production environment. If you already have an older version of WSO2 API Manager or one of its components, you can follow the upgrading instructions in this guide.

This section provides installation and setup instructions for the following three components of WSO2 API Manager that you need to operate as three separate runtimes.

## API Manager

This component manages APIs. To install and set up this component, see the following topics.

### Installing

To install and run the API Manager in virtual machines, see the following topics.

<table>
    <tr>
        <th>
            <a href="{{base_path}}/install-and-setup/install/installing-the-product/installing-api-m-runtime">Installing the API Manager Runtime</a>
        </th>
        <td>
            Explains how to download the API Manager component as a binary and install it on a virtual machine.
        </td>
    </tr>  
    <tr>
        <th>
            <a href="{{base_path}}/install-and-setup/install/installing-the-product/running-the-api-m">Running the API-M Runtime</a>
        </th>
        <td>
            Explains how you can execute the API-M runtime and start using its features.
        </td>
    </tr> 
    <tr>
        <th>
            <a href="{{base_path}}/install-and-setup/install/installing-the-product/installing-api-m-as-a-linux-service">Running API-M as a Linux Service</a>
        </th>
        <td>
            Explains how to install and run the API Manager as a Linux service.
        </td>
    </tr>
    <tr>
        <th>
            <a href="{{base_path}}/install-and-setup/install/installing-the-product/installing-api-m-as-a-windows-service">Running API-M as a Windows Service</a>
        </th>
        <td>
            Explains how to install and run the API Manager as a Windows service.
        </td>
    </tr> 
</table>

### Setting up

To set up the API Manager component, see the following topics.

<table>
<tr>
    <th>
        <a href="{{base_path}}/administer/updating-wso2-api-manager">Applying WSO2 WUM Updates</a>
    </th>
    <td>
        Explains how to get the latest updates that are available for a particular release of the API Manager.
    </td>
</tr>
<tr>
    <th>
        <a>Setting up a Key Manager</a>
    </th>
    <td>
        The key manager of the API Manager handles all clients, security, and access token-related operations. This section covers the following topics:
        <ul>
            <li>
                <a href="{{base_path}}/install-and-setup/setup/distributed-deployment/configure-a-third-party-key-manager">Configure a Third-party Key Manager</a>
            </li>
            <li>
                <a href="{{base_path}}/install-and-setup/setup/distributed-deployment/configuring-wso2-identity-server-as-a-key-manager">Configuring WSO2 Identity Server as a Key Manager</a>
            </li>
        </ul>
    </td>
</tr>
<tr>
    <th>
        <a href="{{base_path}}/install-and-setup/setup/setting-up-databases/overview">Setting up Databases</a>
    </th>
    <td>
        The API Manager is shipped with an H2 database for storing data. This guide explains the default H2 databases used within API Manager as well as how to switch to a different database supported for the API Manager such as MSSQL, MySQL, PostgreSQL, Oracle, MariaDB, IBM DB2, and Oracle RAC. In addition, this section covers how to manage data growth and improve performance when storing metadata and runtime data in databases.
    </td>
</tr>
<tr>
    <th>
        <a>Setting up Proxy Server and the Load Balancer
    <td>
        A load balancer or reverse proxy is required to map external traffic with ports and URLs that the APi Manager component uses internally. This section covers the following topics relating to the proxy server and the load balancer.
        <ul>
            <li>
                <a href="{{base_path}}/install-and-setup/setup/setting-up-proxy-server-and-the-load-balancer/configuring-the-proxy-server-and-the-load-balancer">Configuring the Proxy Server and the Load Balancer</a>
            </li>
            <li>
                <a href="{{base_path}}/install-and-setup/setup/setting-up-proxy-server-and-the-load-balancer/adding-a-custom-proxy-path">Adding a Custom Proxy Path</a>
            </li>
        </ul>
    </td>
</tr>
<tr>
    <th>
        <a>Securing the API Manager</a>
    </th>
    <td>
        Covers the different ways in which you can secure the API Manager and the data it handles. The topics covered are as follows:
        <ul>
            <li>
                <a>Logins and Passwords</a>
            </li>
                <li>
                    <a href="{{base_path}}/install-and-setup/setup/security/logins-and-passwords/maintaining-logins-and-passwords">Maintaining Logins and Passwords</a>
                </li>
                <li>
                    <a>Securing Passwords</a>
                </li>
                    <li>
                        <a href="{{base_path}}/install-and-setup/setup/security/logins-and-passwords/carbon-secure-vault-implementation">Customizing Secure Vault</a>
                    </li>
                    <li>
                        <a href="{{base_path}}/install-and-setup/setup/security/logins-and-passwords/set-passwords-using-vars-and-sys-props">Set Passwords using Environment Variables/System Properties</a>
                    </li>
                    <li>
                        <a href="{{base_path}}/install-and-setup/setup/security/logins-and-passwords/working-with-encrypted-passwords">Working with Encrypted Passwords</a>
                    </li>
            <li>
                <a>Configuring Keystores</a>
            </li>
                <li>
                    <a href="{{base_path}}/install-and-setup/setup/security/configuring-keystores/configuring-keystores-in-wso2-api-manager">Configuring Keystores in API Manager</a>
                </li>
                <li>
                    <a>Keystore Basics</a>
                </li>
                    <li>
                        <a href="{{base_path}}/install-and-setup/setup/security/configuring-keystores/keystore-basics/creating-new-keystores">Creating a New Keystore</a>
                    </li>
                    <li>
                        <a href="{{base_path}}/install-and-setup/setup/security/configuring-keystores/keystore-basics/renewing-a-ca-signed-certificate-in-a-keystore">Renewing a CA Signed Certificate</a>
                    </li>
                    <li>
                        <a href="{{base_path}}/install-and-setup/setup/security/configuring-keystores/keystore-basics/about-asymetric-cryptography">About Asymetric Cryptography</a>
                    </li>
            <li>
                <a href="{{base_path}}/install-and-setup/setup/security/enabling-hostname-verification">Enabling HostName Verification</a>
            </li>
            <li>
                <a href="{{base_path}}/install-and-setup/setup/security/enabling-java-security-manager">Enabling Java Security Manager</a>
            </li>
            <li>
                <a href="{{base_path}}/install-and-setup/setup/security/general-data-protection-regulation-gdpr-for-wso2-api-manager">General Data Protection Regulation (GDPR) for WSO2 API Manager</a>
            </li>
            <li>
                <a href="{{base_path}}/install-and-setup/setup/security/configuring-transport-level-security">Configuring Transport Level Security</a>
            </li>
            <li>
                <a href="{{base_path}}/install-and-setup/setup/security/user-account-management">User Account Management</a>
            </li>                                                                                      
        </ul>
    </td>
</tr>
<tr>
    <th>
        <a href="{{base_path}}/administer/managing-users-and-roles/managing-user-stores/introduction-to-userstores">Configuring User Stores</a>
    </th>
    <td>
        You can configure primary user stores as well as secondary user stores for the API Manager component. This section explains the concept of user stores and provides instructions to configure primary user stores. The topics covered are as follows:
        <ul>
            <li>
                <a href="{{base_path}}/administer/managing-users-and-roles/managing-user-stores/introduction-to-userstores">Introduction to User Stores</a>
            </li>
                <li>
                    <a href="{{base_path}}/administer/managing-users-and-roles/managing-user-stores/configure-primary-user-store/configuring-the-primary-user-store"> Configuring Primary User Stores</a>
                </li>
                <li>
                    <a href="{{base_path}}/administer/managing-users-and-roles/managing-user-stores/configure-primary-user-store/configuring-a-jdbc-user-store">Configuring a JDBC User Store</a>
                </li>
                <li>
                    <a href="{{base_path}}/administer/managing-users-and-roles/managing-user-stores/configure-primary-user-store/configuring-a-read-write-ldap-user-store">Configuring a Read-Write LDAP User Store</a>
                </li>   
                <li>
                    <a href="{{base_path}}/administer/managing-users-and-roles/managing-user-stores/configure-primary-user-store/configuring-a-read-only-ldap-user-store"> Configuring a Read-Only LDAP User Store</a>
                </li>
                <li>
                    <a href="{{base_path}}/administer/managing-users-and-roles/managing-user-stores/configure-primary-user-store/configuring-a-read-write-active-directory-user-store">Configuring a Read-Write Active Directory User Store</a>
                </li>
        </ul>                                                                       
    </td>
</tr>
<tr>
    <th>
        <a>SSO</a>
    </th>
    <td>
        Explains how to configure SSO (Single Sign On) for the API Manager component with an external identity provider. The topics covered are as follows.
        <li>
            <a href="{{base_path}}/install-and-setup/setup/sso/configuring-identity-server-as-external-idp-using-oidc">Configuring Identity Server As External IDP with OIDC</a>
        </li>
        <li>
            <a href="{{base_path}}/install-and-setup/setup/sso/configuring-identity-server-as-external-idp-using-saml">Configuring Identity Server As External IDP with SAML</a>
        </li>
        <li>
            <a href="{{base_path}}/install-and-setup/setup/sso/okta-as-an-external-idp-using-oidc">Using OKTA As An External IDP With OIDC</a>
        </li>
        <li>
            <a href="{{base_path}}/install-and-setup/setup/sso/okta-as-an-external-idp-using-saml">Using OKTA As An External IDP With SAML</a>
        </li>                                   
    </td>
</tr>   
<tr>
    <th>
        <a>Advanced Configurations</a>
    </th>
    <td>
        Covers some advance configurations including how to change the transport used by the API Manager component from the default PassThrough transport to a different transport, how to configure caching, and how to change the user interfaces of the API Manager component.
        <li>
            <a href="{{base_path}}/install-and-setup/setup/advance-configurations/changing-the-default-transport">Changing the Default Transport</a>
        </li>
        <li>
            <a href="{{base_path}}/install-and-setup/setup/advance-configurations/configuring-caching">Configuring Caching</a>
        </li>
        <li>
            <a href="{{base_path}}/install-and-setup/setup/advance-configurations/customizing-the-management-console">Customizing the Management Console</a>
        </li>                   
    </td>
</tr>
</table>
 
### Deploying

To deploy the API Manager runtime, see the topics given below.

<table>
    <tr>
        <th>
            <a href="{{base_path}}/install-and-setup/setup/deployment-overview">Deployment Patterns</a>
        </th>
        <td>
            This explains all the deployment patterns you can follow when you deploy WSO2 API manager. These patterns involve deploying the API Manager component together with Micro Integrator and Streaming Integrator components in clustered setups.
        </td>
    </tr>
    <tr>
        <th>
            <a href="{{base_path}}/install-and-setup/setup/single-node/all-in-one-deployment-overview">All-in-One Deployment</a>
        </th>
        <td>
            This describes the all-in-one deployment patterns where you can deploy all the sub components of the API Manager component in one instance.
        </td>
    </tr>
    <tr>
        <th>
            <a href="{{base_path}}/install-and-setup/setup/distributed-deployment/understanding-the-distributed-deployment-of-wso2-api-m">Distributed Deployment</a>
        </th>
        <td>
            This describes the distributed deployment patterns where you can deploy the sub-components of the API Manager component in a distributed manner in order to handle a high volume of requests in an efficient manner.
        </td>
    </tr>
    <tr>
        <th>
            <a href="{{base_path}}/install-and-setup/install/deploying-api-manager-with-kubernetes-or-openshift-resources">Deploy API-M on Kubernetes using Helm Resources</a>
        </th>
        <td>
            Explains how Helm resources deploy the API Manager component in Kubernetes.
        </td>
    </tr>
    <tr>
        <th>
            <a href="{{base_path}}/install-and-setup/setup/kubernetes-operators/k8s-api-operator/manage-apis/api-deployments">Deploy APIs on Kubernetes</a>
        </th>
        <td>
            Explains how the Kubernetes operator can deploy APIs in Kubernetes as managed APIs.
        </td>
    </tr>
</table>

### CI/CD

To implement continuous integration and continuous deployment pipelines for APIs on API Manager, see the topics given below.

<table>
    <tr>
        <th>
            <a href="{{base_path}}/install-and-setup/setup/api-controller/ci-cd-with-wso2-api-management">CI/CD for APIs - Overview</a>
        </th>
        <td>
            Find out about the methods of implementing CI/CD for APIs using the API Controller (apictl).
        </td>
    </tr>
     <tr>
        <th>
            <a href="{{base_path}}/install-and-setup/setup/api-controller/cicd-using-cli">Building a CI/CD Pipeline for APIs using the CLI</a>
        </th>
        <td>
            See the instructions on how to implement a CI/CD pipeline for APIs using the API Controller (apictl).
        </td>
    </tr>
    <tr>
        <th>
            <a href="{{base_path}}/install-and-setup/setup/api-controller/building-jenkins-ci-cd-pipeline-for-dev-first-approach">Building a CI/CD Pipeline for APIs using Jenkins</a>
        </th>
        <td>
            See the instructions on how to implement a CI/CD pipeline for APIs using Jenkins and the API Controller (apictl).
        </td>
    </tr>
</table>

See the topics given below to manage APIs, API products, Apps, etc. in the API-M runtime by using the API Controller (apictl).

<table>
    <tr>
        <th>
            <a href="{{base_path}}/install-and-setup/setup/api-controller/getting-started-with-wso2-api-controller">Getting Started with WSO2 API Controller</a>
        </th>
        <td>
            Explains how to set up the API Controller.
        </td>
    </tr>
    <tr>
        <th>
            <a>Managing APIs and API Products</a>
        </th>
        <td>
            This section covers the following topics.
            <li>
                <a href="{{base_path}}/install-and-setup/setup/api-controller/managing-apis-api-products/managing-apis-and-api-products">Managing APIs and API Products</a>
            </li>
            <li>
                <a href="{{base_path}}/install-and-setup/setup/api-controller/managing-apis-api-products/importing-apis-via-dev-first-approach">Importing APIs Via Dev First Approach</a>
            </li>
            <li>
                <a href="{{base_path}}/install-and-setup/setup/api-controller/managing-apis-api-products/migrating-apis-to-different-environments">Migrating APIs to Different Environments</a>
            </li> 
            <li>
                <a href="{{base_path}}/install-and-setup/setup/api-controller/managing-apis-api-products/migrating-api-products-to-different-environments">Migrating API Products (with or without dependent APIs) to Different Environments</a>
            </li>       
        </td>
    </tr>
    <tr>
        <th>
            <a>Managing Applications</a>
        </th>
        <td>
            This section covers the following topics.
            <li>
                <a href="{{base_path}}/install-and-setup/setup/api-controller/managing-applications/managing-applications">Managing Applications</a>
            </li>
            <li>
                <a href="{{base_path}}/install-and-setup/setup/api-controller/managing-applications/migrating-applications-to-different-environments">Migrating Apps to Different Environments</a>
            </li>                
        </td>
    </tr>
    <tr>
        <th>
            <a>Advanced Topics</a>
        </th>
        <td>
            This section covers the following topics.
            <li>
                <a href="{{base_path}}/install-and-setup/setup/api-controller/advanced-topics/creating-custom-users-to-perform-api-controller-operations">Creating Custom Users to Perform API Controller Operations</a>
            </li>
            <li>
                <a href="{{base_path}}/install-and-setup/setup/api-controller/advanced-topics/configuring-environment-specific-parameters">Configuring Environment Specific Parameters</a>
            </li>
            <li>
                <a href="{{base_path}}/install-and-setup/setup/api-controller/advanced-topics/using-dynamic-data-in-api-controller-projects">Using Dynamic Data in API Controller Projects</a>
            </li>
            <li>
                <a href="{{base_path}}/install-and-setup/setup/api-controller/advanced-topics/configuring-different-endpoint-types">Configuring Different Endpoint Types</a>
            </li>
            <li>
                <a href="{{base_path}}/install-and-setup/setup/api-controller/advanced-topics/formatting-the-output-of-get-command">Formatting the outputs of get commands</a>
            </li>                        
        </td>
    </tr>
</table>

### Upgrading

To upgrade to the current API Manager component from a previous version refer [Upgrade WSO2 API Manager]({{base_path}}/install-and-setup/upgrading-wso2-api-manager/upgrading-api-manager/).


## Streaming Integrator

This component develops streaming solutions that can be exposed as managed APIs asynchronously.

### Installing

To install and run the Streaming Integrator, see the following topics.

<table>
    <tr>
        <th>
            <a href="{{base_path}}/install-and-setup/install/installing-the-product/installing-si">Installing the Streaming Integrator Runtime</a>
        </th>
        <td>
            Explains how to download the Streaming Integrator runtime as a binary and install it on a virtual machine.
        </td>
    </tr>   
    <tr>
        <th>
            <a href="{{base_path}}/install-and-setup/install/installing-the-product/running-the-si">Running the Streaming Integrator Runtime</a>
        </th>
        <td>
            Explains how you can execute the Streaming Integrator runtime and start using its features.
        </td>
    </tr> 
    <tr>
        <th>
            <a href="{{base_path}}/install-and-setup/install/installing-the-product/installing-si-as-a-linux-service">Running the Streaming Integrator as a Linux Service</a>
        </th>
        <td>
            Explains how to install and run the Streaming Integrator as a Linux service.
        </td>
    </tr>
    <tr>
        <th>
            <a href="{{base_path}}/install-and-setup/install/installing-the-product/installing-si-as-a-windows-service">Running the Streaming Integrator as a Windows Service</a>
        </th>
        <td>
            Explains how to install and run the Streaming Integrator as a Windows service.
        </td>
    </tr>
    <tr>
		<th>
			<a>Installing the Streaming Integrator on Containers</a>
		</th>
		<td>
			Explains how to install the Streaming Integrator component in different containerized environments. The topics covered are as follows:
			<li>
				<a href="{{base_path}}/install-and-setup/install/installing-the-product/installing-in-containers/installing-si-using-docker">Installing the Streaming Integrator on Docker</a>
			</li>
			<li>
				<a href="{{base_path}}/install-and-setup/install/installing-the-product/installing-in-containers/installing-si-using-kubernetes">Installing the Streaming Integrator on kubernetes</a>
			</li>           
		</td>
	</tr>
</table>

### Setting up

Setting up the Streaming Integrator component involves performing the following tasks.

 <table>
    <tr>
        <th>
            <a href="{{base_path}}/install-and-setup/setup/si-setup/updating-si">Applying WSO2 Updates</a>
        </th>
        <td>
            Explains how to get the latest updates that are available for a particular release of the Streaming Integrator.
        </td>
    </tr>
    <tr>
        <th>
            <a href="{{base_path}}/install-and-setup/setup/si-setup/production-checklist">Production Checklist</a>
        </th>
        <td>
            Lists all the setup tasks you need to complete in order to run the Streaming Integrator component in a production environment.
        </td>
    </tr>
    <tr>
        <th>
            <a href="{{base_path}}/install-and-setup/setup/si-setup/performance-analysis-results">Performance Analysis Results</a>
        </th>
        <td>
            This has the results of the performance tests carried out for the Streaming Integrator component.
        </td>
    </tr>
    <tr>
        <th>
            <a href="{{base_path}}/install-and-setup/setup/si-setup/configuring-business-rules-deployment">Configuring Business Rules Deployment</a>
        </th>
        <td>
            Explains how to configure a Streaming Integrator node to use a specified business rule template. Business rules templates are templates Streaming applications and queries that allow you to use the streaming logic ofWSO2 API Manager without writing queries from scratch.
        </td>
    </tr>
    <tr>
        <th>
            <a href="{{base_path}}/install-and-setup/setup/si-setup/configuring-data-sources">Configuring Data Sources</a>
        </th>
        <td>
            Explains how to configure the data sources vis which the Streaming Integrator server and the Streaming Integrator Tooling connect to databases. This section also explains the default data sources configured for the Streaming Integrator and the Streaming Integrator Tooling.   
        </td>
    </tr>
    <tr>
        <th>
            <a>Securing the Streaming Integrator</a>
        </th>
        <td>
            Explains how to secure the Streaming Integrator component and the data it handles. The topics covered are as follows.
            <li>
                <a href="{{base_path}}/install-and-setup/setup/si-setup/general-data-protection-regulations">General Data Protection Regulations</a>
            </li>
            <li>
                <a href="{{base_path}}/install-and-setup/setup/si-setup/working-with-keystores">Working with Keystores</a>
            </li>
            <li>
                <a href="{{base_path}}/install-and-setup/setup/si-setup/protecting-sensitive-data-via-the-secure-vault">Protecting Sensitive Data via the Secure Vault</a>
            </li>
        </td>
    </tr>
    <tr>
        <th>
            <a href="{{base_path}}/install-and-setup/setup/si-setup/supporting-different-transports">Supporting Different Transports</a>
        </th>
        <td>
            Explains the setup tasks you need to complete to allow the Streaming Integrator component to work with different transports.
        </td>
    </tr>
    <tr>
        <th>
            <a href="{{base_path}}/install-and-setup/setup/si-setup/configuring-database-and-file-system-state-persistence">Configuring State Persistence</a>
        </th>
        <td>
            Explains how to prevent the loss of data that can result from a system failure by persisting the state of Streaming Integrator component periodically either into a database system or into the file system.
        </td>
    </tr>
    <tr>
        <th>
            <a href="{{base_path}}/install-and-setup/setup/si-setup/configuring-cluster-coordination">Configuring Cluster Coordination</a>
        </th>
        <td>
            Explains how to configure a cluster coordination strategy that determines how the Streaming Integrator nodes in a cluster coordinate with each other.
        </td>
    </tr>
    <tr>
        <th>
            <a href="{{base_path}}/install-and-setup/setup/si-setup/adding-third-party-non-osgi-libraries">Adding Third Party Non OSGi Libraries</a>
        </th>
        <td>
            The Streaming Integrator component is OSGi-based. Therefore, when you are adding non-OSGi libraries to the Streaming Integrator pack, you need to first convert them into OSGi bundles. This section provides instructions to do this.
        </td>
    </tr>
    <tr>
        <th>
            <a href="{{base_path}}/install-and-setup/setup/si-setup/configuring-default-ports">Configuring Default Ports</a>
        </th>
        <td>
            Explains the default ports that the Streaming Integrator component uses for different purposes when the port offset is 0.
        </td>
    </tr>
    <tr>
        <th>
            <a href="{{base_path}}/install-and-setup/setup/si-setup/change-hostname-and-context-path">Changing the Host Name and Context Path of Web UI Applications</a>
        </th>
        <td>
            Explains how to change the host name and the context path specified in the URLS via which the user interfaces of the Streaming Integrator are accessed.
        </td>
    </tr>
    <tr>
        <th>
            <a href="{{base_path}}/install-and-setup/setup/si-setup/monitoring-received-events-count-via-logs">Enabling Logs for Received Event Count</a>
        </th>
        <td>
            Explains how to configure the Streaming Integrator component to log the total number of events it received via its sources per given time interval.
        </td>
    </tr>                               
 </table>

### Deploying

See the topics given below for instructions on setting up a Streaming Integrator deployment.

<table>
    <tr>
        <th>
            <a href="{{base_path}}/install-and-setup/setup/deployment-overview">Deployment Patterns</a>
        </th>
        <td>
            This explains all the deployment patterns you can follow when you deploy WSO2 API manager. These patterns involve deploying the API Manager component together with Micro Integrator and Streaming Integrator components in clustered setups.
        </td>
    </tr>
    <tr>
        <th>
            <a href="{{base_path}}/install-and-setup/setup/si-deployment/deploying-si-as-a-single-deployment">Single-Node Streaming Integrator Deployment</a>
        </th>
        <td>
            Instructions on setting up a single-node Streaming Integrator deployment.
        </td>
    </tr>
    <tr>
        <th>
            <a href="{{base_path}}/install-and-setup/setup/si-deployment/deploying-si-as-minimum-ha-cluster">Minimum HA Streaming Integrator Deployment</a>
        </th>
        <td>
            Instructions on setting up a Streaming Integrator deployment with minimum high availablity.
        </td>
    </tr>
    <tr>
        <th>
            <a href="{{base_path}}/install-and-setup/setup/si-deployment/deploying-si-as-an-active-active-deployment">Active-Active Streaming Integrator Deployment</a>
        </th>
        <td>
            Instructions on setting up an Active-Active Streaming Integrator deployment.
        </td>
    </tr>
    <tr>
        <th>
            <a href="{{base_path}}/install-and-setup/setup/si-deployment/deploying-si-as-a-scalable-cluster">Scalable Streaming Integrator Deployment</a>
        </th>
        <td>
            Instructions on setting up a scalable Streaming Integrator deployment.
        </td>
    </tr>
</table>

## Reference

<table>
    <tr>
        <th>
            <a href="{{base_path}}/install-and-setup/setup/reference/common-runtime-and-configuration-artifacts">Common Runtime and Configuration Artifacts</a>
        </th>
        <td>
            Describes some artifacts that are commonly used with the API Manager component.
        </td>
    </tr>
    <tr>
        <th>
            <a href="{{base_path}}/install-and-setup/setup/reference/default-product-ports">Default Product Ports</a>
        </th>
        <td>
            Explains the defauly ports used by the API Manager component.
        </td>
    </tr>
    <tr>
        <th>
            <a href="{{base_path}}/install-and-setup/setup/reference/product-compatibility">Product Compatibility</a>
        </th>
        <td>
            Provides details relating to the compatibility of the API Manager component with different operating systems and JDKs, databases, key managers, web browsers, and other WSO2 products.
        </td>
    </tr>
    <tr>
        <th>
            <a href="{{base_path}}/install-and-setup/setup/reference/supported-cipher-suites">Supported Cipher Suites</a>
        </th>
        <td>
            Provides details of the supported cipher suites.
        </td>
    </tr>
</table>