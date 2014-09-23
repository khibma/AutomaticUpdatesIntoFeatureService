AutomaticUpdatesIntoFeatureService
==================================

This Python script turns grabs a point location from an external site which is constantly updating. It parses the feature and pushes submits an updated point to an ArcGIS.com feature service. A feature service with proper schema must already exist for this script to work correctly.

See more information on the [associated ArcGIS Blog post](http://blogs.esri.com/esri/arcgis/...).

## Instructions

1. Download the update.py and settings.ini files. (Hint: Click the `Download ZIP` button on the right)
2. Save these files to your local working directory
3. Setup a feature service with your ArcGIS.com account. The instructions [on this blog post](http://blogs.esri.com/esri/arcgis/2014/09/22/how-to-create-a-hosted-feature-service/) explain the different ways. The required feature service for this example is simple, as such the first option of creating a service from ArcGIS Online would be straight forward. 
3a. From **My Content**, click **Create Layer**.
--1. Select from a URL to a feature layer
--2. Enter:  http://services1.arcgis.com/hLJbHVT9ZrDIzK0I/arcgis/rest/services/issSchema/FeatureServer/0
--3. Select next, accept the default extent and enter some useful tags and summary information on the final page. Remember the title, you'll need to enter this information into the Python script.
--4. Click done.
--5. Set sharing options for the service. You **do not** need to enable editing.
4. Edit the Python script you saved previously and update the variables at the top of the script. 
5. Run the script. As-is, it'll update the point every 5 minutes. Modify this value to your needs.

## Resources

* [ArcGIS REST API Update Features](http://resources.arcgis.com/en/help/arcgis-rest-api/index.html#/Update_Features/02r3000000zt000000)


## Licensing
Copyright 2014 Esri

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

A copy of the license is available in the repository's [license.txt]( https://github.com/update-hosted-feature-service/master/license.txt) file.

[](Esri Tags: ArcGIS.com Online Update Hosted Feature Services Automate Python Publish)
[](Esri Language: Python)​
