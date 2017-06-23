# ansible

* **ansible/rhn-to-rhsm/**
  * ansible rhn-migrate-classic-to-rhsm playbook
  * This playbook is designed to help migrate Red Hat servers from RHN to RHSM
  * **Issues:**  This runs the RHN Migrate script.  This will autosubscribe/autoattach subscriptions. Your machine _may_ attach the wrong subscription.  Be mindful.
