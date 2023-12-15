<!-- @page page_building-samples_index Generating solutions for the FidelityFX SDK -->

<h1>Building FidelityFX SDK Samples</h1>

<h2>Generating solutions for the FidelityFX SDK</h2>

To build the samples in the AMD FidelityFX SDK you should follow these instructions:

1) Install the following software developer tool minimum versions:

- [CMake 3.17](https://cmake.org/download/)
- [Visual Studio 2019](https://visualstudio.microsoft.com/downloads/)
- [Windows 10 SDK 10.0.18362.0](https://developer.microsoft.com/en-us/windows/downloads/windows-10-sdk)
- [Vulkan SDK 1.3.239](https://vulkan.lunarg.com/)

2) Generate Visual Studio FSR sample solutions:

**Native-backend linked version**

  ```bash
  > <installation path>\BuildFSRSolutionNative.bat
  ```

**Native-backend DLL version**

  ```bash
  > <installation path>\BuildFSRSolutionNativeDll.bat
  ```
  
  This will generate a `build\` directory where you will find the solution for either the native-backend-backed SDK samples (`FidelityFX SDK Native.sln`).
  
<h2>Building & running in Visual Studio</h2>

<h3>Building the project</h3>

By default, the Visual Studio solution file (.sln) that is generated by CMake will contain projects for all sample applications included in the SDK. To build the projects in the solution, you should click on ``Build`` and then ``Build solution`` from the menu at the top of Visual Studio. This will build all dependencies of the samples (such as the Cauldron framework), before then building the full collection of sample applications.

<h3>Running the project</h3>

To run a project from Visual Studio you should follow the following instrutions:

1) Select the project of interest in the solution explorer under the "Effects" folder.

2) Right-click the project and select 'Set as Start-up project'.

3) Click on the `Build` menu item from the toolstrip, and then click on `Run`.