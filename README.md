
# Sales Insights An Exercise by CodeBasics

First off, this data analysis project has been taken by "Code Basics" which is a youtube channel. You can access it using below link

<ol>
  <li>
      <a href="https://www.youtube.com/watch?v=hhZ62IlTxYs&list=PLeo1K3hjS3uva8pk1FI3iK9kCOKQdz1I9"> Sales Insights Tutorial </a>
  </li>
</ol>



We are going to cleanse and visualize our data by using Microsoft Power BI as an exercise. In addition to that,  as a database, we will be using MySQL to analyze our data.

As a feedback for the youtube channel (codebasics), I have really enjoyed with the whole series which gave me a good insight to comprehend how data analysis works by using data science tools. So, this has been a good starting point to dive into data science.

<ol type = '1'>
   <li>
       <h4> To find out the total transaction of a company </h4> <p> Use this code : <code> Total Transaction = COUNTROWS('sales transactions') </code> </p> 
   </li>
 
  <li>
      <h4> To find out the revenue of a company </h4> <p> Use this code : <code> Revenue = SUM('sales transactions'[sales_amount]) </code> </p> 
   </li>
   
   <li>
      <h4> To see the revenue of a company in SQL by looking at the year 2020 </h4> <p> Use this code :
      <code> SELECT SUM(sales_amount) FROM transactions as trns INNER JOIN date as dt
             ON trns.order_date = dt.date
            WHERE dt.year = 2020) </code> </p> 
   </li>
   
   <li>
      <h4> To see the revenue of a company in SQL by looking at distinctive years </h4> <p> Use this code :
      <code>SELECT DISTINCT(year) FROM date </code> </p> 
   </li>
   
  
  <li>
     <h4>  To see the profit margin in terms of percentage </h4>
      <p> Use this code in Microsoft Power BI :
      <code> Profit Margins % = DIVIDE([Total Profit Margin], [Revenue], 0)</code> </p> 
   </li>
   
   <li>
     <h4>  To see the profit margin in terms of contribution </h4>
      <p> Use this code in Microsoft Power BI :
      <code> Profit Margin Contribution % = DIVIDE([Revenue], CALCULATE([Total Profit Margin], ALL('sales products'), ALL('sales customers'), ALL('sales markets')))</code> </p> 
   </li>
   
</ul>





<h2> To see design and short demo, click the link below: </h2>

<ol type = "1">

<li>
    <p>
       <a href="https://user-images.githubusercontent.com/110297297/191347007-36945647-3e36-4c95-9162-5c77513844d2.png">First Glance</a>
   </p>
</li>

<li>

<p>
    <a href= "https://user-images.githubusercontent.com/110297297/191347670-5d4f4c61-48dd-4760-a108-bb5f10f0b582.png"> List top 5s </a>  
</p>
</li>

<li>
<p>
   <a href= "https://user-images.githubusercontent.com/110297297/191816450-40634e06-196e-4beb-a585-fac651650987.png
"> Revenue Trend  </a>
</p>
</li>


<li>
<p>
   <a href= "https://user-images.githubusercontent.com/110297297/191347982-95e0fb58-9aaa-4648-9c7e-8dfe53515f08.png"> Comparison betweeen customer type and markets  </a>
</p>
</li>




<li>
<p>
  <a href= "https://user-images.githubusercontent.com/110297297/190001961-0e0fd3f6-d3ed-4c11-8225-761cf50a9c10.mp4" > A short insight about data with a video </a>
</p>
</li>


</ol>






