**==> picture [596 x 420] intentionally omitted <==**

User Guide | PUBLIC Document Version: 1.5 – 2024-11-15 

**How to Package and Deploy SAP Business One Extensions for Lightweight Deployment** 

**==> picture [58 x 29] intentionally omitted <==**

**THE BEST RUN** 

## **Content** 

|**1**|**Document History. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 3**|
|---|---|
|**2**|**Introduction. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 4**|
|2.1|Overview. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .4|
|**3**|**Packaging Your Extensions for Lightweight Deployment. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 5**|
|3.1|Packaging Extension Data Files. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 5|
|3.2|Editing Existing Add-On Registration Data Files. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 6|
|3.3|Specifying Basic Information. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .7|
|3.4|Specifying Compatibility Information. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 7|
|3.5|Specifying Parameters Information. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 8|
|3.6|Packaging Your Extensions in SAP Business One Studio for Microsoft Visual Studio. . . . . . . . . . . . . . 9|
|3.7|Packaging Your Extensions in Command Line Mode. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 10|
|**4**|**Deploying Your Extensions for Lightweight Deployment in SAP Business One. . . . . . . . . . . . . 13**|
|4.1|Accessing SAP Business One Extension Manager. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .13|
|4.2|Importing an Extension. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 14|
|4.3|Removing an Extension. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 14|
|4.4|SAP Business One Extension Manager - Extensions Tab. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 14|
|4.5|Assigning an Extension to a Company. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .15|
|4.6|Unassigning an Extension from a Company. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 17|
|4.7|SAP Business One Extension Manager - Company Assignment Tab. . . . . . . . . . . . . . . . . . . . . . . . . 18|
|4.8|SAP Business One Extension Manager - Security Settings Tab. . . . . . . . . . . . . . . . . . . . . . . . . . . . .18|
|4.9|Running the Extension in SAP Business One. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 19|
|**5**|**Deploying Your Extensions for Lightweight Deployment in SAP Business One Cloud. . . . . . . . 21**|
|**6**|**Upgrading Your Extensions for Lightweight Deployment in SAP Business One. . . . . . . . . . . . . 22**|
|**7**|**Upgrading Your Extensions for Lightweight Deployment in SAP Business One Cloud. . . . . . . . 24**|



How to Package and Deploy SAP Business One Extensions for Lightweight Deployment 

**Content** 

**2** PUBLIC 

## **1 Document History** 

|Version|Date|Change|
|---|---|---|
|1.0|2014-05-09|First version.|
|1.1|2015-06-29|SAP Business One Cloud uses the Extension Package tool|
|1.2|2018-01-09|Supports Command Line mode.|
|1.3|2020-11-03|Add Extension Manager - Security Settings tab|
|1.4|2023-07-14|Update compatible version format for SAP Business One|
|||10.0|
|1.5|2024-11-15|Guide converted from PDF to HTML format for viewing on|
|||the SAP Help Portal.|



How to Package and Deploy SAP Business One Extensions for Lightweight Deployment **Document History** 

PUBLIC 

**3** 

## **2 Introduction** 

This document describes how to manage the lifecycle of your extensions for lightweight deployment. 

Extensions that are enabled for lightweight deployment do not have dedicated installers. Instead, the required files are located within a ZIP archive, and installation is performed by the application. 

The lifecycle management of the extensions for lightweight deployment is managed end to end by SAP Business One. You do not need to use InstallShield (or equivalent) third party tools. 

With this feature, you have the following key benefits: 

- Automated life cycle management of extensions without user interaction 

- Zero operational down time required for extension deployment 

- No administrator privileges required for end users to install the extension 

## **2.1 Overview** 

The following are the basic steps to managing the lifecycle of your extensions for lightweight deployment: 

1. Use the Extension Package tool to package the lightweight binaries into a zip file and generate an addon registration data ( `.ard` ) file containing data about extensions enabled for lightweight deployment in Extensible Markup Language (XML) format. 

For more information, see Packaging Your Extensions for Lightweight Deployment [page 5]. 

##  Caution 

The Extension Package tool is not designed to replace the original Ard Generator tool. This tool is designed for extensions using lightweight deployment only. For extensions that do not use lightweight deployment, use the original tool. 

2. Use the SAP Business One Extension Manager to upload the package into SAP Business One and assign companies that run this extension. 

   - For more information, see Deploying Your Extensions for Lightweight Deployment in SAP Business One [page 13]. 

How to Package and Deploy SAP Business One Extensions for Lightweight Deployment **Introduction** 

**4** PUBLIC 

## **3 Packaging Your Extensions for Lightweight Deployment** 

The Extension Package tool enables you to package your extensions for lightweight deployment. 

The Extension Package tool is a component in SAP Business One Software Development Kit. To install the Extension Package tool, you should install SAP Business One Software Development Kit, and select _Tools ExtensionPackage_ . 

Using the Extension Package tool, you are able to do the following: 

- Package your extension for lightweight deployment 

- Create an add-on registration data (ARD) file 

- Import and edit an existing ARD file 

## **3.1 Packaging Extension Data Files** 

To package the extension files to a zip file and create a new file containing add-on registration data, do the following: 

1. In `…\SAP\SAP Business One SDK\Tools\ExtensionPackage` , run the `ExtensionPackage.exe file.` 

2. In the _Extension Registration Data Generator_ window, expand _Basic Information_ . Specify the extension name, version, and basic properties of the extension, and the name and contact information of the SAP partner that creates the extension. 

For more information, see Specifying Basic Information [page 7]. 

