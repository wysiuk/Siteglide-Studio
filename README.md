# Siteglide Module Boilerplate
A simple and easy way to set up a module in Siteglide. This template, which you can use when creating your module in GitHub, will provide a great starting point for creating your module.

### Installation Procedure

First up, create a new repo for your module, with this repo as the "Repository Template".
Then, head to the [module creation](https://admin.siteglide.com/#/portal/community/marketplace/-1) page in Siteglide Admin.
Input the Name, Type, Version & Description fields and click save.
Upon reload, the Vanity ID field will be populated. This is your module ID, which you should use for your folder structure and in associated setup files.

Now you have your module ID, you should then head over to the [setup.json](setup.json) file in your new repo and replace the `id` field with your module id (e.g. `"id": 101,`), and the `module_name.value` field with your module name (e.g. `"value": "Awesome Module"`)

For now, you shouldn't need to use the [install-process.json](install-process.json) file if you're creating a module that just uses the Custom UI functionality and the [ignore-on-update.json](ignore-on-update.json) file until you provide updates for your module. You can find out more about these files [here](https://developers.siteglide.com/2-create-folder-structure).

Next up, you will need to rename your [module folder](/modules/module_id) to match your module id (e.g. `/modules/module_101`).

Finally, if this is a private repo, you'll need to invite SiteglideAPI (or api@siteglide.com) as a collaborator to the repo. This is in the repo settings, under "Collaborators & Teams". Once this is done and approved by Siteglide, you can then finalise your module in Siteglide Admin.

To finalise your module, head back to the edit module page.

Then you'll need to fill out the "GitHub Repo Account" field (e.g. `wysiuk`) and the "GitHub Repo Name" field (e.g. `Siteglide-Module-Boilerplate`).

If you're using the Custom UI functionality select "Show Menu Item" and input the "Custom UI Path" (e.g. `modules/module_101/index`) & "Menu Name".

If you wish the module to be visible to others outside of Wysi, click Public

Finally, save the module.

You may now install the module on a site.

To easily edit the module, you can add the site you have installed your module to via cli and sync your changes to the site, and sync the changes to the repo, remembering not to include the .siteglide-cli file.
