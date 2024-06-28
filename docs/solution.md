
# Solution Architecture

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
    <tr><td>1</td><td>Assurance provider onboarding</td><td>Assurance provider</td><td></td></tr>
    <tr><td>2</td><td>OSS producer and consumer onboarding</td><td>Consumer </td><td></td></tr>
    <tr><td>3</td><td>Marketplace operator onboarding</td><td></td><td></td></tr>
    <tr><td>4</td><td>Marketplace subscription</td><td>Assurance provider,Consumer</td><td></td></tr>
    <tr><td>5</td><td>Add / modify / delete OSS projects into the projects of interest for assurance provider</td><td>Assurance provider</td><td>While adding or modifying a OSS asset, the OASP should make sure that the attested assessment reports are made available</td></tr>
    <tr><td>6</td><td>Add / modify / delete OSS models into the models of interest for assurance provider</td><td>Assurance provider</td><td>While adding or modifying a OSS asset, the OASP should make sure that the attested assessment reports are made available</td></tr>
    <tr><td>7</td><td>Search for an OSS project</td><td>Consumer</td><td></td></tr>
    <tr><td>8</td><td>Search for an OSS model</td><td>Consumer</td><td></td></tr>
    <tr><td>9</td><td>Place an order for a particular assurance service on an existing OSS artifact</td><td>Consumer</td><td>The assessment artifcats are made available at this time.
    Where do we bring in the payment?</td></tr>
    <tr><td>10</td><td>Place a request for the assurance service on a new OSS artifact</td><td>Consumer</td><td>Should we split this into OSS model and projects?</td></tr>
    <tr><td>11</td><td>Risk Assessment report</td><td></td><td></td></tr>
    <tr><td>12</td><td>Bug bounty program</td><td></td><td></td></tr>
    <tr><td>13</td><td>Remediate a particular bug </td><td></td><td></td></tr>
    <tr><td>14</td><td>Bid for the new OSS project or model onboarding request </td><td>Assurance provider</td><td></td></tr>
  </tbody>
</table>
