https://zenodo.org/records/581789

# Description
[ManyBugs/](./ManyBugs/) contains the ManyBugs programs and defects and the baseline results of running GenProg 2.0, TRPAutoRepair, and AE on them. The results and benchmark scenarios are in different directories:

- [results/](./ManyBugs/results/) is further subdivided into AE, TRPAutoRepair, and GenProg 2.0 results. The results consist of packages that contain the output debug files of the associated run; each debug file contains the command-line arguments that resulted in the run. These packages also contain repaired files, if applicable.
- [scenarios/](./ManyBugs/scenarios/) contains 185 tarballs of the defect scenarios, one per defect per program. The naming scheme indicates the subject program and the revision pair corresponding to the defect in question. Each tarball contains a test.sh file that has all "positive" and "negative" tests individually executable.
- [bug-data.csv](./ManyBugs/bug-data.csv) contains categorization information about the defects in the set.
- The [AutomatedRepairApplicabilityData](https://github.com/LASER-UMASS/AutomatedRepairApplicabilityData) repository contains data on characteristics of the ManyBugs defect scenarios, such as defect priority, size of developer-written patch, time it took developer(s) to fix the defect, etc., as well as scripts for deriving these data