3. Expand _Extension File_ , specify the path of the executable file of your 32-bit or 64-bit add-on, and select the files that should be packaged in the zip file. 

   - To package your app for the version for SAP HANA, specify the app zip file, the name and the package of your app. 

##  Note 

The naming convention for your package is *.*. For example, if the package hierarchy is sap.sbo.atp in SAP HANA, the package name is this, and the corresponding URL will be https:// host:port/sap/sbo/atp . 

4. Expand _Deployment Steps_ , and select the COM dlls to register for your 32-bit or 64-bit add-on. 

5. Expand _SBO Compatibility_ , you can specify the versions of SAP Business One with which the add-on is compatible. 

For more information, see Specifying Compatibility Information [page 7]. 

6. Expand _Parameters_ ; you can optionally specify shared parameters and parameters for the extension. For more information, see Specifying Parameters Information [page 8]. 

How to Package and Deploy SAP Business One Extensions for Lightweight Deployment **Packaging Your Extensions for Lightweight Deployment** 

PUBLIC 

**5** 

7. Choose the _Package_ button. 

8. In the _Save As_ window, specify the location where you want to save the file and choose the Save button. 

##  Note 

If you just want to create a new file containing add-on registration data, choose the _Export_ button, and save the ARD file. 

## **3.2 Editing Existing Add-On Registration Data Files** 

## **Context** 

To edit an existing file containing add-on registration data, do the following: 

## **Procedure** 

1. In `…\SAP\SAP Business One SDK\Tools\ ExtensionPackage` , run the `ExtensionPackage.exe file` . 

2. In the _Extension Registration Data Generator_ window, choose the _Import_ button. 

3. In the _Open_ window, locate the file that you want to edit and choose the _Open_ button. 

4. In the _Extension Registration Data Generator_ window, expand _Basic Information_ . Specify the extension name, version, and basic properties of the extension, and the name and contact information of the SAP partner that creates the extension. 

For more information, see Specifying Basic Information [page 7]. 

5. Expand _SBO Compatibility_ ; you can specify the versions of SAP Business One with which the add-on is compatible. 

For more information, see Specifying Compatibility Information [page 7]. 

6. Expand _Parameters_ ; you can optionally specify shared parameters and parameters for the extension. 

For more information, see Specifying Parameters Information [page 8]. 

7. Choose the _Export_ button. 

8. In the _Save As_ window, specify the location where you want to save the file and choose the _Save_ button. 

How to Package and Deploy SAP Business One Extensions for Lightweight Deployment **Packaging Your Extensions for Lightweight Deployment** 

**6** 

PUBLIC 

## **3.3 Specifying Basic Information** 

To specify basic information, do the following: 

1. In `…\SAP\SAP Business One SDK\Tools\ExtensionPackage` , run the `ExtensionPackage.exe file` . 

2. In the _Extension Registration Data Generator_ window, expand _Basic Information_ , and specify the following fields: 

   - • _Extension Name_ – Enter the name of the extension. This field is mandatory. 

      - _Extension Version_ – Enter the version of the extension for which you want to package and generate the ARD file. This field is mandatory. 

      - _Extension Provider_ – Enter the name of the SAP partner that creates and owns the extension, for example, the name of your company. 

      - _Extension Namespace_ – Enter a name for the folder in which SAP Business One places the extension after a user registers the extension in the application. 

      - _Supported Database_ – Specify the database in which the extension works. This field is mandatory. 

      - _Contact Data._ – Enter contact information for the SAP partner that creates and owns the extension. For example, enter the URL of your company's Website. 

      - _Supported Client Type_ - Select the SAP Business One client type for your add-on to run. 

      - _Desktop_ - Add-ons/extensions work in the on-premise SAP Business One client only. 

      - _Browser_ - Add-ons/extensions work in the browser environment only. 

      - _Multiversion_ - Specify whether to support multiple different versions of the same add-on. That is, the application treats add-on 1.0 and add-on 2.0 as two different add-ons, while not treats add-on 2.0 as an upgrade version of add-on 1.0. 

This function does not support apps for the version for SAP HANA 

3. After specifying the basic information, do either of the following: 

   - If you are editing an existing ARD file, choose the _Export_ button to complete the editing process. 

   - If you are packaging your extension or creating a new ARD file, before exporting the file, you can optionally specify the compatibility information and the parameters information. For more information, see Specifying Compatibility Information [page 7] and Specifying Parameters Information [page 8]. 

## **3.4 Specifying Compatibility Information** 

The files that you generate using the Extension Package tool can contain data about the versions of SAP Business One with which the extension is compatible. This data is optional. 

To specify compatibility information, do the following: 

1. In `…\SAP\SAP Business One SDK\Tools\ExtensionPackage` , run the `ExtensionPackage.exe file` . 

2. In the _Extension Registration Data Generator_ window, select the _SBO Compatibility_ tab. 

3. In the _Compatible with SAP Business One_ area, specify the following: 

How to Package and Deploy SAP Business One Extensions for Lightweight Deployment **Packaging Your Extensions for Lightweight Deployment** 

PUBLIC 

**7** 

- _Version From_ – Enter the earliest version of SAP Business One with which the extension is compatible. 

- _To_ – Enter the latest version of SAP Business One with which the extension is compatible. 

##  Example 

Enter compatible versions of SAP Business One with the format, for example, 1000.100.00. You can refer the extension compatibility version with SAP Business One matrix in SAP Note 3321864 . 

##  Caution 

You must select a later version of SAP Business One from the _To_ dropdown list than the value you select from the _From_ dropdown list; otherwise, the application encounters an error during export. 

