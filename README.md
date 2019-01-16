# repository.example
Example of how to set up a Kodi repository, hosted on GitHub pages.

In order to follow this tutorial, first fork this repository, and then clone your newly forked copy locally.

Place the add-on source folders for whichever add-ons you'd like to be contained in your Kodi repo in the main folder of this repository, and run `_repo_xml_generator.py`.

This will create zips of all of the desired add-ons, and place them in the `zips` folder, along with a generated `addon.xml` and `addons.xml.md5`. You'll need them for the next step.

Next, you'll need to edit the `addon.xml` file and folder name for your Kodi repo. Rename the folder `repository.example` to whatever add-on ID you'd like your repo to have. From the Kodi wiki, "... It must be unique, and must use only lowercase characters, periods, underscores, dashes and numbers." Another good rule of thumb is to name your repository something like `repository.whatever`.

