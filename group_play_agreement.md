<div>

<h1 style="float: left; margin-left: 15px; margin: 15px;">Group Play Agreement</h1>

<img src="https://www.playnow.com/resources/images/lottery/banners/lmax-2.0/lmax-2.0-logo-small.png" alt="LMAX 2.0 Logo" style="float: right; margin-left: 15px; margin-bottom: 15px;background: #84BD00;" />

<hr style="width: 100%; padding-bottom: 15px; margin-top: 15px; visibility: hidden;" />

<br>

<strong>Name of group:</strong> CM Lottery Group<br>
<a href="guidelines.html#trustee" style="font-weight: bold;">Trustee</a>: Shane Y<br>
<a href="guidelines.html#prize-money" style="font-weight: bold;">Share per group member</a>: contribution / total contributions per one draw (e.g., $6 / $120) = 1/20th<br>
<a href="guidelines.html#deadline" style="font-weight: bold;">Cut-off date for contributions</a>: First day shift (Wednesday) day set<br>
<a href="guidelines.html#game" style="font-weight: bold;">Game</a>: Lotto Max plus Extras<br>
<a href="calendar.html" style="font-weight: bold;">Draw dates</a>: ongoing after the cut-off date for contributions<br>
<strong><a target="_blank" href="https://www.playnow.com/lottery/lotto-max/">Jackpot amount</a>:</strong> To be determined per draw<br>
<a href="guidelines.html#prize-money" style="font-weight: bold;">Winnings distribution</a>: Proportional to each member's share in the group as per "Share per group member" above.

<style>
    table { border-collapse: collapse; width: 100%; margin-top: 20px;}
    th, td { border: 1px solid #ddd; padding: 10px; text-align: left; }
    th { background-color: none; cursor: pointer; user-select: none; }
    th::after { content: ""; font-size: 0.8em; color: #aaa; }
</style>

<table border="1" style="width: 100%; border-collapse: collapse; margin-top: 15px; display: table;">
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
    <tr><td>1</td>    <td>Darlington</td>     <td>n/a</td><td>contribution</td><td class="phone">###-###-2418</td><td>$</td><td></td></tr>
    <tr><td>2</td>    <td>Dave G</td>         <td>n/a</td><td>contribution</td><td class="phone">###-###-6181</td><td>$</td><td></td></tr>
    <tr><td>3</td>    <td>Frank</td><td>n/a</td><td>contribution</td><td class="phone">###-###-1896</td><td>$</td><td></td></tr>
    <tr><td>4</td>    <td>Jacob L</td><td>Hedley</td><td>contribution</td><td class="phone">###-###-0930</td><td>$</td><td></td></tr>
    <tr><td>5</td>    <td>Jeremy</td><td>Jeremy</td><td>contribution</td><td class="phone">###-###-9877</td><td>$</td><td></td></tr>
    <tr><td>6</td>    <td>Jessica</td><td>Hedley</td><td>contribution</td><td class="phone">###-###-5144</td><td>$</td><td></td></tr>
    <tr><td>7</td>    <td>Nolan</td><td>Hedley</td><td>contribution</td><td class="phone">###-###-7526</td><td>$</td><td></td></tr>
    <tr><td>8</td>    <td>Patrick</td><td>n/a</td><td>contribution</td><td class="phone">###-###-2444</td><td>$</td><td></td></tr>
    <tr><td>9</td>    <td>Shane</td><td>Cawston</td><td>contribution</td><td class="phone">###-###-1405</td><td>$48</td><td>cash</td></tr>
    <tr><td>10</td>   <td>Stu</td><td>n/a</td><td>contribution</td><td class="phone">###-###-1266</td><td>$</td><td></td></tr>
    <tr><td>11</td>   <td>Tasha</td><td>n/a</td><td>contribution</td><td class="phone">###-###-0162</td><td>$</td><td></td></tr>
    <tr><td>12</td>   <td>Tony</td><td>n/a</td><td>contribution</td><td class="phone">###-###-3057</td><td>$</td><td></td></tr>
    <tr><td></td>     <td></td><td></td><td></td><td></td><td>$48</td><td></td></tr>
  </tbody>
</table>

<p>By making your contribution, you agree to abide by the rules and guidelines of the group play agreement and the group prize agreement.</p>

<p><em>*I will be keeping a copy of full name and phone number offline.</em></p>


</div>

<script>

const pins = document.querySelectorAll(".phone");

// Password protection logic
// get password from phones
const password = Array.from(pins).map(phone => phone.textContent.slice(-4));
const storedPassword = sessionStorage.getItem("userPassword");


const containerDiv = document.querySelector("div");
containerDiv.style.display = "block"; // Hide by default until verified
const userPassword = storedPassword ? storedPassword : prompt("What are the last four digits of your phone number?");

//store the user password for later verification
sessionStorage.setItem("userPassword", userPassword);




if (password.includes(userPassword)) {
    containerDiv.style.display = "block";
} else {
    alert("Incorrect password!");
}
</script>