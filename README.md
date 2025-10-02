Reference: [powerbi-visuals-gantt](https://github.com/microsoft/powerbi-visuals-gantt)


------
Clone repo and install the PowerBI Visual Tools (pbiviz) package:
```
npm i -g powerbi-visuals-tools
```

------
# powerbi-visuals-gantt
[![Build Status](https://github.com/microsoft/powerbi-visuals-gantt/actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/microsoft/powerbi-visuals-gantt/actions/workflows/build.yml)

> A Gantt chart is a type of bar chart which illustrates a project timeline or schedule. The Gantt Chart visual shows the Tasks, Start Dates, Durations, % Complete, and Resources for a project. The Gantt Chart visual can be used to show current schedule status using percent-complete shadings and a vertical "TODAY" line. The Legend may be used to group or filter tasks based upon data values.

![Gantt chart screenshot](assets/screenshot.png)

# Overview

Gantt chart is a type of bar chart to illustrate a schedule with time axis. When you put Gantt chart along with other insightful charts in an interactive canvas, you can manage your project in whole new way. In Power BI as visuals interact with each other, you can look at your resource allocation, task completion, remaining tasks in different perspective and get a firm handle on the future.
Gantt charts are indispensable part of project management portfolio. Project Managers and executives love Gantt charts, since they visually show in a very effective at-a-glance way, the overall time line of the project, the current status & progress (or lack thereof) along with the assignment at considerable details.
With this custom visual, you can specify the Tasks, Start Date, Duration and %Completion for rendering them as Gantt. Please note that the %Completion expects a decimal value ( for example 0.85 means 85%) and Start Date , a date field and not a date hierarchy.
You can also control the color of the bar with a Legend. You can use any relevant field from your project as Legend for example task type for this purpose. Additionally, you can also specify the resource field, which would be listed next the bar in the Gantt.

See also [Gantt chart at Microsoft Office store](https://store.office.com/en-us/app.aspx?assetid=WA104380765&sourcecorrid=968c5e90-8711-48fe-b9b4-a15ad9fe8dc4&searchapppos=0&ui=en-US&rs=en-US&ad=US&appredirect=false)


# Develop-Custom-Visual-Using-React
---------
Follow the setups from microsofts documentations:
*https://learn.microsoft.com/en-us/power-bi/developer/visuals/environment-setup?tabs=desktop*
---------
### Command to add certificate: open CMD and run below command:
```
pbiviz install-cert
```
<img width="597" height="244" alt="image" src="https://github.com/user-attachments/assets/e2aa22a3-0824-4543-ba93-0353b50f93b9" />




---------
Note: When you add Certicate and run to an error see the link/run the command below:
https://camkode.com/posts/fixing-pwsh-is-not-recognized-error-in-powershell-core

```
dotnet tool update --global PowerShell
```



---------
install the PowerBI Visual Tools (pbiviz) package.
```
npm i -g powerbi-visuals-tools
```

---------

Enable Developer mode - The working is only in Web Service - Not sure for Desktop PBI App:
https://app.powerbi.com/user/user-settings/developer-settings?experience=power-bi


---------
# Enhancing with D3.js

On app file, expand the node_modules folder to check the packages d3, @type/d3, core-js, and powerbi-visuals-api are installed. If you can’t find any of these, just run the npm install for all the missing packages:
```
npm install d3 @types/d3 core-js powerbi-visuals-api
```


We've got all we need now to start developing our first visual using D3.js.

---------
Now proceed and Create a development project by following the link below from MSFT:
https://learn.microsoft.com/en-us/power-bi/developer/visuals/create-react-visual


---------
When testing the visual and don't see any changes go to below link and authorize your browser:
```
https://localhost:8080/assets
```