4. After specifying the compatibility information, do either of the following: 

   - If you are editing an existing ARD file, choose the _Export_ button to complete the editing process. 

   - If you are packaging your extension by creating a new ARD file, before you can export the file, you must specify the basic information and you can optionally specify the parameters information. 

For more information, see Specifying Basic Information [page 7] and Specifying Parameters Information [page 8]. 

## **3.5 Specifying Parameters Information** 

The files that you generate using the Extension Package tool can contain parameters information, which includes shared parameters and parameters properties for the extension. This data is optional. 

- Shared Parameters - The parameters or configuration required to run the extension. The parameters are shared in all extension instances running on different companies. 

- Parameters - The parameters or configurations required to run the extension. 

To specify parameters information, do the following: 

1. In `…\SAP\SAP Business One SDK\Tools\ExtensionPackage` , run the `ExtensionPackage.exe file` . 

2. In the _Extension Registration Data Generator_ window, expand the _Parameters_ tab. 

3. From the navigation menu, select _Shared Parameters_ . 

   - In the _Properties_ area of the _Shared Parameters_ window, click the add icon, and then specify the following: 

   - _Name_ – Enter the name of a property, which appears on the application user-interface. 

   - _Value_ – Enter a value for the property, which you can use to customize the extension deployment process. 

   - _Description_ – Optionally, enter a description for the property. 

To add valid values for the property, click the add icon, and then specify the following in the _Valid Values_ area: 

   - _Display Value_ – Enter a name for the valid value, which appears on the application user-interface. 

   - _Value_ – Enter a value for the valid value, which you can use during the deployment process. 

4. To specify additional shared parameters, in the _Properties_ area, click the add icon and specify the information from the previous step. 

How to Package and Deploy SAP Business One Extensions for Lightweight Deployment **Packaging Your Extensions for Lightweight Deployment** 

**8** PUBLIC 

5. From the navigation menu, select _Parameters_ . 

In the _Properties_ area of the _Parameters_ window, click the add icon, and then specify the following: 

- _Name_ – Enter the name of a property, which appears on the application user-interface. 

- _Value_ – Enter a value for the property, which you can use to customize the extension assignment process. 

- _Description_ – Enter an optional description for the property. 

To add valid values for the property, click the add icon, and then specify the following in the _Valid Values_ area: 

   - _Display Value_ – Enter a name for the valid value, which appears on the application user-interface. 

   - _Value_ – Enter a value for the valid value, which you can use during the assignment process. 

6. To specify additional parameters, in the _Properties_ area, click the add icon and specify the information from the previous step. 

7. After specifying the parameters information, do either of the following: 

   - If you are editing an existing ARD file, choose the Export button to complete the editing process. 

   - If you are packaging your extension by creating a new ARD file, before you can export the file, you must specify the basic information and you can optionally specify the compatibility information. 

For more information, see Specifying Basic Information [page 7] and Specifying Compatibility Information [page 7]. 

##  Note 

You can use the following UI API code to get and set the shared parameters and parameters: 

```
string value =
```

```
Application.SBO_Application.Company.GetExtensionProperty(Program.connectionSt
ring, SAPbouiCOM.BoExtensionLCMStageType.lcm_deployment, "SP1");
```

```
Application.SBO_Application.MessageBox(value);
```

```
Application.SBO_Application.Company.SetExtensionProperty(Program.connectionSt
ring, SAPbouiCOM.BoExtensionLCMStageType.lcm_deployment, "SP1", "Test1");
```

```
string value =
```

```
Application.SBO_Application.Company.GetExtensionProperty(Program.connectionSt
ring, SAPbouiCOM.BoExtensionLCMStageType.lcm_assignment, "P1");
```

```
Application.SBO_Application.MessageBox(value);
```

```
Application.SBO_Application.Company.SetExtensionProperty(Program.connectionSt
ring, SAPbouiCOM.BoExtensionLCMStageType.lcm_assignment, "P1", "TestP1");
```

## **3.6 Packaging Your Extensions in SAP Business One Studio for Microsoft Visual Studio** 

The SAP Business One Extension Package features are integrated in SAP Business One Studio for Microsoft Visual Studio. If you develop your extension using SAP Business OneSAP Business One Studio for Microsoft Visual Studio, you can package your project directly from the menu bar. 

How to Package and Deploy SAP Business One Extensions for Lightweight Deployment **Packaging Your Extensions for Lightweight Deployment** 

PUBLIC 

**9** 

To package your project, do the following: 

1. Build your project first to get the executable file of your extension. 

2. From the menu bar of the Microsoft Visual Studio main window, choose _SAP Business One Studio Extension Package_ . 

**==> picture [6 x 11] intentionally omitted <==**

3. In the _Extension Registration Data Generator_ window, specify the required information. For more information, see Packaging Extension Data Files [page 5]. 

4. Choose the _Package_ button and save the file. 

##  Note 

If you are not yet ready to package your extension, you can choose the _Save_ button. The information you entered in the _Extension Registration Data Generator_ window will be saved in your project. The next time you open the _Extension Registration Data Generator_ window, the saved information will be displayed. 

For more information about the SAP Business One Studio, see _Working with SAP Business One Studio Suite_ . 

## **3.7 Packaging Your Extensions in Command Line Mode** 

As of SAP Business One 9.3 PL02, the Extension Package tool supports Command Line mode. 

You can open the _Command Prompt_ window, go to the folder where the `ExtensionPackage.exe` file is located, and enter the command `ExtensionPackage.exe [options]` to execute the ExtensionPackage tool. For example, to package the Elster add-on, execute the following command under the folder where the `ExtensionPackage.exe` file is located: 

```
ExtensionPackage.exe /64:C:\Addons\ELSTERLW\X64\BEElster.exe /
```

