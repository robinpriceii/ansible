**Red Hat**

* **security-scan/**
    * The playbook will run a Red Hat vulnerability scan and generate an HTML report.
    * When the playbook finishes, you may be able to run `firefox /opt/report.html` on the local system to review results.
    
To manually run this from your terminal:
* `[~]$ sudo wget -c4 https://www.redhat.com/security/data/metrics/ds/com.redhat.rhsa-RHEL7.ds.xml && oscap xccdf eval --results results.xml --report report.html com.redhat.rhsa-RHEL7.ds.xml`

