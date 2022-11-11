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
    <td><code>input column</code></td>
    <td>"words"</td>
  </tr>
  <tr>
    <td><code>output</code></td>
    <td>append new column</td>
  </tr>
  <tr>
    <td><code>output column</code></td>
    <td>"vectors"</td>
  </tr>
  <tr>
    <td><code>max iterations</code></td>
    <td>1.0</td>
  </tr>
  <tr>
    <td><code>step size</code></td>
    <td>0.025</td>
  </tr>
  <tr>
    <td><code>seed</code></td>
    <td>0.0</td>
  </tr>
  <tr>
    <td><code>vector size</code></td>
    <td>5.0</td>
  </tr>
  <tr>
    <td><code>num partitions</code></td>
    <td>1.0</td>
  </tr>
  <tr>
    <td><code>min count</code></td>
    <td>2.0</td>
  </tr>
  </tbody>
</table>

### Input

<table class="table">
  <thead>
    <tr>
      <th>words</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>[Lorem,ipsum,at,dolor]</td>
    </tr>
    <tr>
      <td>[Nullam,gravida,non,ipsum]</td>
    </tr>
    <tr>
      <td>[Etiam,at,nunc,lacinia]</td>
    </tr>
  </tbody>
</table>

### Output

<table class="table">
  <thead>
    <tr>
      <th>words</th>
      <th>vectors</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>[Lorem,ipsum,at,dolor]</td>
      <td>[-0.005178218358196318,0.006232232786715031,-3.91125213354826E-4,0.018661257810890675,-0.023597532883286476]</td>
    </tr>
    <tr>
      <td>[Nullam,gravida,non,ipsum]</td>
      <td>[8.919694228097796E-4,0.002301964908838272,-0.006360208615660667,0.023417502641677856,-0.016035044565796852]</td>
    </tr>
    <tr>
      <td>[Etiam,at,nunc,lacinia]</td>
      <td>[-0.006070187781006098,0.003930267877876759,0.0059690834023058414,-0.004756244830787182,-0.007562488317489624]</td>
    </tr>
  </tbody>
</table>

