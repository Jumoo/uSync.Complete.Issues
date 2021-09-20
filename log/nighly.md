# nightly log. 

As we approach relase of v9 - we are rapidly itterating to squash the last few bugs, get performance right and get everything working. 
We are building new builds all the time and pushing then to our nightly feed: 

https://pkgs.dev.azure.com/jumoo/Public/_packaging/nightly/nuget/v3/index.json

this doc is a log of changes (as best we can remember) as we do this. 

## 17/09/2021
- Publisher 
  -  Moved the Licence file to /umbraco/licenses
  - don't default to the 'blank' site page on the dashboard anymore.
  - **FIX**: fixed sending of the zip file on a pull request (so pull was broken)

> BUILD `Install-Package uSync.Complete -version 9.0.0-beta005.20210917.5`

## 18/09/2021
- Publisher
  - Logging around the dependecny checking to see if we can identify any bottle necks.
  - removal of IncludeChildren on first pass of dependency checking (should reduce checks)

> BUILD: `Install-Package uSync.Complete -version 9.0.0-beta005.20210918.8`
