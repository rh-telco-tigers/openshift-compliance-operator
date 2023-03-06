This post will be based on the documentation available at https://docs.openshift.com/container-platform/4.7/security/compliance_operator/compliance-operator-understanding.html.

Many enterprises are required by law and/or corporate policies to follow the Center for Internet Security (CIS) framework and other best-practices for the secure configuration of target systems. The Openshift Compliance Operator is based on the OpenScap project which should be familiar to anyone who is in charge of IT security. For more information about OpenScap, please visit https://www.open-scap.org/. By installing this operator, you will be able to scan your Openshift cluster and the underlying operating system (CoreOS) which is read-only (hardened) version of RHEL (Red Hat Enterprise Linux) for any compliance violations and in most-cases, the violation can be mitigated by applying a MachineConfig configuration to the operating system.

In this post and accompanying videos, I will:

Show how the Compliance Operator is installed via the OCP web console.
Explain the various custom-resource-defininions/APIs that are available after installing the Compliance Operator.
Explain the profiles that are available out-of-the-box.
Describe Compliance Rules
Describe Compliance Operator Scans
How to Retrieve Operator Scan Results
How to Handle Remediations
The Compliance Operator lets OpenShift Container Platform administrators describe the desired compliance state of a cluster and provides them with an overview of gaps and ways to remediate them. The Compliance Operator assesses compliance of both the Kubernetes API resources of OpenShift Container Platform, as well as the nodes running the cluster. The Compliance Operator uses OpenSCAP, a NIST-certified tool, to scan and enforce security policies provided by the content.

https://www.myopenshiftblog.com/openshift-compliance-operator/
