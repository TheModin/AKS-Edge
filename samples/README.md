# AKS Edge Essentials Samples

## Akri samples

| Name           | Description      |
|----------------|------------------|
| [akri-opcua](./akri-opcua/) | Sample to deploy Akri OPC UA discovery handler. For more information, see [Akri OPC UA](https://docs.akri.sh/discovery-handlers/opc-ua). |
| [opcua-server](./opcua-server/) | Sample to deploy a Windows OPC UA server simulator. |
| [akri-onvif](./akri-onvif/) | Sample to deploy ONVIF discovery handler and video streaming application. For more information, see [Akri ONVIF for IP Cameras](https://docs.akri.sh/discovery-handlers/onvif).|

## WebAssembly (WASM) samples

| Name           | Description      |
|----------------|------------------|
| [wasm-spin](./wasm/wasm-spin.md) | Sample to deploy WASM Spin payload. For more information, see [Spin](https://github.com/fermyon/spin/). |
| [wasm-slight](./wasm/wasm-slight.md) | Sample to deploy WASM Slight payload. For more information, see [Spiderlightning](https://github.com/deislabs/spiderlightning/). | 


## Arc enabled data services

| Name           | Description      |
|----------------|------------------|
| [sqledge](./sqledge/) | Sample to deploy SQL Edge container using PVC storage. 

## Interop Samples

_:warning: **WARNING**: Enabling a communication channel between the Windows host and the AKS lite VM may increase security risks._

| Name           | Description      |
|----------------|------------------|
| [interop-textmsg-consoleapp](./interop-textmsg-consoleapp) | Basic interop sample demonstrating text messaging between a Windows console app and an workload running inside the AKS lite cluster. | 
<!-- | [interop-customvision-textmsg-uwpapp](./interop-customvision-textmsg-uwpapp) | <p>Two more advanced interop samples which demonstrate bidirectional communication between a Windows application and an Edge module running inside the AKS lite VM. </p><ul><li>Text messaging between a UWP application and an Edge module. </li><li>A 'Custom vision' machine learning interop sample with a fruit classifier which uses a Windows UWP app to send camera frames to an Edge module for identification.</li></ul>| -->

The interop samples demonstrate usage patterns for interoperatibility between Microsoft's Windows host OS and workloads running on the AKS lite cluster.  These code samples were created with templates available in Visual Studio and are designed, but not limited to, run on devices using AKS lite. For more information, review [AKS lite docs](/docs/AKS-Lite-Concepts.md).

> **Note:** If you are unfamiliar with Git and GitHub, you can download the entire collection as a 
> [ZIP file](https://github.com/Microsoft/Windows-universal-samples/archive/master.zip), but be 
> sure to unzip everything to access shared dependencies. For more info on working with the ZIP file, 
> the samples collection, and GitHub, see [Get the UWP samples from GitHub](https://aka.ms/ovu2uq). 
> For more samples, see the [Samples portal](https://aka.ms/winsamples) on the Windows Dev Center. 

### Windows development environment

These samples require Visual Studio and the Windows Software Development Kit (SDK) for Windows 10/11.

   [Get a free copy of Visual Studio Community Edition with support for building Universal Windows Platform apps](http://go.microsoft.com/fwlink/p/?LinkID=280676)

Additionally, to stay on top of the latest updates to Windows and the development tools, become a Windows Insider by joining the Windows Insider Program. [Become a Windows Insider](https://insider.windows.com/)

### Using the samples

The easiest way to use these samples without using Git is to download the zip file containing the current version (using the following link or by clicking the "Download ZIP" button on the repo page). You can then unzip the entire archive and use the samples in Visual Studio.

   **Notes:**

   * Before you unzip the archive, right-click it, select **Properties**, and then select **Unblock**.
   * Be sure to unzip the entire archive, and not just individual samples. The samples all depend on the SharedContent folder in the archive.   
   * In Visual Studio, the platform target defaults to ARM, so be sure to change that to x64 or x86 if you want to test on a non-ARM device. 

The samples use Linked files in Visual Studio to reduce duplication of common files, including sample template files and image assets. These common files are stored in the SharedContent folder at the root of the repository and are referred to in the project files using links.

**Reminder:** If you unzip individual samples, they will not build due to references to other portions of the ZIP file that were not unzipped. You must unzip the entire archive if you intend to build the samples.

For more info about the programming models, platforms, languages, and APIs demonstrated in these samples, please refer to the guidance, tutorials, and reference topics provided in the Windows 10 documentation available in the [Windows Developer Center](http://go.microsoft.com/fwlink/p/?LinkID=532421). These samples are provided as-is in order to indicate or demonstrate the functionality of the programming models and feature APIs for Windows and AKS lite.

## Contributing

This project welcomes contributions and suggestions. For more information, visit [Contributing](/CONTRIBUTING.md).