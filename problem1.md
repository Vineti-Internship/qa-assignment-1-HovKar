<table style="undefined;table-layout: fixed; width: 988px">
  <tr>
    <th>Test Scenario</th>
    <th>Test Case</th>
    <th>Test Steps</th>
    <th>Test Data</th>
    <th>Expected Result</th>
    <th>Actual Result</th>
    <th>Status</th>
  </tr>
  <tr>
    <td rowspan="11" valign = "top">Check shipping calculator</td>
    <td rowspan="8" valign = "top">Check response<br> on entering<br> valid input</td>
    <td rowspan="11" valign = "top">1. Choose country<br>2. Choose type of order<br>3. Choose shipping method<br>4. Enter parameters</td>
    <td>Country: USA<br>Type of order: Online shopping<br>Shipping method: By air<br>Weight: 0.5 kg</td>
    <td>2000 AMD</td>
    <td>2000 AMD</td>
    <td>PASS</td>
  </tr>
  <tr>
    <td>Country: USA<br>Type of order: Online shopping<br>Shipping method: By air<br>Weight: 11 kg</td>
    <td>38500 AMD</td>
    <td>38500 AMD</td>
    <td>PASS</td>
  </tr>
  <tr>
    <td>Country: USA<br>Type of order: Personal Parcel<br>Shipping method: By air<br>Weight: 4.75 kg</td>
    <td>48 USD</td>
    <td>48 USD</td>
    <td>PASS</td>
  </tr>
  <tr>
    <td>Country: USA<br>Type of order: Personal Parcel<br>Shipping method: By sea<br>Weight: 10 kg<br>Length: 310 cm<br>Width: 30 cm<br>Height: 30 cm </td>
    <td>116 USD</td>
    <td>116 USD</td>
    <td>PASS</td>
  </tr>
  <tr>
    <td>Country: USA (new)<br>Type of order: Online shopping<br>Shipping method: By air<br>Weight: 2 kg</td>
    <td>6000 AMD</td>
    <td>12000 AMD</td>
    <td>FAIL</td>
  </tr>
  <tr>
    <td>Country: Russia<br>Type of order: Online shopping<br>Shipping method: By air<br>Weight: 15 kg<br>Length: 1000 cm<br>Width: 11 cm<br>Height: 15 cm</td>
    <td>55000 AMD</td>
    <td>55000 AMD</td>
    <td>PASS</td>
  </tr>
  <tr>
    <td>Country: UK<br>Type of order: Online shopping<br>Shipping method: By air<br>Weight: 3 kg<br></td>
    <td>12000 AMD</td>
    <td>12000 AMD</td>
    <td>PASS</td>
  </tr>
  <tr>
    <td>Country: China<br>Type of order: Online shopping<br>Shipping method: By air<br>Weight: 7 kg</td>
    <td>28000 AMD</td>
    <td>28000 AMD</td>
    <td>PASS</td>
  </tr>
  <tr>
    <td rowspan="3" valign = "top">Check response<br> on entering<br> invalid input</td>
    <td>Country: USA<br>Type of order: Online shopping<br>Shipping method: By air<br>Weight: My string</td>
    <td>Weight field is empty</td>
    <td>as expected</td>
    <td>PASS</td>
  </tr>
  <tr>
    <td>Country: USA<br>Type of order: Online shopping<br>Shipping method: By air<br>Weight: -1 kg</td>
    <td>Alert invalid<br>inputs or/and<br> weight<br> field is empty</td>
    <td>weight is -1<br> and shipping<br> cost is 400<br> AMD</td>
    <td>FAIl</td>
  </tr>
  <tr>
    <td>Country: USA<br>Type of order: Online shopping<br>Shipping method: By air<br>Weight: 1+2 kg</td>
    <td>Alert invalid<br> inputs </td>
    <td>weight is<br> 1+2 and<br> shipping cost<br> is 400<br> AMD</td>
    <td>FAIL</td>
  </tr>
</table>
