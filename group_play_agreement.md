<div>

<h1 style="float: left; margin-left: 15px; margin: 15px;">Group Play Agreement</h1>

<img src="https://www.playnow.com/resources/images/lottery/banners/lmax-2.0/lmax-2.0-logo-small.png" alt="LMAX 2.0 Logo" style="float: right; margin-left: 15px; margin-bottom: 15px;" />

<hr style="width: 100%; padding-bottom: 15px; margin-top: 15px; visibility: hidden;" />

<a href="/">&lt;&lt;&lt; Back</a>

<br>

<STRONG>GROUP PLAY AGREEMENT</STRONG><br><br>

<strong>Name of group:</strong> CM Lottery Group<br>
<a href="guidelines.md#trustee" style="font-weight: bold;">Trustee</a>: Shane Y<br>
<a href="guidelines.md#prize-money" style="font-weight: bold;">Share per group member</a>: contribution / total contributions per one draw (e.g., $6 / $120) = 1/20th<br>
<a href="guidelines.md#deadline" style="font-weight: bold;">Cut-off date for contributions</a>: First day shift (Wednesday) day set<br>
<a href="guidelines.md#game" style="font-weight: bold;">Game</a>: Lotto Max plus Extras<br>
<a href="calendar.html" style="font-weight: bold;">Draw dates</a>: ongoing after the cut-off date for contributions<br>
<strong><a target="_blank" href="https://www.playnow.com/lottery/lotto-max/">Jackpot amount</a>:</strong> To be determined per draw<br>
<a href="guidelines.md#prize-money" style="font-weight: bold;">Winnings distribution</a>: Proportional to each member's share in the group as per "Share per group member" above.

<style>
    table { border-collapse: collapse; width: 100%; margin-top: 20px; }
    th, td { border: 1px solid #ddd; padding: 10px; text-align: left; }
    th { background-color: none; cursor: pointer; user-select: none; }
    th::after { content: ""; font-size: 0.8em; color: #aaa; }
</style>

<table border="1" style="width: 100%; border-collapse: collapse; margin-top: 15px;">
<caption><strong>Current group members.</strong> If you have paid your contribution and submitted your information, please ensure your information is accurately reflected here. If not contact me.</caption>
  <thead>
    <tr style="cursor: pointer;">
      <th onclick="sortTable(0)">#</th>
      <th onclick="sortTable(1)">Full name</th>
      <th onclick="sortTable(2)">City</th>
      <th onclick="sortTable(3)">Signature</th>
      <th onclick="sortTable(4)">Phone#</th>
      <th onclick="sortTable(5)">$</th>
      <th onclick="sortTable(6)">Type</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>1</td><td>Darlington</td><td>n/a</td><td>contribution</td><td>###-###-2418</td><td>$</td><td></td></tr>
    <tr><td>2</td><td>Dave G</td><td>n/a</td><td>contribution</td><td>###-###-6181</td><td>$</td><td></td></tr>
    <tr><td>3</td><td>Frank</td><td>n/a</td><td>contribution</td><td>###-###-1896</td><td>$</td><td></td></tr>
    <tr><td>4</td><td>Jacob L</td><td>Hedley</td><td>contribution</td><td>###-###-0930</td><td>$</td><td></td></tr>
    <tr><td>5</td><td>Jeremy</td><td>Jeremy</td><td>contribution</td><td>###-###-9877</td><td>$</td><td></td></tr>
    <tr><td>6</td><td>Jessica</td><td>Hedley</td><td>contribution</td><td>###-###-5144</td><td>$</td><td></td></tr>
    <tr><td>7</td><td>Nolan</td><td>Hedley</td><td>contribution</td><td>###-###-7526</td><td>$</td><td></td></tr>
    <tr><td>8</td><td>Patrick</td><td>n/a</td><td>contribution</td><td>###-###-2444</td><td>$</td><td></td></tr>
    <tr><td>9</td><td>Shane</td><td>Cawston</td><td>contribution</td><td>###-###-1405</td><td>$48</td><td>cash</td></tr>
    <tr><td>10</td><td>Stu</td><td>n/a</td><td>contribution</td><td>###-###-1266</td><td>$</td><td></td></tr>
    <tr><td>11</td><td>Tasha</td><td>n/a</td><td>contribution</td><td>###-###-0162</td><td>$</td><td></td></tr>
    <tr><td>12</td><td>Tony</td><td>n/a</td><td>contribution</td><td>###-###-3057</td><td>$</td><td></td></tr>
    <tr><td></td><td></td><td></td><td></td><td></td><td>$48</td><td></td></tr>
  </tbody>
</table>

<p>By making your contribution, you agree to abide by the rules and guidelines of the group play agreement and the group prize agreement.</p>

<p><em>*I will be keeping a copy of full name and phone number offline.</em></p>

<a href="readme.md">&lt;&lt;&lt; Back</a>

</div>

<script>
function sortTable(columnIndex) {
    const table = document.querySelector("table");
    const tbody = table.querySelector("tbody");
    const rows = Array.from(tbody.querySelectorAll("tr"));
    
    const currentDirection = table.dataset.sortDir === "asc" ? "desc" : "asc";
    table.dataset.sortDir = currentDirection;

    rows.sort((rowA, rowB) => {
        const cellA = rowA.children[columnIndex].textContent.trim();
        const cellB = rowB.children[columnIndex].textContent.trim();

        const numA = Number(cellA.replace(/[^0-9.-]+/g,""));
        const numB = Number(cellB.replace(/[^0-9.-]+/g,""));

        if (!isNaN(numA) && !isNaN(numB) && cellA !== "" && cellB !== "") {
            return currentDirection === "asc" ? numA - numB : numB - numA;
        }

        return currentDirection === "asc" 
            ? cellA.localeCompare(cellB) 
            : cellB.localeCompare(cellA);
    });

    rows.forEach(row => tbody.appendChild(row));
}

// Password protection logic
const password = "shane";
const containerDiv = document.querySelector("div");
containerDiv.style.display = "none"; // Hide by default until verified
const userPassword = prompt("Name of the trustee for this group?");

if (userPassword === password) {
    containerDiv.style.display = "block";
} else {
    alert("Incorrect password!");
}
</script>