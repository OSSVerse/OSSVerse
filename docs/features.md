
# High Level Design

## Features

<table>
  <thead>
    <tr>
      <th>Sl.</>
      <th>Features</th>
      <th>Actors</th>
      <th>Remarks</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>1</td><td>Assurance provider onboarding</td><td>Assurance Provider</td><td></td></tr>
    <tr><td>2</td><td>OSS producer and consumer onboarding</td><td>Consumer </td><td></td></tr>
    <tr><td>3</td><td>Marketplace operator onboarding</td><td>Marketplace Operator</td><td></td></tr>
    <tr><td>4</td><td>Marketplace subscription</td><td>Assurance Provider, Consumer</td><td></td></tr>
    <tr><td>5</td><td>Add / modify / delete OSS projects into the projects of interest for assurance provider</td><td>Assurance Provider</td><td>While adding or modifying a OSS asset, the OASP should make sure that the attested assessment reports are made available</td></tr>
    <tr><td>6</td><td>Add / modify / delete OSS models into the models of interest for assurance provider</td><td>Assurance Provider</td><td>While adding or modifying a OSS asset, the OASP should make sure that the attested assessment reports are made available</td></tr>
    <tr><td>7</td><td>Search for an OSS project</td><td>Consumer</td><td></td></tr>
    <tr><td>8</td><td>Search for an OSS model</td><td>Consumer</td><td></td></tr>
    <tr><td>9</td><td>Place an order for a particular assurance service on an existing OSS artifact</td><td>Consumer</td><td>The assessment artifcats are made available at this time.
    Where do we bring in the payment?</td></tr>
    <tr><td>10</td><td>Place a request for the assurance service on a new OSS artifact</td><td>Consumer</td><td>Should we split this into OSS model and projects?</td></tr>
    <tr><td>11</td><td>Risk Assessment report</td><td></td><td></td></tr>
    <tr><td>12</td><td>Bug bounty program</td><td></td><td></td></tr>
    <tr><td>13</td><td>Remediate a particular bug </td><td></td><td></td></tr>
    <tr><td>14</td><td>Bid for the new OSS project or model onboarding request </td><td>Assurance Provider</td><td></td></tr>
  </tbody>
</table>

## OSSVerse User Interface Views

### Public View
1. OSSVerse Homepage (ossverse.com)
    -	Logo placeholder
    - Top menu navigation
    - Menus : Platform, Solutions, Resources, Company, Sign In, Get Started, Book a demo
    - Marketing banner placeholder. Also has buttons for Get Started and Explore Marketplace
    -	Featured Offerings section
    -	Featured Assurance Provider section with buttons to navigate to each of their offerings
    -	Bottom banner with links to website navigation
    -	Copyright text

2. Explore marketplace
    - Navigate to the search page from the home page. Shows the complete list of  OSS Software / Model list page with search and filter
    - Each item to be represented as tiles. Each tile should have the OSS artifact name, artifact type indicator (ML model / Project), first few lines of the description, OSSVerse recommended OASP name providing this offering. The user click on a tile will redirects to Login or Sign Up as a business user

### Producer / Business
1.	OSS artifact details page 
    - Opens up post login and when the user click on an OSS Project / Model tile from the explore marketplace view. 
    - The details page should contain the below key elements.
      -	Name of the artifact
      - Detailed description
      -	Price of assessment service (This includes 1 OASP doing assessment and 2 OASPs doing a validation). The business user is going to get an assessment report which is attested from OASP1 and validated by 2 other OASPs as end delivery
      - Default selection of marketplace recommend OASP for assessment and 2 OASPs for validation. (User will have the option to change the OASPs. The pricing will change accordingly)
      - Button to place an order. Once order is placed, the page redirects to the order tracking screen.
2.	Order details and tracking page 
    - User intuitive representation of the progress of a single order from start to delivery. 
    - Show the transaction id, OASPs delivering the service, order details, payment information, billing information, expected time of delivery
    - Provision to edit billing information
    - Provision to cancel the order if the OASP is yet to accept it
    - Link to download the deliverables. Attested and certified assessment report can be downloaded if the delivery is complete.
    - The same page can be used in the OASP view to see the order details before accepting or rejecting it. 
