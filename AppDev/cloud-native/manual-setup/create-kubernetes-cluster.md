![](../../../common/images/customer.logo2.png)

# Creating your own Kubernetes cluster

**ATTENTION !!!** 

If you are doing the lab self guided, or the instructor does not tell you they have created a cluster for you then you need to complete this section.

If you are in an instructor led lab they **may** have already created Kubernetes clusters for you, **only** in the situation where you have been given a kubeconfig file and you do not need to continue with this section.



## Introduction

**Estimated module duration** 5 mins.

### Objectives

Creating a Managed Kubernetes cluster on the Oracle Cloud.  

### Prerequisites

If you are doing the full labs (these include modules on Helidon and Docker) you need to have completed the steps in the `Helidon` modules (including the setup)

If you are only doing the Kubernetes based labs you need to have completed the steps in the `Tenancy Setup for the Kubernetes Labs` module.

## Step 1: Creating your Kubernetes cluster

### Navigate to the Managed Kubernetes dashboard

- Log into the **Cloud Console** using the URL provided, and using the username and password you created earlier.
- Once on the **OCI infrastructure** page, click on the hamburger menu to navigate to 
  - **Developer services**, then **Container Clusters (OKE)**

- In the **List Scope** section, use the dropdown to select the **CTDOKE** compartment
  - You may have to expand the tree nodes to locate this compartment
- Click the **Create Cluster** button at the top of the clusters list

- Choose the option for the **Quick Create**, then click the **Launch workflow** button



### Creating the cluster

- Fill in the form with following parameters:

  - In the next form name the cluster something like Helidon-Lab-YOUR-INITIALS
  - Make sure the compartment is **CTDOKE**
  - Make sure the Kubernetes version is the highest on the list (at the time of the last update of this document in October 2020 that was 1.17.9, but it may have been updated since then)
  - Leave the visibility type as **private**
  - Set the shape to VM.Standard2.1
  - Set the number of nodes to be 2

There is no need to do anything in the `Advanced Options` section.

These images are for creating a 1.16.8 cluster, they may be slightly different for later versions.
 
![](images/create-k8s-cluster.png)

- Click the Next button to go to the review page.

- On the review page check the details you have provided are correct
- Click the Create Cluster button.

You'll be presented with a progress option, if you want read what's happening

- Scroll to the bottom and click the **Close** button

The state will be "Creating" for **a few minutes** (usually 3-4 mins)

