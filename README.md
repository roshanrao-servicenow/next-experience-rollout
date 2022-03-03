# next-experience-rollout
Enable Next Experience is an application containing utilities that can be used for a controlled rollout of Next Experience. Individuals can request that the experience be enabled/disabled for them through the provided service catalog item. Administrators can use scripts to enable/disable the experiences for all users in one or more roles or groups.

What is included in the package:
- PrefMgmtUtil: Script include providing utility functions that support Flows/Scripts/Jobs to help set the Next Experience enablement preference for users either individually or as a collection based on role assignment/group membership.
- Request ServiceNow Next Experience: Service catalog item that allows users to request Next Experience to be enabled/disabled for them on the ServiceNow platform. The catalog listing can be updated to include demo/training video. Request processing is done using a Flow (Next Experience - Automated toggle) that triggers a confirmation notification, "Next Experience toggled for user".
- Enable NE for Agents and Admins: SAMPLE script for enabling next experience for Agents (itil) and Platform Admins (admin). This has been left with commented code that can be updated based on upgrade goals.

Dependencies:
There are no plugin dependencies and this should run on San Diego or higher.
Since this is a scoped application, it is required that update access ("Can update") be enabled on sys_user_preference table.

Licensing and Distribution:
This code is provided free of charge with no limitations on use or distribution. However, there are no liabilities attached to this; use at your own risk. This is NOT code provided by ServiceNow development team.
