## Example

### Parameters

<table class="table">
  <thead>
    <tr>
      <th style="width:20%">Name</th>
      <th style="width:80%">Value</th>
    </tr>
  </thead>
  <tbody>
  <tr>
    <td><code>Left dataframe id</code></td>
    <td>"beds"</td>
  </tr>
  <tr>
    <td><code>Right dataframe id</code></td>
    <td>"prices"</td>
  </tr>
  <tr>
    <td><code>expression</code></td>
    <td><pre>
SELECT DISTINCT beds.city, beds.beds
FROM beds
JOIN prices ON beds.city = prices.city
AND prices.price < 120000 * beds.beds
        </pre></td>
  </tr>
  </tbody>
</table>

### Input


#### Input 0

<table class="table">
  <thead>
    <tr>
      <th>city</th>
      <th>beds</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>CityA</td>
      <td>4.0</td>
    </tr>
    <tr>
      <td>CityC</td>
      <td>2.0</td>
    </tr>
    <tr>
      <td>CityB</td>
      <td>3.0</td>
    </tr>
  </tbody>
</table>


#### Input 1

<table class="table">
  <thead>
    <tr>
      <th>city</th>
      <th>price</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>CityA</td>
      <td>695611.0</td>
    </tr>
    <tr>
      <td>CityC</td>
      <td>294691.0</td>
    </tr>
    <tr>
      <td>CityB</td>
      <td>430784.0</td>
    </tr>
    <tr>
      <td>CityB</td>
      <td>336677.0</td>
    </tr>
    <tr>
      <td>CityA</td>
      <td>584639.0</td>
    </tr>
    <tr>
      <td>CityA</td>
      <td>579560.0</td>
    </tr>
  </tbody>
</table>


### Output

<table class="table">
  <thead>
    <tr>
      <th>city</th>
      <th>beds</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>CityB</td>
      <td>3.0</td>
    </tr>
  </tbody>
</table>

