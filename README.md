# adobeCampaignClassic
AC codes
Webapp to allow WYSWYG editor for email templates in AC v6.1


Installation Instructions

1. Create a webapp with just two webpages page1 and page 2
2. Update the source of the pages as provided in repository
3. update the yourserver to to your AC server name
4. Create a jssp page with the source as provided in repo with same name and update the path of jssp page in page1 and page2 whereever required
5. Host the other resources in AC resources and update the path in page1 and pag2 source
6. Create a personalization blocks type folder with internal name "contentBlocks" 
7. Break your Email template HTML in to sections and create blocks like header/footer/modules in content block folder
8. Add the emailTemplate in Delivery Templates folder in your AC server folder "nmsDeliveryModel".
9. Make sure the editable blocks in your email template contains class contentBox. For ex if repeating outer tag in your email is a div, then all divs must have class contentBox, if all repeating modules in your template are a table, then all of them must have class "contentBox".  A sample email template is added in repo.

Features:
1. Arrange Bloacks
2. Add/Drop blocks from personalization blocks from AC
3. Edit Text/Image
4. Edit Hyperlinks
5. Edit Source code
6. Export the modified email to an existing delivery in AC
7. Export the modified email as new email template in AC
