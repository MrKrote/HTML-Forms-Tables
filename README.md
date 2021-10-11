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
  
&nbsp;
  
> HTML
> 
> The Button Element - ```<button></button>```
  
- represents a clickable button, used to submit forms or anywhere in a document for accessible (elérhető,rendelkezésre álló), standard button functionality.



- If the type = button -> then its a standard button

```<button type="button">JUST A BUTTON NOT Submit</button>```


- standard type is submit (make the action of the form element)

```<button>Submit</button>```
=
  
```<button type="submit">Submit</button>```


**Code:**
```
<form action="">
    <button type="button">JUST A BUTTON NOT Submit</button>
    <p>
        <button>Submit</button>
    </p>
</form>
```
  
&nbsp;
  
> HTML
> 
> Input : The Name Attribute - ```name=""```
  
- Name Attribute should put it on every single input that you use and it will be used when you send your data to a server

```<input id="username" type="text" placeholder="username" name="username">```  
  
&nbsp;
  
> HTML
> 
> **Hijacking** - Google,Reddit,Yt Search - **name** and **action** attributes
 
**Youtube Search:**
  
```
<form action="https://www.youtube.com/results">
    <p>
        <input type="text" name="search_query" id="">
        <button>Search YT</button>
    </p>
</form>
```

**Google Search:**

```
<form action="https://www.google.com/search">
    <p>
        <input type="text" name="q" id="">
        <button>Search Google</button>
    </p>
</form>
```
  
&nbsp;
  
> HTML
> 
> Radio Buttons,Checkboxes,Selected
  
**Select:**
```
<select name="" id="">    
    <option value=""></option>
</select>
```

**Normal selecter: BUT**

- Pre selected selected

- Empty option [Please select an option] : 
```
<form action="/meal">
    <label for="meal"></label>
    <select name="meal" id="meal">
        <option value="fish">Fish</option>
        <option value="veg">Vegetarian</option>
        <option value="steak">Steak</option>
        <option value="" selected >Please select an option</option>
    </select>
    <button>Submit</button>
</form>
```
  
**Normal selecter:**

- Value will send to the server
```
<form action="/meal">
    <label for="meal">Please select a meal!</label>
    <select name="meal" id="meal">
        <option value="fish">Fish</option>
        <option value="veg">Vegetarian</option>
        <option value="steak">Steak</option>
    </select>
    <button>Submit</button>
</form>
```
  
  
**Checkboxes:** -  ```<input type="checkbox" name="" id="">```

- Already checked checked

- Send the name to the server
```
<form action="/birds">
    <input type="checkbox" name="agree_tos" id="agree" checked>
    <label for="agree">I agree to everything</label>
    <button>Submit</button>
</form>
```

  
- not already checked

- doesn't send anything to the server
```
<form action="/birds">
    <input type="checkbox" name="agree_tos" id="n_agree">
    <label for="n_agree">I agree to everything</label>
    <button>Submit</button>
</form>
```
  
**Radio Buttons:** -  ```<input type="radio" name="" id="">```

To can click on just only one button -> the **name of the input** should be the **SAME**!
```
<form action="/radio">
    <input type="radio" name="size" id="xs" value="xs">
    <label for="xs">XS</label>
 
    <input type="radio" name="size" id="s" value="s">
    <label for="s">S</label>
 
    <input type="radio" name="size" id="m" value="m">
    <label for="m">M</label>
    <button>Submit</button>
</form>
```
- **for** and **id** should be the same of each pair

- **NOT** the name of the input but the value will send to the server!!
  
&nbsp;
  
> HTML
> 
> Range & Text Areas
  
**Text Areas:**

```<textarea name="" id="" cols="" rows="" placeholder="></textarea>```

- can be set the cols,rows
```
<form action="/text">
    <label for="requests">Any special requests?</label>
    <textarea name="text" id="requests" cols="40" rows="5" placeholder="Type something here..."></textarea>
    <button>Submit</button>
</form>
```
  
**Range:**

```<input type="range" name="" id="" max="" min="" value="">```

- can set the max and min value

- value is the standard,begin value
```
<form action="/cheese">
    <input type="range" name="amount" id="cheese" max="100" min="0" value="75">
    <label for="cheese">Amount of Cheese</label>
    <button>Submit</button>
</form>
```
   
&nbsp;
  
> HTML
> 
> Validations
  
```required``` - must to type something in
```
<form action="/dummy">
    <p>
        <label for="first">Enter First Name</label>
        <input type="text" name="first" id="first" required>
    </p>
```
  
```required``` **+** ```minlength``` **+** ```maxlength```
```
<p>
    <label for="username">Username</label>
    <input type="text" name="username" id="username" minlength="5" maxlength="15" required>
    <button>Submit</button>
</p>
```
  
```
<p>
    <label for="email">Email</label>
    <input type="email" required>
</p>
```
  
```
<p>
    <label for="url">URL</label>
    <input type="url" required>
</p>
</form>
 ```
