# Persist Prerendered State in Blazor Web Apps

A practical demonstration of persisting prerendered state in Blazor Web Apps using interactive server-side rendering. This sample shows how to eliminate UI flicker and reduce redundant API calls during component hydration by preserving prerendered data through the `PersistentComponentState` API.

## Overview

When a Blazor Web App renders components on the server during prerendering and then transitions to interactive mode on the client, there can be a noticeable flicker as components re-render and re-fetch data. This sample demonstrates two approaches:

- **With persistent state**: Data is serialized during prerendering and restored on the client, eliminating flicker
- **Without persistent state**: Data is fetched after interactivity starts, potentially causing UI flicker

The sample uses Grid components to display order data from the API, making the difference between both approaches immediately visible.

## Features

- **Side-by-side comparison** of state persistence strategies
- **Smooth component hydration** with prerendered state
- **Real-world data fetching** using HTTP client and async operations
- **Interactive Grid** with proper data binding
- **Responsive design** with Bootstrap styling

## Prerequisites

- [.NET SDK 8.0](https://dotnet.microsoft.com/download/dotnet/8.0) or later
- [Visual Studio 2022](https://visualstudio.microsoft.com/vs/) or later
- [Visual Studio Code](https://code.visualstudio.com/)

## Getting Started

### Clone the repository

```bash
git clone https://github.com/SyncfusionExamples/blazor-persist-prerendered-state-sample.git
cd blazor-persist-prerendered-state-sample
```

### Run with Visual Studio

1. Open the solution file using Visual Studio 2022 or later.
2. Restore the NuGet packages by rebuilding the solution.
3. Build the project to ensure there are no compilation errors.
4. Run the project.

### Run with .NET CLI

```bash
# Restore dependencies
dotnet restore

# Run the project
dotnet run
```
## References

- [Blazor DataGrid Documentation](https://blazor.syncfusion.com/documentation/datagrid/getting-started-with-web-app)
- [Blazor Components](https://blazor.syncfusion.com/documentation/introduction)

