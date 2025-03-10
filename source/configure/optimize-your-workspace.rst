Optimize your Mattermost workspace
==================================

|all-plans| |cloud| |self-hosted|

.. |all-plans| image:: ../images/all-plans-badge.png
  :scale: 30
  :target: https://mattermost.com/pricing
  :alt: Available in Mattermost Free and Starter subscription plans.

.. |cloud| image:: ../images/cloud-badge.png
  :scale: 30
  :target: https://mattermost.com/sign-up
  :alt: Available for Mattermost Cloud deployments.

.. |self-hosted| image:: ../images/self-hosted-badge.png
  :scale: 30
  :target: https://mattermost.com/deploy
  :alt: Available for Mattermost Self-Hosted deployments.

With workspace optimizations, System Admins can review their workspace health and growth scores, then take advantage of recommended actions for ensuring their workspace is running smoothly and teams are maximizing productivity. 

System Admins can access their workspace optimization page in the System Console by going to **Reporting > Workspace Optimization**.

.. image:: ../images/workspace-optimization.png
  :alt: Review your workspace health and growth scores, then take advantage of recommended optimizations.

How is the overall score calculated?
------------------------------------

The highest score possible is 100. Your score is calculated based on the type of issue reported and the level of potential security risk introduced to your Mattermost deployment if ignored. 

Each item on the dashboard is calculated based on its individual impact score. These differ depending on whether they're problems, warnings, or suggestions. For example, if SSL encryption isn't configured in your workspace, Mattermost reports that as a problem, which reduces your score until it's addressed. 

Warnings impact your score less than problems, and suggestions have the least impact on your score.

Want to improve your overall workspace optimization score? Take action towards the problems, warnings, and suggestions reported on this dashboard. We recommend the following workspace optimizations.

Recommendations
---------------

The following optimization areas can alert you to workspace suggestions, warnings, or problems that may require your attention:

+-----------------------+----------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Optimization category | Suggestions, Warnings, or Problems Detected                                                              | Additional Information                                                                                                                                               |
+=======================+==========================================================================================================+======================================================================================================================================================================+
| Mattermost release    | Are you on the latest Mattermost release?                                                                | You're notified when updates are available.                                                                                                                          |
|                       |                                                                                                          | See the `Upgrade Mattermost <https://docs.mattermost.com/upgrade/upgrading-mattermost-server.html>`__ product documentation for details on upgrading your workspace. |
+-----------------------+----------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Configuration issues  | - **SSL**: Should your workspace be more secure with SSL?                                                | See the product documentation to learn more:                                                                                                                         |
|                       |                                                                                                          |                                                                                                                                                                      |
|                       | - **Session Length**: The default value may not provide an optimal user experience.                      | - `Set up SSL <https://docs.mattermost.com/onboard/ssl-client-certificate.html>`__                                                                                   |
|                       |                                                                                                          | - `Configure session length <https://docs.mattermost.com/configure/configuration-settings.html#session-lengths>`__                                                   |
+-----------------------+----------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Workspace access      | Is the Mattermost workspace may not be accessible to users?                                              | If your web server settings don't pass a live URL test, your workspace may not be accessible to others.                                                              |
|                       |                                                                                                          | See the `Environment Configuration Settings <https://docs.mattermost.com/configure/configuration-settings.html#environment>`__ product documentation to learn more:  |
+-----------------------+----------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Search performance    | As your user base grows, is search getting slower?                                                       | See the `Elasticsearch <https://docs.mattermost.com/scale/elasticsearch.html>`__ product documentation to learn more.                                                |
+-----------------------+----------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Data privacy          | Do you need more control and insights into your data?                                                    | See the product documentation to learn more:                                                                                                                         |
|                       |                                                                                                          |                                                                                                                                                                      |
|                       |                                                                                                          | - `Data Retention <https://docs.mattermost.com/comply/data-retention-policy.html>`__                                                                                 |
|                       |                                                                                                          | - `Compliance Export <https://docs.mattermost.com/comply/compliance-export.html>`__                                                                                  |
+-----------------------+----------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| User authentication   | - **AD/LDAP**: As your user base grows, would you benefit from easier onboarding,                        | See the product documentation to learn more:                                                                                                                         |
|                       |   automated deactivations, and role assignments?                                                         |                                                                                                                                                                      |
|                       |                                                                                                          | - `AD/LDAP <https://docs.mattermost.com/configure/configuration-settings.html#ad-ldap>`__                                                                            |
|                       | - **Guest accounts**: Do you want to control user access to channels and teams with guest accounts?      | - `Guest accounts <https://docs.mattermost.com/onboard/guest-accounts.html>`__                                                                                       |
+-----------------------+----------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------+
