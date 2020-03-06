# pendo-resource-center
As an addition to supporting documentation for our apps the resource center will be a hub for support and more.

Current state of the Mindtouch-Pendo Resource Center integration:
What is DOES in V1:
  - Links to the help article for the page a user is on in V1 based on the available Cid on the page that maps to Mindtouch
  - Selecting this link pulls the page content into the resource center
  - Links in the content will take the user to the Community site
  - There is an option to "View in Community" which takes the user to that article on the Community Site
  - The Search functionality leverages the search alogrithm of Mindtouch
  - The search is set to query after the 3rd key stroke
  - The search will return the first 10 results (the limit can be changed)
  - Clearing search will clear results
  - There is an option for "Back to Results" that will return to the previously searched list

 What is DOES in Continuum:
  - The Search functionality leverages the search alogrithm of Mindtouch
  - The search is set to query after the 3rd key stroke
  - The search will return the first 10 results (the limit can be changed) 
  - Selecting a link pulls the page content into the resource center
  - Links in the content will take the user to the Community site
  - There is an option to "View in Community" which takes the user to that article on the Community Site
  - Clearing search will clear results
  - There is an option for "Back to Results" that will return to the previously searched list

What is does NOT do but SHOULD:
  - Provide a list of related articles based on the page you are on. Must reworking mappings and create a relational list

Learnings:
  - The page content format is difficult to work with. There are a lot of different elements that vary from page to page and I had a difficult time writing the CSS to correct all misalignments.
  - The Mindtouch API key is generated from the Admin section. Only 1 API key can be in use at a time. Regenerating the key will cause the integration to break until you change the key in the code to the new one.
  - Mindtouch API calls - https://success.mindtouch.com/Integrations/API/API_Calls