```
86:C:\Addons\ELSTERLW\X86\BEElster.exe /s:C:\Addons\ELSTERLW\ELSTERLW.xml /
p:C:\Addons\ELSTERLW.zip /ex:.ard /v:930.110.01
```

If you enter the command `ExtensionPackage.exe /help` , you can see the options. 

_Packagepath_ , _SourceARDFile_ and at least one client _AddonExePath_ must be provided. 

- /help 

Display this help 

- /86:32bit-AddonExePath /64:64bit-AddonExePath 

   - /86:32bit-AddonExePath 

   - /64:64bit-AddonExePath 

- /p:FullPathToOutputDirectory/ExtensionName.zip 

Full path to save the output package. 

Application will override existing package file. 

- /s:SourceARDFile 

Source ARD file contains basic information and installation steps. 

- /v:Version 

Override version information. 

How to Package and Deploy SAP Business One Extensions for Lightweight Deployment **Packaging Your Extensions for Lightweight Deployment** 

**10** PUBLIC 

- /ex:".suffix1|.suffix2" 

Exclude files with specified suffixes under the packaging directory. 

##  Example 

```
/64:C:\Addons\ELSTERLW\X64\BEElster.exe
 /86:C:\Addons\ELSTERLW\X86\BEElster.exe
/s:C:\Addons\ELSTERLW\ELSTERLW.xml
/p:C:\Addons\ELSTERLW.zip
/ex:".chm|.pdb"
/v:930.110.01
```

##  Note 

An installation file list is not mandatory in _SourceARDFile_ . Packaging rules depend on whether the <Files> tag is empty. 

- For empty <Files>: 

The application will automatically package files in _ExeDir_ and sub-folders. 

All COM DLLs with matching platform will be marked to register. 

Option _/ex:_ files with listed suffixes won't be included in the package. 

• If there are files listed in <Files>: The application will package all the files listed. 

For more information about the SourceARDFile template, please see the following sample. 

```
<?xml version="1.0" encoding="utf-8"?>
    <AddOnRegData xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://
www.w3.org/2001/
   XMLSchema-instance" SlientInstallation="No" SlientUpgrade="No"
Partnernmsp="6" SchemaVersion=
   "3.0" Type="LightAddOn" MultipleVersion="false" OnDemand="True"
OnPremise="False" ExtName=
   "ELSTERLW" ExtVersion="930.110.01" Contdata="http://service.sap.com"
Partner="SAP" DBType="HANA"
   ClientType="A">
   <Validity>
     <SBOCompatibility>
     <Version From="930.110.01" To="930.110.01" />
     </SBOCompatibility>
   </Validity>
   <Configuration>
     <Repository />
     <Deployment>
       <Properties />
     </Deployment>
     <Assignment>
       <Properties />
     </Assignment>
   </Configuration>
   <Addons>
     <Addon Name="ELSTERLW" Group="" ForceFlag="False" Visible="False"
AutoAssign="False" SelfUpgrd=
     "False">
      <x86 AddonExe="BEElster.exe" AddonSig="D18D064AE7D7C76E98B30F80865F6FB5"
ExeDir="X86Client">
         <Installation>
           <Files>
```

How to Package and Deploy SAP Business One Extensions for Lightweight Deployment **Packaging Your Extensions for Lightweight Deployment** 

PUBLIC **11** 

```
             <File FileName="X86Client\BFLogger.dll">
                 <Actions>
                 <Register32bit />
               </Actions>
             </File>
             <File FileName="X86Client\BEElster.exe">
               <Actions />
             </File>
           </Files>
         </Installation>
         <Uninstallation>
           <Files>
             <File FileName="X86Client\BFLogger.dll">
                <Actions>
                <Unregister32bit />
               </Actions>
             </File>
             <File FileName="X86Client\BEElster.exe">
               <Actions />
             </File>
           </Files>
         </Uninstallation>
       </x86>
       <x64 AddonExe="BEElster.exe" AddonSig="BC8C639A3790BBABC9FC04255150FA16"
ExeDir="X64Client">
         <Installation>
           <Files>
             <File FileName="X64Client\BEElster.exe">
               <Actions />
             </File>
             <File FileName="X64Client\BFLogger.dll">
               <Actions />
             </File>
           </Files>
         </Installation>
         <Uninstallation>
           <Files>
             <File FileName="X64Client\BEElster.exe">
               <Actions />
             </File>
             <File FileName="X64Client\BFLogger.dll">
               <Actions />
             </File>
           </Files>
         </Uninstallation>
       </x64>
     </Addon>
   </Addons>
   <XApps>
     <XApp Name="" Path="" FileName="" />
   </XApps>
   <UDQs>
     <UDQ udqname="">
       <Hana FileName="" />
     </UDQ>
   </UDQs>
 </AddOnRegData>
```

How to Package and Deploy SAP Business One Extensions for Lightweight Deployment **Packaging Your Extensions for Lightweight Deployment** 

PUBLIC 

**12** 

## **4 Deploying Your Extensions for Lightweight Deployment in SAP Business One** 

The SAP Business One Extension Manager enables you to deploy your extensions for lightweight deployment. 

The SAP Business One Extension Manager is a component in Server Tools for SAP Business One. To install SAP Business One Extension Manager, you should install SAP Business One, and select _Server Tools Landscape Management Extension Management_ . 

To deploy an extension, perform the following steps: 

1. Import the extension to SAP Business One Extension Manager. 

2. Assign the extension to companies in SAP Business One Extension Manager. 

3. Run the extension in SAP Business One. 

## **4.1 Accessing SAP Business One Extension Manager** 

