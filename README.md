# HTML-Forms-Tables

> HTML
> 
> Tables
> 
```
<table>
  <td>
  <tr>
  <th>
  <thead>
  <tbody>
  <tfoot>
  <colgroup>
  <caption>
```

**Table Data Cell Element** - ```<td>``` - [cella elementek]

```
<table>
    <td>Ostrich</td>
    <td>104kg</td>
    <td>156.8</td>
</table>
```

**Table Row Element** - ```<tr>``` - [sorok]

```
<table>
    <tr>
        <td>Ostrich</td>
        <td>104kg</td>
        <td>156.8</td>
    </tr>
</table>
```

**Table Header** - ```<th>``` - [címek]

```
<table>
    <tr>
        <th>Animal</th>
        <th>Average Mass</th>
        <th>Maximum Mass</th>
    </tr>
</table>
```


**Rowspan** - Sorköz [két sorba teszi]

```<th rowspan="2">Animal</th>```


**Colspan** - Oszlopköz [két oszlopra osztja]

```<th colspan="2">Average Mass</th>```

&nbsp;

> HTML
> 
> The Form Element - ```<form></form>```

- The <form> element is a container that doesn't have any visual impact. We then fill the form with inputs,buttons,checkboxes etc..

```<form action=""></form>```
  
- The action attribute specifies WHERE the data should be sent.

- The method attribute specifies WHICH HTTP method should be used. ( later...)
  
&nbsp;
  
> HTML
> 
> The Input Element: - ```<input>```
  
- We have 20+ possible types of inputs ( color pickers , checkboxes etc..)

```
<form action="">
    <input type="text" placeholder="username">
    <input type="password" placeholder="password">
    <input type="color">
    <input type="number" placeholder="enter a number">
</form>
```
  
&nbsp;
  
> HTML
> 
> The Label Element - ```<label></label>```
  
- represents a caption for an item in a user interface

- label has a connection to to input element

- It makes the input clickable
  
```
<form action="">
    <p>
        <label for="username">Enter a Username:</label>
        <input id="username" type="text" placeholder="username">
    </p>
    <p>
        <label for="password">Enter a Password:</label>
        <input id="password" type="password" placeholder="password">
    </p>
    <p>
        <label for="color">Pick a Color:</label>
        <input id="color" type="color">
    </p>
</form>
```
  
The **FOR** attribute of the label and a **ID** attribute of the input should be the **SAME**!
  
  