3. My orders
    - Shows the complete list of orders placed by this organization. 
    - On click of an item, page redirects to “Order details and tracking page”.

### Open Source Assurance Provider View

1. Dashboard
    - Gives a holistic view of the assurance provider business. 
    - Count of assigned orders for assessment. It’s a hyperlink to the pending assessment order list.
    - Count of assigned orders for validation. It’s a hyperlink to the pending validation order list.
    - Count of open challenges OASP can bid for. It’s a hyperlink to the open challenges page.
    - Statistics section about the overall business, revenue etc
    - Count of Open Source Projects this OASP is offering services. It’s a hyperlink to the OSS projects list page
    - Count of Open Source Models this OASP is offering services. It’s a hyperlink to the OSS models list page
2. Assessment orders page
    - Lists all assessment orders assigned to this OASP. Both OSS projects and models assessments are listed here. This should have search and filter feature.
    - The list can be represented as a table
    - On click of a row redirects the page to “Order details and tracking page” that is similar to the “Business/Producer” user view. 
3. Risk Assessment Order details and tracking
    - “Order details and tracking page” that is similar to the “Business/Producer” user view
    - Accept and reject button. In case of rejection, there will be a reject reason text box appears before submit.
    - Provision to mark the order as complete. User should be able to upload the deliverables at this stage.
4. Validation orders page
    - Lists all validation orders assigned to this OASP
    - The list can be represented as a table
    - On click of a row redirects the page to “Order details and tracking page” that is similar to the “Business/Producer” user view. Only addition is the Accept and reject button. In case of rejection, there will be a reject reason text box appears before submit.
5. Open challenges page
    - Lists all the open on-demand challenges published in the marketplace
    - The list can be represented as a table
    - On click of a row redirects the page to “Challenge details” page
6. Challenge details page
    - Challenge details should be there. This is similar to TopCoder challenge details page.
    - Provision to bid for the challenge with pricing, delivery timelines, deliverables etc
7. Open source projects listing page
    - Table representation of all projects this OASP supports.
    - Search and filter should be there
    - On click of a row redirects the page to OSS project details page.
    - Button to list new OSS project to marketplace
8. Open source project details page
    - Project name
    - Description
    - GitHub URL
    - Modify button click makes this page editable
    - Modify offerings checkboxes
      - Risk Assessment
      - Third-party validation of risk assessment
      - Vulnerability remediation
      - TAVOSS version (TAVOSS: Trusted and Verified Open Source Software)
      - Feature enhancement
9. List new OSS project to marketplace
    - Project name
    - Description
    - GitHub URL
    - Checkboxes to select the services that can be offered on the model
      - Risk Assessment
      - Third-party validation of risk assessment
      - Vulnerability remediation
      - TAVOSS version (TAVOSS: Trusted and Verified Open Source Software)
      - Feature enhancement
10. Open source models listing page
    - Table representation of all ML models this OASP supports.
    - Search and filter should be there
    - On click of a row redirects the page to ml model details page.
    - Button to list new ML model to marketplace
11.	ML model details page
    - Model name
    - Description
    - GitHub / HuggingFace URL
    - Modify button click makes the page editable
    - Modify offerings checkboxes
      - Risk Assessment
      - Third-party validation of risk assessment
12.	List new ML model to marketplace
    - Model name
    - Description
    - GitHub / HuggingFace URL
    - Checkboxes to select the services that can be offered on the model
    - Risk Assessment
    - Third-party validation of risk assessment

### Marketplace Operator
1. Dashboard
    - This is a typical business analytics dashboard
    - Pending order count across OASPs
    - Count of open challenges and number of bids
    - Completed order count during a time window
    - Overall revenue during a time window
    - Count of active OASPs
    - Geography wise automotive company view who are placing orders
2. Marketplace Configurations
    - User should be able to modify configurations for the below
    - Assessment pricing and validation percentages for OASP1, OASP2 and OASP3
    - Configuration to enable or disable OASP recommendations for the assessment of OSS artifacts
    - Business, OASP and OSSVerse operator user management

