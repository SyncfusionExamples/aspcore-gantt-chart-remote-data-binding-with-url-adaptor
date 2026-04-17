# ASP.NET Core Gantt Chart Remote Data Binding Sample
A sample ASP.NET Core app demonstrating Syncfusion EJ2 Gantt remote binding with `UrlAdaptor` and batch CRUD operations.

## Overview

A Gantt chart in `DataManager/Views/Home/Index.cshtml` loads remote task data from `Home/UrlDatasource` and sends batch updates to `Home/BatchUpdate`.

## Features

- Remote read binding with `UrlAdaptor`
- Batch add/edit/delete operations
- In-memory sample task data
- Resource mapping and dependency support
- CORS enabled for development

## Prerequisites

- .NET 7 SDK
- Syncfusion EJ2 ASP.NET Core package
- HTTPS certificate for `https://localhost`

## Run

1. Open `DataManager.sln` or use the command line.
2. Restore:
   ```bash
   dotnet restore
   ```
3. Run:
   ```bash
   dotnet run --project DataManager/DataManager.csproj
   ```
4. Open the reported URL.

## Endpoints

- `POST /Home/UrlDatasource` returns Gantt data, including counts.
- `POST /Home/BatchUpdate` applies added, edited, and deleted records.

## Notes

- Data is stored in-memory and resets on restart.
- Change hardcoded `https://localhost:44379` URLs if the port differs.
- Syncfusion license may be required for production use.

