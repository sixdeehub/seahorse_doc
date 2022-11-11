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
    <td><code>column operation code</code></td>
    <td><pre>transform.column <- function(column, column.name) {
  return(column / 0.45359237)
}</pre></td>
  </tr>
  <tr>
    <td><code>target type</code></td>
    <td>double</td>
  </tr>
  <tr>
    <td><code>operate on</code></td>
    <td>one column</td>
  </tr>
  <tr>
    <td><code>input column</code></td>
    <td>"Weight"</td>
  </tr>
  <tr>
    <td><code>output</code></td>
    <td>append new column</td>
  </tr>
  <tr>
    <td><code>output column</code></td>
    <td>"WeightInPounds"</td>
  </tr>
  </tbody>
</table>

### Input

<table class="table">
  <thead>
    <tr>
      <th>Animal</th>
      <th>Kind</th>
      <th>Weight</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Cow</td>
      <td>Mammal</td>
      <td>300.0</td>
    </tr>
    <tr>
      <td>Ostrich</td>
      <td>Bird</td>
      <td>0.5</td>
    </tr>
    <tr>
      <td>Dog</td>
      <td>Mammal</td>
      <td>5.0</td>
    </tr>
    <tr>
      <td>Sparrow</td>
      <td>Bird</td>
      <td>0.5</td>
    </tr>
    <tr>
      <td>Thing</td>
      <td></td>
      <td>null</td>
    </tr>
  </tbody>
</table>

### Output

<table class="table">
  <thead>
    <tr>
      <th>Animal</th>
      <th>Kind</th>
      <th>Weight</th>
      <th>WeightInPounds</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Cow</td>
      <td>Mammal</td>
      <td>300.0</td>
      <td>661.3867865546327</td>
    </tr>
    <tr>
      <td>Ostrich</td>
      <td>Bird</td>
      <td>0.5</td>
      <td>1.1023113109243878</td>
    </tr>
    <tr>
      <td>Dog</td>
      <td>Mammal</td>
      <td>5.0</td>
      <td>11.023113109243878</td>
    </tr>
    <tr>
      <td>Sparrow</td>
      <td>Bird</td>
      <td>0.5</td>
      <td>1.1023113109243878</td>
    </tr>
    <tr>
      <td>Thing</td>
      <td></td>
      <td>null</td>
      <td>null</td>
    </tr>
  </tbody>
</table>

