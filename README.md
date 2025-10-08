# Build a Custom Power BI Visual with React

The GitHub repository below served as a valuable reference for this build. Big thanks to everyone who contributed.

**Reference**: *[powerbi-visuals-gantt](https://github.com/microsoft/powerbi-visuals-gantt)*

---

## Getting Started

**Development Setup**

Follow Microsoft's official setup and prerequisites guide:
[Environment setup docs](https://learn.microsoft.com/en-us/power-bi/developer/visuals/environment-setup?tabs=desktop)

## Create a React Custom Visual

Follow the Microsoft guide: [Create a React Visual](https://learn.microsoft.com/en-us/power-bi/developer/visuals/create-react-visual)

---

## Developer Mode

Enable developer mode in Power BI Service:
[Power BI Developer Settings](https://app.powerbi.com/user/user-settings/developer-settings?experience=power-bi)

> Note: Developer mode works only in **Power BI Service** (not Desktop app).

---

### Add Developer Certificate

Run in **CMD**:

Open cmd (win + r then type cmd)
```bash
pbiviz install-cert
```

If you encounter an error sayong like "pbiviz is not recognized by the system as a command...." or similar to below:
<img width="1350" height="228" alt="image" src="https://github.com/user-attachments/assets/735c82c7-578e-4eb1-8154-43fce727c903" />

Use below approach:
- open command prompt: Start -> Run -> CMD
- change directory to npm folder to *C:\users<userid>\AppData\Roaming\npm*
- run the command ```pbiviz --install-cert```

You should be able to see this window:
<img width="801" height="783" alt="image" src="https://github.com/user-attachments/assets/e42c59e2-626e-4017-97f5-4fb135f14a4a" />

Go to this folder mentioed below and click **Next**
<img width="801" height="783" alt="image" src="https://github.com/user-attachments/assets/dcf85bc0-c53e-479b-bb29-ef8d65a35da0" />

And enter the password generated from above folder:
<img width="801" height="783" alt="image" src="https://github.com/user-attachments/assets/2b80c6e6-9816-4bc4-8fd3-4ba5c0b5514f" />






If you encounter the `pwsh is not recognized` error, run below command:

```bash
dotnet tool update --global PowerShell
```

Or you can visit this link to find more details: [Fixing pwsh issue](https://camkode.com/posts/fixing-pwsh-is-not-recognized-error-in-powershell-core)

---

## About the Gantt Visual

A **Gantt chart** is a bar chart that illustrates a project timeline.

This custom visual supports:

* Tasks, Start Dates, Durations, % Complete, Resources.
* Percent-complete shading
* Vertical "TODAY" line
* Legend-based grouping/filtering

## My Updates:
### Milestone Settings
* Added milestone icon flag (pennant)
* Option to display legend text next to the milestone icon
* Ability to apply milestone icon to all occurrences

### Tooltip Settings
* Option to change tooltip mode (All, Dates only, Off)


![Gantt chart screenshot](assets/screenshot.png)


---

### If you want to clone this repo:

Copy below command:
```
git clone https://github.com/domants/Custom-Visual-Using-React.git
```

## Install Dependencies
### cd to your root folder and run the below command to install required packages.

Global Installation (CLI Tool) - You need to run this outside your root folder to install it globally.
```
npm install -g powerbi-visuals-tools
```

Project Dependencies: To give you the building blocks to create, style, test, and optimize custom visuals for Power BI.
```
npm install d3 @types/d3 core-js powerbi-visuals-api powerbi-visuals-utils-interactivityutils powerbi-visuals-utils-testutils lodash @types/lodash powerbi-visuals-utils-formattingutils powerbi-visuals-utils-chartutils powerbi-visuals-utils-svgutils powerbi-visuals-utils-formattingmodel powerbi-visuals-utils-colorutils powerbi-visuals-utils-tooltiputils powerbi-visuals-utils-typeutils
```

Check under `node_modules`. -> d3 folder
If any are missing, rerun `npm install d3 @types/d3 core-js powerbi-visuals-api`.

---

## Debugging & Testing

If your changes don’t show up, authorize browser access:

```url
https://localhost:8080/assets
```

---

### Package your Power BI visual. Follow the link below:
*[Package PBI Visual](https://learn.microsoft.com/en-us/power-bi/developer/visuals/package-visual)*

---

### You can also see the link below for the single source of truth for all of the Power BI Custom Visuals

[PowerBI-Visuals-AppSource](https://github.com/DataChant/PowerBI-Visuals-AppSource/tree/main)

*The link above is a repository of Power BI custom visuals that are periodically exported from Microsoft AppSource to support the Power BI community*

---

## 📚 Summary

* **pbiviz** is the main tool for Power BI visuals.
* Use **D3.js + React** to build interactive visuals.
* Enable developer mode in **Power BI Service** for live testing.
* Troubleshoot with certificate setup and dependency checks.

---
