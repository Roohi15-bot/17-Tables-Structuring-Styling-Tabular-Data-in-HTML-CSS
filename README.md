Tables are ideal for displaying structured data like stats, pricing, reports, and schedules.

# > 1. Basic Table Structure
   
    <table>
      <tr>
        <th>Name</th>
        <th>Role</th>
      </tr>
      <tr>
        <td>Ramya Latha</td>
        <td>Frontend Architect</td>
      </tr>
    </table>
  
Tag	        Purpose
> table  	Table container

> tr	    Table row

> th     	Table header (bold + centered)

> td        Table data cell

 Browsers render borders and spacing by default—custom styling needed.

 # 2. Table Sections: thead, tbody, tfoot
 
Use semantic grouping to improve structure and accessibility:

      <table>
        <thead>
          <tr>
            <th>Product</th>
            <th>Price</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>Domain</td>
            <td>$12/year</td>
          </tr>
          <tr>
            <td>Hosting</td>
            <td>$5/month</td>
          </tr>
        </tbody>
        <tfoot>
          <tr>
            <td>Total</td>
            <td>$72/year</td>
          </tr>
        </tfoot>
      </table>
   
 Helps screen readers and improves structure for large data sets.

 # 3. Styling Tables with CSS
 
    table {
      width: 100%;
      border-collapse: collapse;
      margin: 20px 0;
    }

    th, td {
      border: 1px solid #ccc;
      padding: 12px;
      text-align: left;
    }

    thead {
      background-color: #f4f4f4;
    }

    tbody tr:nth-child(even) {
      background-color: #f9f9f9;
    }

    tbody tr:hover {
      background-color: #e9f7ff;
    }
    
 Key properties:

> border-collapse: collapse; removes double borders

> nth-child(even) for zebra striping

> :hover for interaction feedback

# 4. Alignment Options

      td {
        text-align: left;     /* or center, right */
        vertical-align: top;  /* or middle, bottom */
      }
  
 Useful for clean, readable columns especially with numbers.

 # 5. Advanced Table Features
 
Feature               	Attribute/Tag	         Description
> Merge columns	           colspan	          Combine multiple columns in a row

> Merge rows    	         rowspan	          Combine rows in a column

> Responsive table	      overflow-x: auto	  Scrollable table on mobile

Example: Colspan

    <tr>
      <td colspan="2">Total</td>
    </tr>

# Responsive Table Tip

    .table-wrapper {
      overflow-x: auto;
    }
    <div class="table-wrapper">
      <table>...</table>
    </div>
    
 Prevents layout breaking on mobile screens.

 # Summary
Element	          Purpose
> table       Table container

> thead      	 Header section (column labels)

> tbody	       Main data body

> tfoot      	 Summary/footer rows

> tr	         Row of cells

> th       	 Header cell

> td	         Data cell

> colspan      	Merge columns

> rowspan      	Merge rows








