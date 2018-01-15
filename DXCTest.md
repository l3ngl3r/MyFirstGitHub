# Technical Writer Tips and Tricks

## Table of Contents
 - [Characteristics of Good Technical Writing](#characteristics-of-good-technical-writing)
 - [Document Standards](#document-standards)
   - [Standard Formatting](#standard-formatting)
   - [File and Folder Names](#file-and-folder-names)
     - [File Names](#file-names)
     - [Folder Names](#folder-names)
- [Document Purpose](#document-purpose)
- [Identify Your Audience](#identify-your-audience)
- [Be Specific](#be-specific)
- [Glossary](#glossary)

## Characteristics of Good Technical Writing

A technical writer has to be able to write to a wide range of audiences on topics from high-level overviews to task-level documents to coding guidance.  You can find many resources on the internet with samples and guidelines, and there are also courses which you can take to learn more about best practices.  A few references are listed here.

[MIT Effective Technical Communication](http://web.mit.edu/communicate/effective_comm.html "mit.edu")  
[Qualities of a Good Technical Report](https://www.aboutcivil.org/characteristics-of-technical-report-writing.html "AboutCivilEngineering")  
[Great Examples of Technical Writing](http://www.helpscribe.com/2008/12/great-examples-of-technical-writing.html "HelpScribe")

There are even Wikipedia pages for both [Technical Writer](https://en.wikipedia.org/wiki/Technical_writer "Wikipedia") and [Technical Writing](https://en.wikipedia.org/wiki/Technical_writing "Wokipedia") if you are just getting started.

A good technical writing product exhibits the following characteristics:
* Accuracy
* Clarity
* Conciseness
* Readability
* Usability
* Correctness

[Back to Top](#top)

## Document Standards

### Standard Formatting

You are strongly urged to use a standard formatting template.  Having a cohesive feel between documents - regardless of author - presents a professional and organized impression to your enterprise.

A standard format should include:
1.  A document title which is clear
2.  A statement of purpose for the document
3.  State the intended audience
4.  The author of the document
5.  A revision history, if appropriate
6.  Which version/release the information applies to, if appropriate
7.  Certain documents may also require the DXC branding or logo to be included.  A customer's logo may also be used as needed.
    * Example of a valid DXC Logo  
  ![alt text](https://github.com/l3ngl3r/MyFirstGitHub/blob/master/dxc-logo.jpg "DXC Logo")

8.  If modifying an existing document, it may be desirable to mark the changes for the user using block quotes.

     ... this is part of the existing documentation that was unchanged.
>      This is new or changed information in the document.  
>      The blockquotes may be used to show these lines have changed.  
     
     ... then we go back to existing wording without blockquotes.


[Back to Top](#top)

### File and Folder Names

People often search for documents within a repository using a file name, so the naming conventions of the files and folders should be consistent.  Keeping a well-organized naming structure makes it easier for people to quickly locate the information they need.

Review any existing naming standards for your team before creating a new structure.  This ensures consistency in presentation.

[Back to Top](#top)

#### File Names

The file name should be descriptive of it's contents without being too long.  Utilize keywords which someone might use to search, such as the application name (DXCTest), the topic (contacts), or other descriptors such as "GetCompanyDataAPI".  Always consider the intended audience when naming files as a front-end user would search on different keywords than a technical resource might use.

If your folder structure is also well named then your file names can be shorter since some of the context can be derived from the folder name.

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

Before you start creating a document, you should first identify the purpose of your document.  Ask yourself a few questions to ensure you understand what the end product needs to provide.

  * Who is your intended audience?
  * Is a new document required, or is it more appropriate to update an existing document with the new information?
  * Do you have enough information to create a complete document?
  * Are there other people you need to collaborate with in creating the document?
  
  [Back to Top](#top)

## Identify Your Audience

Every document should be written in language appropriate to the consumer of the information.  By identifying your audience you will know the level of detail to be provided.  Some examples of different documentation types are listed below.

|  Audience| Type of Documents |
|:-----------:|:---------------------------------|
|Account Managers| High-Level Overview|
|Front-End Users | User guide for UI tasks - menus, unique keys, default values|
|Developers| API formats, Business Requirements, Database Tables/Keys/Triggers|
|Test Team| Detailed test steps for both positive and negative tests|
|Support Team| Deployment Guides, Troubleshooting Documentation|

[Back to Top](#top)

## Be Specific

*Terminology matters!*  Always be aware of terms you put into your document since we are a global workplace and information can be interpreted differently based on location or experience. 
   * When referring to a field on a UI screen, use the actual field name shown to the user.  Provide a screenshot as needed.
   * Be aware of regional differences in the meaning of words.
       * a 'Holiday' in the US is a company-paid day off.
       * a 'Holiday' in a European country is a vacation.
       * using the term 'company-designated holiday' may be clearer.
   * There may be other regional differences, such as the formatting of date values - MM-DD-YYYY or DD-MM-YYYY.
   * If referring to a database field, use the table name and field name.
   * For test cases, provide detailed steps ensuring code coverage - both positive and negative results.
   * Provide code examples as needed.  Pseudo-code may be appropriate in many cases.  If using GitHub, formatting support is available for many languages which will make the documented code more readable for the user.  For example:  
   ```csharp
      private void index(){
      MessageBox.Show("hello world");
      }
   ```
   ```sql
      update PERS_SECURITY set priority = 1, access_level = 0 where pers_id = 12345;
   ```
   * If describing the use of a service or API call, there are details described in this [GitHub Article](https://gist.github.com/iros/3426278 "GitHub REST API") to show the level of detail to include.  Ensure the document consumer has all the pieces needed to do their work.

Try to think like the consumer of your document.  What information would they need to fully understand their use of your application or service?  When writing procedure-like information, it's always a good idea to take your finished document and step through the pieces line by line just like a consumer would.  You may find gaps in your steps or wording modifications that would provide more clarity.

When in doubt, it's better to provide more detail than less detail.  Be mindful of feedback provided on your documentation and tweak the level of detail in future documents of that type as you get to know your audiences better.

[Back to Top](#top)

## Glossary

We utilize many acronyms in our day-to-day work.  A best practice could be to utilize a common glossary that contains abbreviations and their definitions, plus other terms which are common across the enterprise.  If no common glossary exists, add a glossary section to your document to ensure readers are clear on what your references mean.  

[Back to Top](#top)
