**Red Hat**

* **/rhn-to-rhsm/**
  * **supported-rhn-classic-to-rhsm/**
    * This playbook is designed to help migrate Red Hat servers from RHN to RHSM
    * Knowledgebase article referenced: [Migrating from RHN to RHSM in Red Hat Enterprise Linux ](https://access.redhat.com/solutions/129723)
    * **NOTE:**  
      * As of RHEL5.8 and RHEL6.2, Red Hat provides a script that will assist in the migration of systems registered to RHN Classic to Certificate-based RHN.
      * This playbook runs the RHN Migrate script.  This will autosubscribe/autoattach subscriptions. Your machine _may_ attach the wrong subscription.  Be mindful.
