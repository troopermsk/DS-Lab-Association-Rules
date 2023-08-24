<h1 align="center" > DATA SCIENCE PROJECT 3</h1>

<h2 align="left"> Description: </h2>
<p>This is a project that is aimed at implementing a FP-growth algorithm which is one of the main algorithms that is used for Association Rule Mining. <br>
  We make use of the MLXTEND library of Python for implementing this algorithm and extracting frequent itemsets after we have cleaned and collected the data in a correct form using a Pandas database. <br>
</p>
<h2 align="left"> Dataset </h3>
<p> The dataset we used for this purpose was the Online Retail Data Set made available at the UCI Machine Learning Repository. However, for the purpose of the course offered at the University, the data was made available in the form of a CSV file for students. <br>
Each of the rows contains an item that has been purchased by someone, and the columns start with the InvoiceNo and then there are other descriptive fields such as: 
<ul>
  <li>StockCode</li>
  <li>Description</li>
  <li>Product Quantity</li>
</ul>
and so on. </p>

<h2 align="left">Code Description and walk-through</h2>
<p><ol>
  <li>I first started by exploring the data and making sure to read it properly into a list (one entry for each row). We made sure to exclude rows which didn't have all of the columns or ones that started the InvoiceNo with the letter C. </li>
  <li>I implemented a dictionary in order to store for each transaction itself, all of the products that were bought. We did this using basic loops. </li>
  <li> Then, I implemented a matrix representation of the data, where we had the unique products as the columns and each of the transaction/Invoice as the rows. If the Invoice included the product, we put a 1 there to signify this fact. </li>
  <li> Once the matrix was complete, we converted it into a Pandas dataframe in order to have better efficiency and be able to manipulate the data using Numpy methods when we need further analysis.</li>
  <li>Finally, we used this matrix to implement the FP-Growth Algorithm using the MLXTEND library of Python.</li>
  <li> We also show and mention how using the algorithm allows us to see which items or products are frequently bought together, and thus surmise that customers might buy the two products as a Bundle item. </li>
</ol>
</p>
