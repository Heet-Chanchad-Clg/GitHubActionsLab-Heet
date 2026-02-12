GitHubActionsLab-Heet

1) The purpose of each workflow:

Dependent Jobs:
This workflow was made to demonstrate the execution in a sequential manner. It is to make sure that the project is started by building it, then testing it then only if these two are successful, deploy it.

Multi-Platform Jobs:
This workflow shows parallel execution in different environments at the same time. So basically, it tests the code on the different operating systems – Ubuntu, Windows and macOS. This ensures the cross-platform compatibility.

2) Key Concepts being demonstrated:

Needs: This is utilized in the dependent workflow in order to create a hierarchy. In this demonstration, test job needs build will stop running tests if the build fails.

Runs-on: This tell whick platform to run on, in this case, it is ubuntu-latest, windows-latest and macos-latest.

3) Challenges and solution:

When I tried pushing the files on GitHub, I was facing challenges like when I tried pushing the files, they were uploaded but I could not see the workflows being run.

Then I looked closely and found out that my file hierarchy was not correct and then I fixed it by placing the yml files in the .github/workflows file.
