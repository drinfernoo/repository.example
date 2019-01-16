# repository.example
Example of how to set up a Kodi repository, hosted on GitHub pages.

In order to follow this tutorial, first fork this repository, and then clone your newly forked copy locally.

First, you'll need to edit the `addon.xml` file and folder name for your Kodi repo. Rename the folder `repository.example` to whatever add-on ID you'd like your repo to have.
From the Kodi wiki, "... It must be unique, and must use only lowercase characters, periods, underscores, dashes and numbers." Another good rule of thumb is to name your repository something like `repository.whatever`.
Inside the `addon.xml` file in your `repository.whatever` folder, edit line 2 with your chosen add-on ID, the version number (or leave at 1.0), and your username (or whatever you'd like) for `provider`.
You also need to replace `YOUR_USERNAME_HERE` and `REPOSITORY_NAME_HERE` with your GitHub username and this repository's name, respectively, as seen on lines 5-7 n `addon.xml`:

```
            <info compressed="false">https://raw.githubusercontent.com/YOUR_USERNAME_HERE/REPOSITORY_NAME_HERE/master/zips/addons.xml</info>
            <checksum>https://raw.githubusercontent.com/YOUR_USERNAME_HERE/REPOSITORY_NAME_HERE/master/zips/addons.xml.md5</checksum>
            <datadir zip="true">https://raw.githubusercontent.com/YOUR_USERNAME_HERE/REPOSITORY_NAME_HERE/master/zips/</datadir>
```

Place the add-on source folders for whichever add-ons you'd like to be contained in your Kodi repo in the main folder of this repository, and run `_repo_xml_generator.py`.

This will create zips of all of the desired add-ons, and place them in the `zips` folder, along with a generated `addon.xml` and `addons.xml.md5`. You'll need them for the next step.



