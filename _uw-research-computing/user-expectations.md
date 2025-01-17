---
layout: guide
title: Policies and Expectations for Using CHTC
alt_title: Policies and Expectations for Using CHTC
guide:
    order: 1
    category: Basics and Policies
---


This page lists important policies and expectations for using CHTC computing and 
data services. Our goal is to support a community of users and a variety of 
research. If an individual user is taking 
action that negatively impacts our services, we reserve the right to 
deactivate their account or remove files without notice. 

## Access and Use

Use of CHTC services are free to use in support of UW - Madison’s research and 
teaching mission.

**Accounts are linked to individuals and should NOT be shared.** We are happy to make new
accounts for individuals or group-owned spaces for sharing files. Accounts that we 
notice being shared will be immediately disabled and a meeting with the PI 
(faculty advisor) may be necessary to reinstate the account.

For more information on access to CHTC after graduation, see [below](#access-chtc-resources-after-graduation).

## Data Policies

**CHTC data locations are not backed up**, and users should
treat CHTC compute systems as temporary storage locations for *active*,
currently-queued computational work. Users should remove data from CHTC
systems upon completion of a batch of computational work and keep copies of
all essential files in a non-CHTC location. CHTC staff reserve the right
to delete data from any CHTC data location at at any time, to preserve
systems performance, and are not responsible for data loss or file system
corruption, which are possible in the absence of back-ups.

**CHTC is not HIPAA-compliant** and users should not bring HIPAA data into 
CHTC services. If you have data security concerns or any questions about 
data security in CHTC, [please get in touch](https://chtc.cs.wisc.edu/uw-research-computing/get-help.html)! 

To request a change in the quotas for a storage location, please see
our [Request a Quota Change](quota-request) guide.

### Export Control

Users agree not to access, utilize, store, or in any way run export controlled data, information, 
programs, etc. on CHTC software, equipment, or computing resources without prior review by the 
UW-Madison Export Control Office.

Export controlled information is subject to federal government rules on handling and viewing and has 
restrictions on who and where it may be accessed. A license can be required for access by foreign 
persons and in foreign jurisdictions so it’s important to ensure that all legal requirements are 
followed.
If you have export controlled information that you would like to use on the CHTC, or you are unsure 
if the information you have is export controlled, please contact the Export Control Office at 
[exportcontrol@grad.wisc.edu](mailto:exportcontrol@grad.wisc.edu) for guidance.

**Note: The CHTC is not compliant with Controlled Unclassified Information (CUI) requirements.**

## User Expectations

Because our systems are shared by many CHTC users, everyone contributes to 
helping the systems run smoothly. The following are some best practices 
to get the most out of CHTC without harming other users. Our goal 
is always to help you get your work done - if you think the following recommendations 
limit your capacity to run work, please contact us to discuss alternatives. 

**Never run computationally intensive tasks on the login nodes** for either 
system. As a rule of thumb, anything that runs for more than a few seconds, or 
is known to use a lot of cores or memory should not be run directly, but as a job. 
Small scripts and commands (to compress data, create directories,
etc.) that run within a few minutes on the submit server are okay,
but their use should be minimized when possible. If you have questions about this, 
please contact the facilitation team. CHTC staff reserve the right to kill any long-running or problematic processes on the 
head nodes and/or disable user accounts that violate this policy

**Avoid unsupervised scripts on the login nodes.** Automating tasks via tools like 
`cron`, `watch`, or using a workflow manager (not including HTCondor's DAGMan) on the login node is not allowed without prior 
discussion with the facilitation or infrastructure team. 

> **(HTC system specific):** Since use of `watch` with `condor_q` is prohibited, 
we recommend using `condor_watch_q` as an alternative for live updates on your jobs 
in the queue. `condor_watch_q` is more efficient and will not impair system performance. 

**Test your jobs**. We recommend testing a small version of your overall workflow 
before submitting your full workflow. By testing a smaller version of your jobs, 
you can determine resource requests, runtimes, and whether you may need an increase 
in your user quota. Both our HTC and HPC systems use a fair shair policy and each 
researcher has a user priority. **Submitting many jobs that fail or do not produce 
the unexpected output will decrease your user priority without helping you complete 
your research.**  User priorities naturally reset over time. 

## Access CHTC Resources after Graduation

We understand that some users may need to continue carrying out their computational 
analyses after graduation and the subsequent expiration of their NetID. 

To maintain access to CHTC resources after you leave your position at the University, 
your faculty advisor can sponsor continued access to CHTC resources and your NetID. 
Your Faculty Sponsor should email CHTC (chtc@cs.wisc.edu) and provide:

1. Your name,
1. The reason you need continued access to CHTC resources,
1. The amount of time they would like to sponsor your account,
1. Your new city/country of residence, and 
1. Your new institution. 

CHTC staff will then go through the needed steps to extend your account. 

* We highly recommend reaching out to CHTC staff before your NetID expires, if possible. 
* Your faculty sponsor can sponsor your account for up to one year at a time. If 
you need continued access past one year, your faculty sponsor must contact us and 
re-confirm that you should have continued access. 
* As a reminder, CHTC accounts are deactivated and user data is erased after a user 
is no longer actively using their account (~1 year of inactivity). It is your responsibility
to maintain your data and important files in a location that is not CHTC's file systems. 
