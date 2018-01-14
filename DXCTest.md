# Technical Writer Tips and Tricks

## Table of Contents
 - [Document Standards](#document-standards)
   - [File and Folder Names](#file-and-folder-names)
     - [File Names](#file-names)
     - [Folder Names](#folder-names)
- [Document Purpose](#document-purpose)
- [Identify Your Audience](#identify-your-audience)
   - [Account Managers](#account-managers)
   - [Front End Users](#front-end-users)
   - [Developers](#developers)
   - [Support Team](#support-team)
 - [Provide Examples](#provide-examples)
 - [Be Specific](#be-specific)
 - [Glossary](#glossary)

## Document Standards

You are strongly urged to use a standard formatting template.  This should include:
1.  A document title which is clear
2.  A statement of purpose for the document
3.  Identify the intended audience
4.  The author of the document
5.  A revision history, if appropriate
6.  What version/release the information applies to, if appropriate
7.  Certain documents may also require the DXC branding or logo to be included - especially any document intended for external customers.
    * Example of a valid DXC Logo  
  ![alt text](https://github.com/l3ngl3r/MyFirstGitHub/blob/master/dxc-logo.jpg "DXC Logo")

[Back to Top](#top)

### File and Folder Names

People often search for documents within a repository using a file name, so the naming conventions of the files and folders should be consistent.  Keeping a well-organized naming structure makes it easier for people to quickly locate the information they need.

Review any existing naming standards for your team before creating a new structure.

[Back to Top](#top)

#### File Names

The file name should be descriptive of it's contents.  Utilize keywords which someone might use to search, such as the application name (DXCTest), the topic (contacts), or other descriptors such as "GetCompanyDataAPI".  Always consider the intended audience when naming files as a front-end user would search on different keywords than a technical resource might use.

[Back to Top](#top)

#### Folder Names

Folder names should follow a logical heirarchy, with the highest level being the most generic and folder names becoming more specific as you drill down.

\CoreTeam\UserGuides\CDS  
\CoreTeam\UserGuides\DXCTest    
\CoreTeam\UserGuides\Provisioning    
\CoreTeam\UserGuides\ServiceNow    
\CoreTeam\SupportDocumentation\Security\CDS  
\CoreTeam\SupportDocumentation\Security\DXCTest  
\CoreTeam\SupportDocumentation\Security\Provisioning  
\CoreTeam\SupportDocumentation\Security\ServiceNow  

[Back to Top](#top)

## Document Purpose

Before you start creating a document, you should first identify the purpose of your document.  Ask yourself a few questions to ensure you understand what the end product will provide.

  * Who is your audience?
  * Is a new document required, or is it more appropriate to update an existing document?
  
  [Back to Top](#top)

## Identify Your Audience

Every document should be written in language appropriate to the consumer of the information.  By identifying your audience you will know the level of detail to be provided.  Below you will see some examples of how you might document contact/user information for a sample application I will refer to as the DXCTest Application.

[Back to Top](#top)

### Account Managers

An account manager wouldn't need to know the technical details of how contact information is created or stored.  A high level summary would be appropriate.
1.  Contact information for each unique user is stored in the DXCTest Application.

Note that there is no item #2.  We wouldn't need to explain other details related to contacts since the account manager wouldn't be responsible for data changes, coding, or support.

[Back to Top](#top)

### Front End Users

Documentation for a front end user would contain details around UI tasks.  It would be appropriate to include screenshots and other detail helpful to their tasks.
1.  Contact information for each unique user is stored in the DXCTest Application.  
       * A unique user is based on the network login name stored within the record.
2.  The following fields are available for each contact record.

|   Field Label   |   Required?  |  Allowed Values  | Max Length|   Example     |
|-----------------|:------------:|:-----------------|:---------:|:-------------|
|UserID| Yes| Alphanumeric|20|SJONES3|
| First Name  | Yes| Alphanumeric|50| Susan| 
|Last Name| Yes | Alphanumeric, dash|50| Jones|
|Phone Number| No| Numbers, parenthesis, dash|12| 214-555-1212|
|Access Level| No| Numbers (Default is 0)|2| 3|

3.  Fields are not case-sensitive.
4. Any leading or trailing spaces entered will be removed from the stored data.

If there are any data transformation rules the user may need to understand then you can detail them at the field level, or in pseudo code or text.

5.  If no Access Level is entered, a default of 0 will be applied to new records.

[Back to Top](#top)

### Developers

Developer documentation is focused more on the technical aspects - database, APIs, keys, data transformation, etc.  Data you might provide is outlined below.

[Back to Top](#top)

### Support Team

The support team would require deployment, monitoring, and troubleshooting information.

[Back to Top](#top)

## Provide Examples


   
   
[Back to Top](#top)

## Be Specific

*Terminology matters!*  Always be aware of terms you put into your document since we are a global workplace and information can be interpreted differently based on location or experience. 
   * When referring to a field on a UI screen, use the actual field name shown to the user.
   * Be aware of regional differences in the meaning of words.
       * a 'Holiday' in the US is a company-paid day off.
       * a 'Holiday' in a European country is a vacation.
       * using the term 'company-designated holiday' would be clearer
   * If referring to a database field, use the table name and field name
   * There may be other regional differences, such as the formatting of date values - MM-DD-YYYY or DD-MM-YYYY.

[Back to Top](#top)

## Glossary

We utilize may acronyms in our day-to-day work.  A best practice would be to utilize a common glossary that contains abbreviations and their definitions, plus other terms which are common across the enterprise.  If no common glossary exists, add a glossary section to your document to ensure readers are clear on what your references mean.  

[Back to Top](#top)
