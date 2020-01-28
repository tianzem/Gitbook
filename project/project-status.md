# Project Status

The project status section shows the various states that a project can be in. These are set by the user throughout the course of wireframing a project. 

![](../.gitbook/assets/project-status.png)

{% hint style="info" %}
The "Created" status and "Processing" status can not be set by the user
{% endhint %}

* Created
  * A project has been created, but the files have not been uploaded to start processing the project.
  * Projects in this state will show up as white on the intranet queue. Users can't do anything with projects in this status
* Processing
  * The files are uploading, and the project is being generated.
  * During this status, the autogen-Wireframe branch will be created.
  * This status will also be triggered when [Plane Refine](../tools/wireframe-tools/wireframe/plane-refine.md) is running.
* In\_QA
  * The autogen-Wireframe branch is available, and the project is ready to be wireframed.
* In\_Review
  * This status is for users in training. Projects are set to in\_review when the trainee is finished and ready for a senior member to review their work before publishing the project.
* In\_Support
  * This is reserved for projects with specific issues that hinder the workflow. Refer to the link below to determine if a project falls under this status:
    * [https://pointivo.atlassian.net/wiki/spaces/CO/pages/170229773/In+Support+Projects](https://pointivo.atlassian.net/wiki/spaces/CO/pages/170229773/In+Support+Projects)
* Complete\_Initial
  * Ignore this status for now.
* Complete\_Final
  * In this status, a project is finished. 
  * Before setting a project to Complete\_Final, all resources must be generated and published, structure type verified, and project issues noted.
  * Once this status is selected, the files are immediately returned to the customer.
    * It is **extremely** important that everything is double checked before setting projects to complete\_final.

{% hint style="warning" %}
If a project is IN\_QA, but has no autogen-Wireframe branch to open, please post a message on the Custops-help channel on Slack. Check this link to see if the issue falls within these parameters:

How to restart a processing request [https://pointivo.atlassian.net/wiki/spaces/CO/pages/187596815/How+to+Restart+a+Processing+Request](https://pointivo.atlassian.net/wiki/spaces/CO/pages/187596815/How+to+Restart+a+Processing+Request)
{% endhint %}



