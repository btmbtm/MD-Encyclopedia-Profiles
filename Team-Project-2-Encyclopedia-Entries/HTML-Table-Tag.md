#HTML - Table Tag



The `<table>` tag is used to declare an HTML table. The `table` tag itself does not display data on the page, instead relying on its children tags to do so.

####Study this basic table example to see how the html is rendered on a page:



```html
	<html>
		<table>
			<th>This is a table header it uses the `<th>` tag to display information in bold</th>			
			<tr>
				<td> `<tr>` creates a row that spans both columns. `<td>` is used to create this column. Visible information is provide by the `<td>` tag </td>
				<td>`<td>` creates columns</td>	
			</tr>
			<tr>
				<td>`<tr>` creates a row that spans all columns. `<td>` is used to create this column. </td>
				<td> `<td>` creates columns </td>
			</tr>
		</table>
	</html> 
```  
  
<html>
	<table>
			<th>This is a table header it uses the `<th>` tag to display information in bold</th>
			<tr>
				<td> `<tr>` creates a row that spans both columns. `<td>` is used to create this column. Visible information is provide by the `<td>` tag </td>
				<td>`<td>` creates columns</td>	
			</tr>
			<tr>
				<td>`<tr>` creates a row that spans all columns. `<td>` is used to create this column. </td>
				<td> `<td>` creates columns </td>		
			</tr>
		</table>
</html>

<br>

####Additional table tags allow for more advanced styling using only HTML:


```html
	<html>
		<table>
		<caption>This is text written within the `<caption>` tag, it displays a title for the table.</caption>
			<th colspan = "3">This table header uses the `colspan = "3"` attribute to span the columns</th>
			<tr>
				<td rowspan = "2"> This is `<td>` with the `rowspan="2"` attribute. </td>
				<td> `<td>` </td>
				<td> `<td>` </td>
			</tr>
			<tr>			
				<td>`<td>` </td>
				<td> `<td>`</td>		
			</tr>
		</table>
   </html>
``` 

<html>
	<table>
		<caption>This is text written within the `<caption>` tag, it displays a title for the table.
		</caption>
			<th colspan = "3">This table header uses the `colspan = "3"` attribute to span the columns</th>
			<tr>
				<td rowspan = "2"> This is `<td>` with the `rowspan="2"` attribute. </td>
				<td> `<td>` </td>
				<td> `<td>` </td>
			</tr>
			<tr>			
				<td>`<td>` </td>
				<td> `<td>`</td>		
			</tr>
	</table>
</html>


<br>

####Another set of table tags allow for more advanced styling using CSS:

#####Content Grouping:
The tags below are used to break the table into sections, much like the `<header>`, `<body>` and `<footer>` tags are used to break up an html document into sections that allow for additional styling via CSS.

`<thead>` Defines a header section. 

`<tbody>`Defines a body section. 

`<tfoot>` Defines a footer section. 

`<colgroup>` Defines a group of columns which can be styled independently of other other columns. 

```html
<html>
	<table>
		<thead>
			<tr>
				<td rowspan = "2"> This is `<td>` with the `rowspan="2"` attribute.</td>
		    </tr>		
	   </thead>
	   <tbody>
	   		<tr>
				<td> `<td>` </td>
				<td> `<td>` </td>
			</tr>
		<tfoot>
			<tr>			
				<td>`<td>` </td>
				<td> `<td>`</td>		
			</tr>
		</tfoot>
	</table>
</html>
```

###Special Notes

In IE9, there is a rendering bug for `<table>`'s that causes the table height to increase if the following conditions are met. 

- Table has a parent with a non-auto width and overflow-x: auto;
- Table has enough content to horizontally overflow its parent 
- Table has`:hover` styles set on elements within the table

A workaround to fix this issue to is to set min-height: 0%; on the table's parent element. The `%` unit must be used. `px` won't work. 

###Browser Compatability

<table>
		<tr>
			<th>Feature</th>
			<th>Chrome</th>
			<th>Firefox / (Gecko)</th>
			<th>Internet Explorer</th>	
			<th>Opera</th>
			<th>Safari</th>
		<tr>
			<td>Basic support</td>
			<td>Version 1.0 and up</td>
			<td>1.0 (1.7 or earlier)</td>
			<td> Version 4.0 and up</td>
			<td>Version 7.0 and up</td>
			<td>Version 1.0 and up</td>
		</tr>
</table>
    
 





