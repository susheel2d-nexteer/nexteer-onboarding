# Nexteer Onboarding Plan - SAP Build Work Zone

## Deploy via SAP Business Application Studio (BAS)
1. Open BAS > Create Full Stack Cloud Application dev space
2. File > Import Project from File System > select this ZIP
3. Open Terminal in project root
4. Run: `mbt build`
5. Run: `cf login -a <API_ENDPOINT>`
6. Run: `cf deploy mta_archives/com.nexteer.onboarding_1.0.0.mtar`

## Deploy via Command Line
1. Prerequisites: `npm install -g mbt` and `cf install-plugin multiapps`
2. Extract ZIP, cd into folder
3. `mbt build`
4. `cf deploy mta_archives/com.nexteer.onboarding_1.0.0.mtar`

## After Deployment - Add to Work Zone Site
1. SAP Build Work Zone > Channel Manager > Update HTML5 Apps content provider
2. Content Manager > Content Explorer > HTML5 Apps > find "Nexteer Onboarding Plan" > Add to My Content
3. Content Manager > My Content > create a Group > add the app
4. Assign a Role (e.g., Everyone) > include the app
5. Open your Site - the tile appears!

## Roles
| Role Collection | Permission |
|----------------|------------|
| Nexteer Onboarding Manager | Manager checkboxes only |
| Nexteer Onboarding Employee | Employee checkboxes only |
| Nexteer Onboarding Buddy | Buddy checkboxes only |
