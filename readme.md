


# AwsMetering

Mashup Sequencer project


For more technical informations : [documentation](./project.md)

- [Installation](#installation)
- [Sequences](#sequences)
    - [CheckEntitlement](#checkentitlement)
    - [CheckJWT](#checkjwt)
    - [MakeJWE](#makejwe)
    - [RegisterUsage](#registerusage)
    - [ReportUsageToAWSMarketPlace](#reportusagetoawsmarketplace)
    - [UpdateKeys](#updatekeys)


## Installation

1. In your Convertigo Studio click on ![](https://github.com/convertigo/convertigo/blob/develop/eclipse-plugin-studio/icons/studio/project_import.gif?raw=true "Import a project in treeview") to import a project in the treeview
2. In the import wizard

   ![](https://github.com/convertigo/convertigo/blob/develop/eclipse-plugin-studio/tomcat/webapps/convertigo/templates/ftl/project_import_wzd.png?raw=true "Import Project")
   
   paste the text below into the `Project remote URL` field:
   <table>
     <tr><td>Usage</td><td>Click the copy button at the end of the line</td></tr>
     <tr><td>To contribute</td><td>

     ```
     AwsMetering=git@github.com:convertigo/c8oprj-aws-metering.git:branch=master
     ```
     </td></tr>
     <tr><td>To simply use</td><td>

     ```
     AwsMetering=git@github.com:convertigo/c8oprj-aws-metering/archive/master.zip
     ```
     </td></tr>
    </table>
3. Click the `Finish` button. This will automatically import the __AwsMetering__ project


## Sequences

### CheckEntitlement

Check if this project runs on a AWS Marketaplce and has been registered

### CheckJWT

Check the JWT Token with the marketplace public key

**variables**

<table>
<tr>
<th>name</th><th>comment</th>
</tr>
<tr>
<td>JWT</td><td></td>
</tr>
</table>

### MakeJWE

**variables**

<table>
<tr>
<th>name</th><th>comment</th>
</tr>
<tr>
<td>dimension</td><td></td>
</tr>
<tr>
<td>JWT</td><td></td>
</tr>
<tr>
<td>recordId</td><td></td>
</tr>
<tr>
<td>usageQuantity</td><td></td>
</tr>
<tr>
<td>version</td><td></td>
</tr>
</table>

### RegisterUsage

Call the AWS Market place register usage API and get A JWT Token

### ReportUsageToAWSMarketPlace

**variables**

<table>
<tr>
<th>name</th><th>comment</th>
</tr>
<tr>
<td>dimension</td><td></td>
</tr>
<tr>
<td>usageQuantity</td><td></td>
</tr>
</table>

### UpdateKeys

**variables**

<table>
<tr>
<th>name</th><th>comment</th>
</tr>
<tr>
<td>keys</td><td></td>
</tr>
</table>