##  Caution 

Access to SAP Business One Extension Manager is under SAP Business One user authorization. Only a site user can open it. For more information about site users, see SAP Business One online help. 

To access SAP Business One Extension Manager, do the following: 

1. In the SAP Business One client, from the Main Menu, choose _Administration Add-Ons Add-On_ 

_Administration_ . The _Add-On Administration_ window appears. 

2. In the A _dd-On Administration_ window, click the _Manage Extensions for Lightweight Deployment_ hyperlink. A Web browser opens and displays the logon page of System Landscape Directory (SLD). 

3. To log on, enter the site user name and password and choose the _Log On_ button. The _SAP Business One Extension Manager_ window appears. 

##  Note 

Alternatively, you can access SAP Business One Extension Manager directly from a Web browser on the machine on which the System Landscape Directory (SLD) service is running using the following URL: **`https://<hostname>:<port>/ExtensionManager`** . 

How to Package and Deploy SAP Business One Extensions for Lightweight Deployment **Deploying Your Extensions for Lightweight Deployment in SAP Business One** 

PUBLIC **13** 

## **4.2 Importing an Extension** 

To import your extension to SAP Business One, perform the following steps: 

1. In the _SAP Business One Extension Manager_ window, on the _Extensions_ tab, choose the _Import_ button. The _Extension Import Wizard_ window appears. 

2. Choose the _Browse_ button to locate the zip file of your extension (created in Packaging Extension Data Files [page 5]), and choose _Upload_ . 

The basic information of the extension appears. 

3. Choose _Next_ to optionally specify the value of the shared parameters. The shared parameters are the parameters or configuration required to run the extension. The parameters are shared in all extension instances running on different companies. 

   - The _Shared Parameters_ table displays all shared parameters that are defined in the _Extension Package_ tool when you package your extension. 

For more information, see Specifying Parameters Information [page 8]. 

4. Choose _Next_ . 

5. On the _Finish_ tab, we recommend that you continue to assign this extension to a company. After you click the _Finish import and run the company assignment wizard_ hyperlink, the _Company Assignment Wizard_ window appears. 

For more information, see Assigning an Extension to a Company [page 15]. 

## **4.3 Removing an Extension** 

To remove the imported extensions, perform the following steps: 

1. In the _SAP Business One Extension Manager_ window, choose the _Extensions_ tab. 

2. From the table, select the extension you want to remove. 

3. Choose the _Remove_ button. 

##  Caution 

If an extension is assigned to companies, after the removal, the assigned extension will no longer be available. 

## **4.4 SAP Business One Extension Manager - Extensions Tab** 

The _Extensions_ tab displays a list of available extensions with basic information of the extensions. You can import new extensions or remove existing extensions. 

How to Package and Deploy SAP Business One Extensions for Lightweight Deployment **Deploying Your Extensions for Lightweight Deployment in SAP Business One** 

**14** PUBLIC 

## **SAP Business One Extension Manager, Extensions Tab Fields** 

|Field|Activity/Description|
|---|---|
|_Server_|Select the SAP Business One server that is registered in System Landscape Directory|
||(SLD).|
|_Import_|Choose the_Import_button to open the_Extension Import Wizard_window and import your|
||extension to SAP Business One.|
|_Remove_|Removes an imported extension. If an extension is assigned to companies, after the re-|
||moval, the assigned extension will no longer be available.|
|_Name_|Displays the name of the extension.|
|_Version_|Displays the version of the extension.|
|_Provider_|Displays the name of the SAP partner that creates and owns the extension.|
|_Parameters_|Choose the_Edit_link to edit the shared parameters that you have specifed for the extension.|
|_Force Install_|Forces the SAP Business One application to install the extension each time the user on this|
||client logs on to the assigned company.|
||If the extension is already installed, the application does not reinstall it.|
|_Status_|Displays the status of the extension.|
|_More Info_|Choose the_Details_link to view the extension details. The extension details contain the com-|
||patibility information with SAP Business One, and the extension component information if|
||the extension is an app for the version for SAP HANA.|



## **4.5 Assigning an Extension to a Company** 

Use one of the following two ways to assign an extension to a company: 

- Run the company assignment wizard 

- Run the extension assignment wizard 

## **Running the Company Assignment Wizard** 

1. In the last step of the _Extension Import Wizard_ window, choose the _Finish import and run the company assignment wizard_ hyperlink. The _Company Assignment Wizard_ window appears. 

2. From the _Specify Company_ tab, select a company to which you want to assign this extension, and choose _Next_ . 

3. Optionally, from the _Specify Parameters_ tab, specify the value of the parameters and choose _Next_ . The parameters are the parameters or configuration required to run the extension. The parameters are specific for the extension in this company. 

How to Package and Deploy SAP Business One Extensions for Lightweight Deployment **Deploying Your Extensions for Lightweight Deployment in SAP Business One** 

PUBLIC **15** 

The _Parameters_ table displays all parameters that are defined in the Extension Package tool when you package your extension. 

For more information, see Specifying Parameters Information [page 8]. 

