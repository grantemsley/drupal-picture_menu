-- SUMMARY --

Picture menu creates a field type that allows entering a title, picture and description, then using views to format them as pretty picture menus.

-- REQUIREMENTS --

None.

-- INSTALLATION --

* Install as usual, see https://drupal.org/node/895232 for further information.

-- VIEW --

You can create a view to display the picture menu, which gives you more control over where it appears in the page.
To do this:

 - Hide the display of the field on the content type display settings
 - Create a new view with a block
 - Set format to "Unformatted list"
 - Set show to "Fields"
 - Under fields, add only this field
 - Add a contextual filter, and choose the field "Content: Nid"
 - Choose When the filter value is not available, "Provide default value"
 - Type: "Content ID from URL"
 
 Then add your block, or embed it in the page with something like Token Embed Views module
 

-- CONTACT --

Created by Grant Emsley <grant@emsley.ca>