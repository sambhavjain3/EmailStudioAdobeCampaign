# EmailStudio
Email Studio is a Webapp providing WYSWYG editor for modifying email templates in Adobe Campaign (AC v6.1)
Once configured, this webapp can be used by non technical users to modify the email templates and use them in campaigns with out any dependency on devs. 

Features:
1. Arrange Bloacks
2. Add/Drop blocks from personalization blocks from AC
3. Edit Text/Image  (Images must be already hosted in public resources in AC)
4. Edit Hyperlinks
5. Edit Source code
6. Export the modified email to an existing delivery in AC
7. Export the modified email as new email template in AC


Installation Instructions

1. Create a webapp with just two webpages page1 and page 2
2. Update the source of the pages as provided in repository
3. update the yourserver to to your AC server name
4. Create a jssp page with the source as provided in repo with same name and update the path of jssp page in page1 and page2 where ever required. Also update the logon escalation in jssp to an operator which has read/write permissions to schemas
5. Host the other resources in AC resources and update the path in page1 and page2 source
6. Create a personalization blocks type folder with internal name "contentBlocks" 
7. Break your Email template HTML in to sections and create blocks like header/footer/modules in content block folder (samples provided in resources)
8. Add the sampleEmailTemplate in Delivery Templates folder in your AC server folder "nmsDeliveryModel".
9. Make sure the editable blocks in your email template contains class contentBox. For ex if repeating outer tag in your email is a div, then all divs must have class contentBox, if all repeating modules in your template are a table, then all of them must have class "contentBox".  A sample email template is added in repo.


App Interface:
![App Interface](https://raw.githubusercontent.com/sambhavjain3/adobeCampaignClassic/master/page2EditTemplate.png)



MIT License

Copyright (c) [2018] [Sambhav Jain]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.
Proper credit to the Author must be given.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