4. From the _Specify Setup Mode_ tab, select the default startup mode of this extension, specify the user preferences, and choose _Next_ . 

   - _Default Startup Mode_ : The default startup mode determines how the extension is launched for all users that are connected to the company. 

      - _Automatic_ - SAP Business One starts the extension automatically. Users can stop automatically started add-ons with no impact on SAP Business One. A warning message informs users when the extension stops. 

      - _Manual_ - SAP Business One does not start the extension automatically. Users can start the extension at any time. A message informs users when a manually started extension is stopped. 

      - _Mandatory_ - SAP Business One starts the extension automatically. The extension is necessary for the successful operation of the SAP Business One application. The application launches the extension at start-up and shuts it down if the extension is terminated for any reason. Users cannot start or stop mandatory extensions. 

      - _Disabled_ - The extension is disabled. 

   - _User Preferences_ : All users are displayed in the User Preferences table,. letting you set preferences for users in the company. 

      - _Default_ - User preferences for the extension come from the company preferences. 

      - _Automatic_ - SAP Business One starts the extension automatically. Users can stop automatically started extensions with no impact on SAP Business One. 

      - _Manual_ - SAP Business One does not start the extension automatically. Users can start the extension at any time. 

      - _Disabled_ - The extension is disabled for the selected user. 

5. On the _Finish_ tab, if you want to assign another extension, click the _Run the company assignment wizard again_ hyperlink, and you can repeat the steps to assign the extension to another company. 

6. Choose _Finish_ to close the _Company Assignment Wizard_ window. 

7. To check the assigned extensions in a company, in the _SAP Business One Extension Manager_ window, choose the _Company Assignment_ tab. From _Company List_ , select the company and check whether the extension is available. 

## **Running the Extension Assignment Wizard** 

1. In the _SAP Business One Extension Manager_ window, choose the _Company Assignment_ tab. 

2. From _Company List_ , select the company to which you want to assign extensions. 

3. In the _Extensions_ area, choose _Assign_ . The _Extension Assignment Wizard_ window appears. 

4. On the _Specify Extension_ tab, select an extension that you want to assign to this company, and choose _Next_ . 

5. Optionally, on the _Specify Parameters_ tab, specify the value of the parameters, and choose _Next_ . The parameters are the parameters or configuration required to run the extension. The parameters are specific for the extension in this company. 

The _Parameters_ table displays all parameters that are defined in the _Extension Registration Data Generator_ tool when you package your extension. 

How to Package and Deploy SAP Business One Extensions for Lightweight Deployment **Deploying Your Extensions for Lightweight Deployment in SAP Business One** 

**16** PUBLIC 

For more information, see Specifying Parameters Information [page 8]. 

6. From the _Specify Setup Mode_ tab, select the default startup mode of this extension and specify the user preferences, and choose _Next_ . 

   - _Default Startup Mode_ : The default startup mode determines how the extension is launched for all users that are connected to the company. 

      - _Automatic_ - SAP Business One starts the extension automatically. Users can stop automatically started add-ons with no impact on SAP Business One. A warning message informs users when the extension stops. 

      - _Manual_ - SAP Business One does not start the extension automatically. Users can start the extension at any time. A message informs users when a manually started extension is stopped. 

      - _Mandatory_ - SAP Business One starts the extension automatically. The extension is necessary for the successful operation of the SAP Business One application. The application launches the extension at start-up and shuts it down if the extension is terminated for any reason. Users cannot start or stop mandatory extensions. 

      - _Disabled_ - The extension is disabled. 

   - _User Preferences_ : All users are displayed in the User Preferences table, letting you set preferences for users in the company. 

      - _Default_ - User preferences for the extension come from the company preferences. 

      - _Automatic_ - SAP Business One starts the extension automatically. Users can stop automatically started extensions with no impact on SAP Business One. 

      - _Manual_ - SAP Business One does not start the extension automatically. Users can start the extension at any time. 

      - _Disabled_ - The extension is disabled for the selected user. 

7. On the _Finish_ tab, if you want to assign another extension, click the _Run the extension assignment wizard again_ hyperlink, and repeat the steps to assign other extensions to this company. 

8. Choose _Finish_ to close the _Extension Assignment Wizard_ window. 

## **4.6 Unassigning an Extension from a Company** 

To unassign an extension from a company, perform the following steps: 

1. In the _SAP Business One Extension Manager_ window, choose the _Company Assignment_ tab. 

2. From _Company List_ , select the company for which you want to modify the extensions assignments. 

3. In the _Extensions_ area, select the extension. 

4. Choose _Unassign_ . 

##  Note 

After you unassign an extension from a company, the extension is still available in the server side, and therefore, you can still assign the extension to other companies. 

##  Note 

You can also disable an extension by deselecting the _Enabled_ checkbox in the _Extensions_ area. If an extension is disabled, when you open the SAP Business One client, the extension is not loaded. 

How to Package and Deploy SAP Business One Extensions for Lightweight Deployment **Deploying Your Extensions for Lightweight Deployment in SAP Business One** 

PUBLIC 

**17** 

## **4.7 SAP Business One Extension Manager - Company Assignment Tab** 

The _Company Assignment_ tab displays a list of available companies. Choosing a company from the list lets you see the basic information of the company and the extensions assigned to it. You can assign new extensions to or unassign existing extensions from the company. 

## **SAP Business One Extension Manager, Company Assignment Tab Fields** 

|Field|Activity/Description|
|---|---|
|_Server_|Select the SAP Business One server that is registered in System Landscape Directory|
||(SLD).|
|_Company List_|List all companies that are connected to the server.|
||Choose a company from the list to assign or unassign extensions.|
|_Database Name_|Displays the name of the company database.|
|_Company Name_|Displays the name of the company.|
|_Version_|Displays the version of SAP Business One.|
|_Extensions_|Displays the basic information of the extensions:|
||•<br>_Assign_: Choose the Assign button to open the_Extension Assignment Wizard_window|
||and assign your extension to the company.|
||•<br>_Unassign_: Choose the Unassign button to unassign an extension from a company.|
||•<br>_Name_: Displays the name of the extension.|
||•<br>_Version_: Displays the version of the extension.|
||•<br>_Provider_: Displays the name of the SAP partner that creates and owns the extension.|
||•<br>_Enabled_: By default, this checkbox is selected. You can disable an extension by dese-|
||lecting the_Enabled_checkbox. If an extension is disabled, it is not loaded when you open|
||the SAP Business One client.|
||•<br>_Settings_: Choose the_Edit_link to edit the shared parameters and the startup mode that|
||you have specifed for the extension.|
||•<br>_Status_: Displays the status of the extension.|



