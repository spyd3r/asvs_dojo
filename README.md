# OWASP ASVS Issue Tracker

Create a github personal access token, then set an environment variable named GITHUB_PERSONAL_ACCESS_TOKEN with the value of your access token

The value of <verification_level> will dictate which issues will be associated to their corresponding ASVS milestones. For instance, a level 3 issue will not be assigned to a milestone if <verification_level> is set to 2. All issues regardless of their level will still be created.

```
./asvs.rb
Missing or invalid arguments: asvs.rb <project_name> <verification_level> <path_to_clone_repo>
Example: asvs.rb asvs-graphql 2 /home/bobdobs/projects/
```
**WHAT**
asvs_dojo is a utility to leverage Defect Dojo as the mediator between industry-recognized security tools and how they provide coverage to ASVS security requirements.

**WHY**
The why around this project aims to fulfill two objectives:
  * Demonstrate ASVS security coverage of engagements instantiated in Defect Dojo.
  * Identify coverage gaps in tests executed for respective engagements to continuously achieve the first objective.

**HOW**
* Create a new test in Defect Dojo called, "Level 1 Requirements."
* Read through the most recent copy of asvs.db and populate the, "Level 1 Requirements" test with the respective ASVS requirements to achieve level 1 adherence.
* Iterate through all of the tests completed for a respective Defect Dojo enagement, capture the CWE IDs, and the respective test name.
* Using the CWE IDs and respective test names in a Defect Dojo engagement, map the CWE IDs to every respective ASVS requirement and tag the ASVS requirement with the name of the test completed.
* Determine whether the tests within the Defect Dojo enagement provide coverage to satisfy ASVS requirements.

**Create an issue for each ASVS requirement**

![Screenshot](docs/images/asvs-issues.png)

**Filter issues by label**

![Screenshot](docs/images/asvs-label-search.png)

**Group ASVS requirements into milestones to easily track progress**

![Screenshot](docs/images/asvs-milestones.png)

**Create project boards to visualize work**

![Screenshot](docs/images/asvs-project-board.png)
