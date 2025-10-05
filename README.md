# Build a Custom Power BI Visual with React

Below is the GitHub repository I'm using as a reference for this repo. Thanks to those guys who participated on this build.

**Reference**: *[powerbi-visuals-gantt](https://github.com/microsoft/powerbi-visuals-gantt)*

Copy below if you want to clone the Repo

```bash
git clone https://github.com/microsoft/powerbi-visuals-gantt.git
cd powerbi-visuals-gantt
```

### You can also see the link below for the single source of truth for all of the Power BI Custom Visuals

[PowerBI-Visuals-AppSource](https://github.com/DataChant/PowerBI-Visuals-AppSource/tree/main)

*The link above is a repository of Power BI custom visuals that are periodically exported from Microsoft AppSource to support the Power BI community*

---

## 🚀 Getting Started

**Development Setup**

Follow Microsoft's official setup and prerequisites guide:
👉 [Environment setup docs](https://learn.microsoft.com/en-us/power-bi/developer/visuals/environment-setup?tabs=desktop)

---

## 📊 About the Gantt Visual

[![Build Status](https://github.com/microsoft/powerbi-visuals-gantt/actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/microsoft/powerbi-visuals-gantt/actions/workflows/build.yml)

A **Gantt chart** is a bar chart that illustrates a project timeline or schedule.

This custom visual supports:

* Tasks, Start Dates, Durations, % Complete, Resources, Milestone Icon with legend next to it
* Percent-complete shading
* Vertical "TODAY" line
* Legend-based grouping/filtering

![Gantt chart screenshot](assets/screenshot.png)

See also: [Microsoft AppSource Gantt Chart](https://store.office.com/en-us/app.aspx?assetid=WA104380765)

---

### Add Developer Certificate

Run in **CMD**:

```bash
pbiviz install-cert
```
<img width="597" height="244" alt="image" src="https://github.com/user-attachments/assets/b0c93803-834e-46e2-8e50-2ed881124059" />



If you encounter the `pwsh is not recognized` error:

```bash
dotnet tool update --global PowerShell
```

More details: [Fixing pwsh issue](https://camkode.com/posts/fixing-pwsh-is-not-recognized-error-in-powershell-core)

---

## ⚙️ Developer Mode

Enable developer mode in Power BI Service:
[Power BI Developer Settings](https://app.powerbi.com/user/user-settings/developer-settings?experience=power-bi)

> ⚠️ Note: Developer mode works only in **Power BI Service** (not Desktop app).

---

### If you want to clone this repo:

Copy below command:
```
git clone https://github.com/domants/Custom-Visual-Using-React.git
```

## 📦 Install Dependencies
### cd to your root folder and run the below command to install required packages.

Global Installation (CLI Tool)
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

## 📈 Create a React Custom Visual

Follow the Microsoft guide:
👉 [Create a React Visual](https://learn.microsoft.com/en-us/power-bi/developer/visuals/create-react-visual)

---

## 🔍 Debugging & Testing

If your changes don’t show up, authorize browser access:

```url
https://localhost:8080/assets
```

---

### Package your Power BI visual. Follow the link below:
*[Package PBI Visual](https://learn.microsoft.com/en-us/power-bi/developer/visuals/package-visual)*


---

## 📚 Summary

* **pbiviz** is the main tool for Power BI visuals.
* Use **D3.js + React** to build interactive visuals.
* Enable developer mode in **Power BI Service** for live testing.
* Troubleshoot with certificate setup and dependency checks.

---
