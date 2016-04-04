# ops-custom-eap6

##Overview
This Git repository demonstrates how to customize an image within OSEv3.  This simple example create a license file named 'ops-license.txt' in the JBOSS_HOME directory.  
This repository is used as part of the [Ops Workflow for Customizing Builder Images Demo](https://github.com/rhtconsulting/rhc-ose/tree/openshift-enterprise-3/demos/operations-workflow-for-customizing-builder-images)

## Bill of Materials

### Environment Specifications

This code should be run on an installation of OpenShift Enterprise V3

### Template Files

None

### Config Files

None

### External Source Code Repositories

N/A


## Setup and Usage Instructions

The example below takes the base EAP6 OpenShift image and runs the assemble script in this GitHub repo.  The resulting image will have a new license file named `ops-license.txt`

Example usage:  
```bash
oc new-app registry.access.redhat.com/jboss-eap-6/eap-openshift~http://github.com/rhtconsulting/ops-custom-eap6.git --name=ops-custom-eap6 --namespace=ops-custom-eap6-proj
```
