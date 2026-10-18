


<div>



<h1 style="float: left; margin-left: 15px; margin: 15px;">Group Play Agreement </h1>

<!-- Insert images here for https://www.playnow.com/resources/images/lottery/banners/lmax-2.0/lmax-2.0-logo-small.png -->

<!-- position the image to the right -->

<img src="https://www.playnow.com/resources/images/lottery/banners/lmax-2.0/lmax-2.0-logo-small.png" alt="LMAX 2.0 Logo" style="float: right; margin-left: 15px; margin-bottom: 15px;" />

<!-- add horizontal line full width and add padding below and make not visible -->
<hr style="width: 100%; padding-bottom: 15px; margin-top: 15px; visibility: hidden;" />

<!-- link back to readme -->
[ <<< Back](readme.md)

<STRONG>GROUP PLAY AGREEMENT</STRONG>


<!-- make Name of group stand out -->
<strong>Name of group:</strong> CM Lottery Group

<strong>[Trustee](guidelines.md#trustee):</strong> Shane Y

<strong>[Share per group member](guidelines.md#prize-money):</strong> contribution / total contributions per one draw (e.g., $6 / $120) = 1/20th

<strong>[Cut-off date for contributions](guidelines.md#deadline):</strong> First day shift (Wednesday) day set
    
<strong>[Game](guidelines.md#game):</strong> Lotto Max plus Extras

<strong>[Draw dates](calendar.html):</strong> ongoing after the cut-off date for contributions

<strong><a target="_blank" href="https://www.playnow.com/lottery/lotto-max/">Jackpot amount</a>:</strong> To be determined per draw

<strong>[Winnings distribution](guidelines.md#prize-money):</strong> Proportional to each member's share in the group as per "Share per group member" above.




<style>
    table { border-collapse: collapse; width: 100%; margin-top: 20px; }
    th, td { border: 1px solid #ddd; padding: 10px; text-align: left; }
    th { background-color: none; cursor: pointer; user-select: none; }
    th::after { content: " ↕"; font-size: 0.8em; color: #aaa; }
</style>
<table border="1" style="width: 100%; border-collapse: collapse; margin-top: 15px;">
<caption><strong>Current group members.</strong> If you have paid your contribution and submitted your information, please ensure your information is accurately reflected here. If not contact me.</caption>
  <thead>
    <tr>
      <th>#</th>
      <th>Full name</th>
      <th>City</th>
      <th>Signature</th>
      <th>Phone#</th>
      <th>$</th>
      <th>Type</th>
    </tr>
  </thead>
  <tbody>
    <!-- Add rows for each group member here -->
    <tr><td>1</td>  <td>Darlington</td>   <td>n/a</td>      <td>contribution</td>     <td>###-###-2418</td>       <td>$</td>        <td></td> </tr>
    <tr><td>2</td>  <td>Dave G</td>       <td>n/a</td>      <td>contribution</td>     <td>###-###-6181</td>       <td>$</td>        <td></td> </tr>
    <tr><td>3</td>  <td>Frank</td>        <td>n/a</td>      <td>contribution</td>     <td>###-###-1896</td>       <td>$</td>        <td></td> </tr>
    <tr><td>4</td>  <td>Jacob L</td>      <td>Hedley</td>   <td>contribution</td>     <td>###-###-0930</td>       <td>$</td>        <td></td> </tr>
    <tr><td>5</td>  <td>Jeremy</td>       <td>Jeremy</td>   <td>contribution</td>     <td>###-###-9877</td>       <td>$</td>        <td></td> </tr>
    <tr><td>6</td>  <td>Jessica</td>      <td>Hedley</td>   <td>contribution</td>     <td>###-###-5144</td>       <td>$</td>        <td></td> </tr>
    <tr><td>7</td>  <td>Nolan</td>        <td>Hedley</td>   <td>contribution</td>     <td>###-###-7526</td>       <td>$</td>        <td></td> </tr>
    <tr><td>8</td>  <td>Patrick</td>      <td>n/a</td>      <td>contribution</td>     <td>###-###-2444</td>       <td>$</td>        <td></td> </tr>
    <tr><td>9</td>  <td>Shane</td>        <td>Cawston</td>  <td>contribution</td>     <td>###-###-1405</td>       <td>$48</td>      <td>cash</td> </tr>
    <tr><td>10</td> <td>Stu</td>          <td>n/a</td>      <td>contribution</td>     <td>###-###-1266</td>       <td>$</td>        <td></td> </tr>
    <tr><td>11</td> <td>Tasha</td>        <td>n/a</td>      <td>contribution</td>     <td>###-###-0162</td>       <td>$</td>        <td></td> </tr>
    <tr><td>12</td> <td>Tony</td>         <td>n/a</td>      <td>contribution</td>     <td>###-###-3057</td>       <td>$</td>        <td></td> </tr>
    <tr><td></td>   <td></td>             <td></td>         <td></td>                 <td></td>                   <td>$48</td>      <td></td> </tr>

  </tbody>
</table>


By making your contribution, you agree to abide by the rules and guidelines of the group play agreement and the group prize agreement.


***I will be keeping a copy of full name and phone number offline.

<!-- link back to readme -->
[ <<< Back](readme.md)


</div>

<script>
function sortTable(columnIndex) {
    const table = document.querySelector("table");
    const tbody = table.querySelector("tbody");
    const rows = Array.from(tbody.querySelectorAll("tr"));
    
    // Determine sort direction (toggle between ascending and descending)
    const currentDirection = table.dataset.sortDir === "asc" ? "desc" : "asc";
    table.dataset.sortDir = currentDirection;

    // Sort rows
    rows.sort((rowA, rowB) => {
        const cellA = rowA.children[columnIndex].textContent.trim();
        const cellB = rowB.children[columnIndex].textContent.trim();

        // Check if values are numeric
        const numA = Number(cellA);
        const numB = Number(cellB);

        if (!isNaN(numA) && !isNaN(numB)) {
            return currentDirection === "asc" ? numA - numB : numB - numA;
        }

        // Fallback to alphabetical sort
        return currentDirection === "asc" 
            ? cellA.localeCompare(cellB) 
            : cellB.localeCompare(cellA);
    });

    // Re-append sorted rows to the tbody
    rows.forEach(row => tbody.appendChild(row));
}



//make div password protected
const password = "shane";
const div = document.querySelector("div");
div.style.display = "none";
const userPassword = prompt("Name of the trustee for this group?");

if (userPassword === password) {
    div.style.display = "block";
}


</script>