## **4.8 SAP Business One Extension Manager - Security Settings Tab** 

##  Note 

As of SAP Business One 10.0 FP 2011, if you want to enable the add-on security mechanism, you need to issue trusted certificates for your add-ons. The supported certificates are base64-encoded, standard 

How to Package and Deploy SAP Business One Extensions for Lightweight Deployment **Deploying Your Extensions for Lightweight Deployment in SAP Business One** 

**18** 

PUBLIC 

x.509 certificates, with the filename extension .crt or .cer. The certificate can be issued by a third-party certification authority (CA) or a local enterprise CA. For instructions on setting up a local certification authority to issue internal certificates, see Microsoft Documentation . 

The add-ons provided by SAP use an SAP certificate. The SAP certificate is by default imported in the Extension Manager. 

The _Security Settings_ tab displays a list of imported certificates. You can view or delete the existing certificates or import new certificates. 

On the _Security Settings_ tab, the checkbox _Enable Security Certificates_ is disabled by default. If you select this checkbox, the security mechanism will verify add-ons that are registered with the Add-On Manager and read the certificate information of their main executable file. 

To import a new certificate, choose _Import_ . The _Certificate Import Wizard_ appears for you to import the certificate and add comments. 

**==> picture [455 x 151] intentionally omitted <==**

## **4.9 Running the Extension in SAP Business One** 

After you assign the extension to a company, the SAP Business One client automatically loads the extension program the next time you log on to the company. 

The extension is started based on the company preferences and user preferences you set in SAP Business One Extension Manager. 

SAP Business One starts the extension automatically if you set the preference to _Automatic_ . 

To manually start the extension, perform the following steps: 

1. From the SAP Business One _Main Menu_ , choose _Administration Add-Ons Add-On Manager_ . 

2. On the _Installed Add-Ons_ tab, select the relevant extension and choose the _Start_ button. SAP Business One starts the add-on and sets the status to _Connected_ . 

3. To close the _Add-On Manager_ window, choose the _OK_ button. 

##  Caution 

If you have stopped the _SAP Business One Client Agent_ service, you must restart it before the application installs the extension. 

How to Package and Deploy SAP Business One Extensions for Lightweight Deployment **Deploying Your Extensions for Lightweight Deployment in SAP Business One** 

PUBLIC 

**19** 

If the service is stopped and you are not running the SAP Business One client as administrator, the extension will fail to load. 

**==> picture [455 x 335] intentionally omitted <==**

How to Package and Deploy SAP Business One Extensions for Lightweight Deployment **Deploying Your Extensions for Lightweight Deployment in SAP Business One** 

**20** PUBLIC 

## **5 Deploying Your Extensions for Lightweight Deployment in SAP Business One Cloud** 

You can completely configure add-ons enabled for lightweight deployment using the SAP Business One Cloud Control Center. 

To deploy an extension in SAP Business One Cloud environment, perform the following steps: 

1. Configure Extension Repositories. 

2. Copy extensions to the Incoming folder and synchronize extensions. 

3. Deploy the extension to a service unit. 

4. Assign the extension to tenants. 

For more information, see the Managing Extensions chapter in the SAP Business One Cloud Administrator's Guide. 

How to Package and Deploy SAP Business One Extensions for Lightweight Deployment **Deploying Your Extensions for Lightweight Deployment in SAP Business One Cloud** 

PUBLIC **21** 

## **6 Upgrading Your Extensions for Lightweight Deployment in SAP Business One** 

To upgrade your extension for lightweight deployment in SAP Business One, perform the following steps: 

1. Package the higher version extension files in the Extension Package tool. For more information, see Packaging Extension Data Files [page 5]. 

##  Note 

When you package a higher version extension, make sure that you specify the same _Extension Name_ and the same _Extension Provider_ , and a higher _Extension Version_ . 

2. Import the higher version extension zip file into SAP Business One Extension Manager. For more information, see Importing an Extension [page 14]. 

3. Assign the extension to a company in SAP Business One Extension Manager. This step is optional. If you have already assigned the lower version to a company, you do not need to perform this step. 

For more information, see Assigning an Extension to a Company [page 15]. 

Once the extension is assigned to a company, SAP Business One automatically loads the higher version extension program the next time you log on to the company. The lower version extension is automatically uninstalled. 

4. Run the extension in SAP Business One client. 

For more information, see SAP Business One Extension Manager - Security Settings Tab [page 18] 

##  Note 

As of SAP Business One 10.0 FP 2011, if you want to enable the add-on security mechanism, you need to issue trusted certificates for your add-ons. The supported certificates are base64-encoded, standard x.509 certificates, with the filename extension .crt or .cer. The certificate can be issued by a third-party certification authority (CA) or a local enterprise CA. For instructions on setting up a local certification authority to issue internal certificates, see Microsoft Documentation. 

The add-ons provided by SAP use an SAP certificate. The SAP certificate is by default imported in the Extension Manager. 

The _Security Settings_ tab displays a list of imported certificates. You can view or delete the existing certificates or import new certificates. 

On the _Security Settings_ tab, the checkbox _Enable Security Certificates_ is disabled by default. If you select this checkbox, the security mechanism will verify add-ons that are registered with the Add-On Manager and read the certificate information of their main executable file. 

