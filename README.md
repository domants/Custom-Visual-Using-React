# Build a Custom Power BI Visual with React

Below is the GitHub repository I'm using as a reference for this repo. Thanks to those guys who participated on this build.

**Reference**: *[powerbi-visuals-gantt](https://github.com/microsoft/powerbi-visuals-gantt)*

Copy below if you want to clone the Repo

```bash
git clone https://github.com/microsoft/powerbi-visuals-gantt.git
cd powerbi-visuals-gantt
```

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

### Install Power BI Visual Tools (pbiviz)

```bash
npm i -g powerbi-visuals-tools
```

## 📦 Install Dependencies (D3.js)

Make sure required packages are installed:

```bash
npm install d3 @types/d3 core-js powerbi-visuals-api
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

## 📚 Summary

* **pbiviz** is the main tool for Power BI visuals.
* Use **D3.js + React** to build interactive visuals.
* Enable developer mode in **Power BI Service** for live testing.
* Troubleshoot with certificate setup and dependency checks.

---
