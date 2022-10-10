# How to Contribute

We'd love to accept your patches and contributions to this project. There are
just a few small guidelines you need to follow.

## Contributor License Agreement

Contributions to this project must be accompanied by a signed
[Contributor Agreement](ContributorAgreement.txt).
You (or your employer) retain the copyright to your contribution,
this simply gives us permission to use and redistribute your contributions as
part of the project.

## Checklist before contributing

When adding your contribution using a Pull Request, you will be asked the following questions:

1. Confirm that you have the right to submit the code that is being contributed. Please consider the origin of your code and confirm you
   have the appropriate rights to make the submission subject to the Apache 2.0 license that applies to everything in this repository of
   custom steps. If so, follow the instructions for the [Contributor Agreement](ContributorAgreement.txt) (which is based on the
   industry-standard Developer Certificate of Origin (DCO))
2. Confirm that your contribution does not include any personally identifiable information (PII), for example, in any examples used 
   in your README file.
3. Confirm your contribution does not include any encryption or other export-controlled technology.  

## Guidelines for contributions

1. Make sure your custom step contribution is provided as a **.step** file and embeds all the macro definitions it relies on.
    * This to make it very easy to install in a user's environment: Simply download the **.step** file from this repository 
      and then upload it to a SAS Content folder to have it show up in the Steps panel in SAS Studio. 
      No further steps/configuration required.
    * Once you have added a custom step from this repository to your SAS Viya environment, see 
      [(FAQ) How to share macro definitions across multiple Custom Steps](./docs/FAQ.md#how-to-share-sas-macro-definitions-across-multiple-custom-steps)
      for more information on how you could separate the macro definitions into separate files and store them in **SAS autocall libraries**. 
2. Recommendations to use in the Program part (code generation) of a custom step can be found in 
  [SAS coding best practices](./docs/SASCodingBestPractices.md).
3. All submissions, including submissions by project members, require review. We use GitHub pull requests for this purpose.
   Consult [GitHub Help](https://help.github.com/articles/about-pull-requests/) for more information on using pull requests in general.
   The next section will go through the detailed steps from start to finish.  

## Steps to perform when contributing a Custom Step
 
High-level the procedure is as follows: Create a **Fork** of the public repository under your own GitHub account, create a dedicated folder in the
forked repository to contain your contribution including documentation, then issue a **Pull request** which makes your contribution available for review by the maintainers of the public repository, and answer the questions being asked. When accepted, the maintainer will merge into the public repository. 

There are multiple tools that can be used to do all of this. A list of tasks to perform using a combination of GitHub webUI and [GitHub Desktop](https://desktop.github.com/) is shown below: 

1. (GitHub webUI) [Login to GitHub](https://github.com/) using your own account (a personal GitHub account should work just fine)
2. (GitHub webUI) Issue a **Fork** request on the
   [public SAS Studio Custom Steps repository](https://github.com/sassoftware/sas-studio-custom-steps) 
3. (GitHub Desktop) **Clone** your **Fork** to a local repository (on your local harddisk)
4. In that local repository create a dedicated folder and copy the contents of the **Rank Columns - Starter template** folder into that folder,
   and replace the **.step** file with your **.step** file 
5. Update the **README.md** file in that dedicated folder to reflect your custom step and replace the screenshots in the **img** subdirectory
   with screenshots of the UI of your custom step 
6. (GitHub Desktop) Commit the changed files and push them back to your **Forked** repository (aka. origin remote repository)
7. (GitHub webUI) **Sync** your **Forked repository** to incorporate all changes from the upstream/parent repository.
8. (GitHub Desktop/GitHub webUI) From the **Forked repository**, issue a **Pull request** to make your contribution available for review 
   by the maintainers of the parent repository
8. (GitHub webUI) As part of the **Pull request** you will be shown a message in the GitHub webUI that asks you to answer the questions outlined in
   "Checklist before contributing" shown above, and also asks to attach a signed version of the [Contributor Agreement](ContributorAgreement.txt)

Ad step 8:
    * This can be done directly from the **GitHub webUI** or initiated from the **GitHub Desktop application**. The latter will
      open a browser tab showing the Pull request page in the GitHub webUI.
    * A **Pull request** results in the maintainers of the parent repository to be notified of a contribution/update.  
    * The **maintainers** will review the request, ask additional questions if needed, and then if everything is okay
      perform a **merge request**. This will make your contribution available in the public repository. 
    * You will automatically be notified by GitHub when the merge request has finished successfully.