To import a new certificate, choose _Import_ . The _Certificate Import Wizard_ appears for you to import the certificate and add comments. 

How to Package and Deploy SAP Business One Extensions for Lightweight Deployment **Upgrading Your Extensions for Lightweight Deployment in SAP Business One** 

**22** 

PUBLIC 

**==> picture [455 x 150] intentionally omitted <==**

Running the Extension in SAP Business One. 

How to Package and Deploy SAP Business One Extensions for Lightweight Deployment **Upgrading Your Extensions for Lightweight Deployment in SAP Business One** 

PUBLIC **23** 

## **7 Upgrading Your Extensions for Lightweight Deployment in SAP Business One Cloud** 

When new versions of extensions are available, you can upgrade extensions deployed to service units individually. 

Note that all tenants in the same service unit must run the same version of an extension, unless it is an add-on enabled for lightweight deployment with multiple version support. In this scenario, you can deploy multiple versions of the same add-on to a single service unit. 

## **Procedure** 

As of SAP Business One Cloud 1.1 PL10, the upgrade process is simplified. 

To upgrade the extensions that have already been assigned to tenants, you don't need to unassign the extension from all tenants and assign the upgraded version back again. 

To upgrade an extension, do the following: 

1. Copy the new extension files to the _Incoming_ folder, and synchronize the extensions by choosing the Synchronize All button from _Landscape Management Extensions_ . The system compares `Extension Name` , `Provider Name` and `Version` of the extensions. If `Extension Name` and `Provider Name` are the same, only `Version` is different, the extension is considered as a new version. 

2. Deploy the new version of the extension to the service unit. The upgraded extension is assigned to the tenants automatically. 

For more information, see the Managing Extensions chapter in the SAP Business One Cloud Administrator's Guide. 

How to Package and Deploy SAP Business One Extensions for Lightweight Deployment **Upgrading Your Extensions for Lightweight Deployment in SAP Business One Cloud** 

**24** PUBLIC 

## **Important Disclaimers and Legal Information** 

## **Hyperlinks** 

Some links are classified by an icon and/or a mouseover text. These links provide additional information. About the icons: 

- Links with the icon : You are entering a Web site that is not hosted by SAP. By using such links, you agree (unless expressly stated otherwise in your agreements with SAP) to this: 

   - The content of the linked-to site is not SAP documentation. You may not infer any product claims against SAP based on this information. 

   - SAP does not agree or disagree with the content on the linked-to site, nor does SAP warrant the availability and correctness. SAP shall not be liable for any damages caused by the use of such content unless damages have been caused by SAP's gross negligence or willful misconduct. 

- Links with the icon : You are leaving the documentation for that particular SAP product or service and are entering an SAP-hosted Web site. By using such links, you agree that (unless expressly stated otherwise in your agreements with SAP) you may not infer any product claims against SAP based on this information. 

## **Videos Hosted on External Platforms** 

Some videos may point to third-party video hosting platforms. SAP cannot guarantee the future availability of videos stored on these platforms. Furthermore, any advertisements or other content hosted on these platforms (for example, suggested videos or by navigating to other videos hosted on the same site), are not within the control or responsibility of SAP. 

## **Beta and Other Experimental Features** 

Experimental features are not part of the officially delivered scope that SAP guarantees for future releases. This means that experimental features may be changed by SAP at any time for any reason without notice. Experimental features are not for productive use. You may not demonstrate, test, examine, evaluate or otherwise use the experimental features in a live operating environment or with data that has not been sufficiently backed up. 

The purpose of experimental features is to get feedback early on, allowing customers and partners to influence the future product accordingly. By providing your feedback (e.g. in the SAP Community), you accept that intellectual property rights of the contributions or derivative works shall remain the exclusive property of SAP. 

## **Example Code** 

Any software coding and/or code snippets are examples. They are not for productive use. The example code is only intended to better explain and visualize the syntax and phrasing rules. SAP does not warrant the correctness and completeness of the example code. SAP shall not be liable for errors or damages caused by the use of example code unless damages have been caused by SAP's gross negligence or willful misconduct. 

## **Bias-Free Language** 

SAP supports a culture of diversity and inclusion. Whenever possible, we use unbiased language in our documentation to refer to people of all cultures, ethnicities, genders, and abilities. 

How to Package and Deploy SAP Business One Extensions for Lightweight Deployment **Important Disclaimers and Legal Information** 

PUBLIC **25** 

www.sap.com/contactsap 

© 2025 SAP SE or an SAP affiliate company. All rights reserved. 

No part of this publication may be reproduced or transmitted in any form or for any purpose without the express permission of SAP SE or an SAP affiliate company. The information contained herein may be changed without prior notice. 

Some software products marketed by SAP SE and its distributors contain proprietary software components of other software vendors. National product specifications may vary. 

These materials are provided by SAP SE or an SAP affiliate company for informational purposes only, without representation or warranty of any kind, and SAP or its affiliated companies shall not be liable for errors or omissions with respect to the materials. The only warranties for SAP or SAP affiliate company products and services are those that are set forth in the express warranty statements accompanying such products and services, if any. Nothing herein should be construed as constituting an additional warranty. 

SAP and other SAP products and services mentioned herein as well as their respective logos are trademarks or registered trademarks of SAP SE (or an SAP affiliate company) in Germany and other countries. All other product and service names mentioned are the trademarks of their respective companies. 

Please see https://www.sap.com/about/legal/trademark.html for additional trademark information and notices. 

**==> picture [58 x 29] intentionally omitted <==**

**THE BEST RUN** 

