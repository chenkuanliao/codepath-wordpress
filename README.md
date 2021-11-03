# Project 7 - WordPress Pentesting

Time spent: **38** hours spent in total

> Objective: Find, analyze, recreate, and document **five vulnerabilities** affecting an old version of WordPress

## Pentesting Report

### 1. (Required) Authenticated Cross-Site Scripting via Media File Metadata
  - [X] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.7.3
  - [X] GIF Walkthrough: <img src='https://github.com/chenkuanliao/codepath-wordpress/blob/main/EXP%201.gif' title='Video Walkthrough' width='' alt='Video Walkthrough' />
  - [X] Steps to recreate: 
    - Upload an image.
    - Add "filename <noscript/><script>alert("Exploit Successful");</script>" in the description including quotes.
    - View attachment page and our alert box will pop up.
  - [X] Affected source code:
    - [Link 1](https://wpscan.com/vulnerability/741d07d1-2476-430a-b82f-e1228a9343a4)
### 2. (Required) Unauthenticated Stored Cross-Site Scripting
  - [X] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.2.1
  - [X] GIF Walkthrough: <img src='https://github.com/chenkuanliao/codepath-wordpress/blob/main/EXP%202.gif' title='Video Walkthrough' width='' alt='Video Walkthrough' />
  - [X] Steps to recreate: enter wordpress site as a viewer and paste this link in the comment box and post.
  - [X] Affected source code:
    - [Link 1](https://klikki.fi/adv/wordpress2.html)
### 3. (Required) Large File Upload Error XSS
  - [X] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.7.2
    - Fixed in version: 4.7.13
  - [X] GIF Walkthrough: <img src='https://github.com/chenkuanliao/codepath-wordpress/blob/main/EXP%203.gif' title='Video Walkthrough' width='' alt='Video Walkthrough' />
  - [X] Steps to recreate: 
    - Create a 20MB file called "Dinosaurs secret life<img src=x onerror=alert(1)>.png"
    - Goto your wordpress site and drag and dropthe file via
    - An error will appear with ... exceeds the maximum upload size for this site. along with a alert box to display that the payload has been executed.
  - [X] Affected source code:
    - [Link 1](https://hackerone.com/reports/203515)
### 4. (Optional) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types:
    - Tested in version:
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
### 5. (Optional) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types:
    - Tested in version:
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php) 

## Assets

List any additional assets, such as scripts or files

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with [LiceCap](http://www.cockos.com/licecap/).

## Notes

Describe any challenges encountered while doing the work

## License

    Copyright [Chen-Kuan Liao] [name of copyright owner]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
