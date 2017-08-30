**Red Hat**

* **/rhn-to-rhsm/**
  * **supported-rhn-classic-to-rhsm/**
    * This playbook is designed to help migrate Red Hat servers from RHN to RHSM
    * Knowledgebase article referenced: [Migrating from RHN to RHSM in Red Hat Enterprise Linux ](https://access.redhat.com/solutions/129723)
    * **NOTE:**  
      * As of RHEL5.8 and RHEL6.2, Red Hat provides a script that will assist in the migration of systems registered to RHN Classic to Certificate-based RHN.
      * This playbook runs the RHN Migrate script.  This will autosubscribe/autoattach subscriptions. Your machine _may_ attach the wrong subscription.  Be mindful.

  * **unsupported-rhn-classic-to-rhsm/**
    * This playbook is designed to help migrate Red Hat servers from RHN to RHSM
    * Knowledgebase article referenced: [Migrating from RHN to RHSM in Red Hat Enterprise Linux ](https://access.redhat.com/solutions/129723)
    * **NOTE:**  
      * This playbook is designed around the unsupported manual steps listed in the knowledgebase article.
      * This playbook is for versions of RHEL where the migration script isn't "supported".
      * This will run the --auto-attach feature from Subscription Manager.
      * This may add additional repositories to the machine.
      * Example:  
        * EUS repos/CloudForms tools repo/RHN tools repo
        * None of these will compromise the health of the machine.
        
* **security-scan/**
    * The playbook will run a Red Hat vulnerability scan and generate an HTML report.
    * When the playbook finishes, you may be able to run 'firefox /opt/report.html' on the local system to review results.

