When you first enable version updates, you may have many dependencies that are outdated and some may be many versions behind the latest version. {% data variables.product.prodname_dependabot %} checks for outdated dependencies as soon as it's enabled. You may see new pull requests for version updates within minutes of adding the configuration file, depending on the number of manifest files for which you configure updates. {% data variables.product.prodname_dependabot %} will also run an update on subsequent changes to the configuration file.

{% data variables.product.prodname_dependabot %} may also create pull requests when you change a manifest file after an update has failed. This is because changes to a manifest, such as removing the dependency that caused the update to fail, may cause the newly triggered update to succeed.

To keep pull requests manageable and easy to review, {% data variables.product.prodname_dependabot %} raises a maximum of five pull requests to start bringing dependencies up to the latest version. If you merge some of these first pull requests before the next scheduled update, remaining pull requests will be opened on the next update, up to that maximum. You can change the maximum number of open pull requests by setting the [`open-pull-requests-limit` configuration option](/github/administering-a-repository/configuration-options-for-dependency-updates#open-pull-requests-limit).