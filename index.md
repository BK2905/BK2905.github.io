<!DOCTYPE html>
<html lang="en">

	<head>
		<meta charset="utf-8" />
		<title>Party Tickets Order Form</title>
		<link rel="stylesheet" href="styles/normalize.css">
		<link rel="stylesheet" href="styles/main.css">
	</head>

	<body>
		<!-- header starts -->
		<header>
			<img src="images/pumpkin.gif" alt="Pumpkin" width="85">
			<h2>The Halloween Store</h2>
			<h3>For the little Goblin in all of us!</h3>
		</header>
		
		<!-- navigation starts -->
		<nav id="nav_menu">
			<ul>
				<li><a href="index.html" class="current">Home</a></li>
				<li><a href="about_us.html">About Us</a>
					<ul>						
						<li><a href="our_history.html">Our History</a></li>
						<li><a href="our_team.html">Our Team</a></li>
					</ul>
				</li>
				<li><a href="products.html">Our Products</a></li>
				<li><a href="tickets_order_form.html">Party Tickets</a></li>
				<li><a href="contact_us.html">Contact Us</a></li>
			</ul>
		</nav>

		<!-- main content starts -->
		<main>
			<!-- sidebar starts -->
			<aside>
				<ul>
					<li><a href="products/props.html">Props</a></li>
					<li><a href="products/costumes.html">Costumes</a></li>
					<li><a href="products/special.html">Special FX</a></li>
					<li><a href="products/masks.html">Masks</a></li>
				</ul>
			</aside>

			<!-- the main section of the content starts -->
			<section>
				<h1>Buy Tickets for a Halloween Party</h1>
				
			<!-- the order form goes here -->
				<form name="order_form" method="post" action="place_order.html">
					<fieldset id="member_info">
						<legend>Membership Information</legend>
						<label for="email">E-Mail:</label>
						<input type="email" name="email" id="email" required autofocus pattern="[a-z0-9._%+-]+@[a-z0-9.-]+\.[a-z]{2,}$" title="Must contain a valid email address, example, 'mikesmith@gmail.com'"><br>
						<label for="first_name">First Name:</label>
						<input type="text" name="first_name" id="first_name" required title="Please enter your first name here"><br>
						<label for="last_name">Last Name:</label>
						<input type="text" name="last_name" id="last_name" required title="Please enter your last name here"><br>
						<label for="address">Address:</label>
						<input type="text" name="address" id="address" required title="Please enter your street address here"><br>
						<label for="city">City:</label>
						<input type="text" name="city" id="city" required title="Please enter the name of your city here"><br>
						<label for="province">Province:</label>
						<input type="text" name="province" id="province" required pattern="[A-Za-z]{2}" placeholder="2-character code" title="Must be a 2 letter province code, example, 'ON'"><br>
						<label for="postal_code">Postal Code:</label>
						<input type="text" name="postal_code" id="postal_code" required pattern="[A-Za-z0-9]{6}" placeholder="6 characters" title="Must be 6 alphanumeric characters long"><br>
						<label for="phone_number">Phone Number:</label>
						<input type="text" name="phone" id="phone" required pattern="[0-9]{3}-[0-9]{3}-[0-9]{4}" placeholder="999-999-9999" title="Please enter a valid phone number in the correct format"><br>
					</fieldset>
					<fieldset id="order_info">
						<legend>Ordering Information</legend>
						<label for="party">Party:</label>
						<select name="party" id="party">
							<option value="ff" selected>Fang-tastic Feast</option>
							<option value="fn">Fright Night</option>
							<option value="gno">Ghoul's Night Out</option>
							<option value="mm">Monster Mash</option>
						</select><br>
						<label for="order_type">Order Type:</label>
						<select name="order_type" id="order_type">
							<option value="mp" selected>Member Package</option>
							<option value="dp">Donor Package</option>
							<option value="st"> Single Tickets</option>
						</select><br>
						<label for="number_of_tickets">Number of Tickets:</label>
						<input type="text" name="number_of_tickets" id="number_of_tickets" placeholder="Number of single tickets" pattern="[0-9]{1-2}" title="Please enter a number from 1 to 99"><br>
					</fieldset>
					<fieldset id="payment_info">
						<legend>Payment Method</legend>
						<input type="radio" id="bill_me" name="payment_mtd" value="bill_me">Bill Me
						<input type="radio" id="credit_card" name="payment_mtd" value="credit_card"> Credit Card
					</fieldset>
					<fieldset id="credit_card_info">
						<legend>Credit Card Information</legend>
						<label for="credit_card_type">Card Type:</label>
						<select name="credit_card_type" id="credit_card_type">
							<option value="visa" selected>Visa</option>
							<option value="master_card">Master Card</option>
							<option value="discover">Discover</option>
						</select><br>
						<label for="card_number">Card Number:</label>
						<input type="text" name="card_number" id="card_number" required pattern="[0-9]{16}" placeholder="16 digits" title="Please enter a valid 16 digit credit card number"><br>
						<label for="expiration_date_month">Expiration Date:</label>
						<select name="expiration_date_month" id="expiration_date_month">
							<option value="jan" selected>January</option>
							<option value="feb">February</option>
							<option value="mar">March</option>
							<option value="apr">April</option>
							<option value="may">May</option>
							<option value="june">June</option>
							<option value="july">July</option>
							<option value="aug">August</option>
							<option value="sept">September</option>
							<option value="oct">October</option>
							<option value="nov">November</option>
							<option value="dec">December</option>
						</select>
						<select name="expiration_date_year" id="expiration_date_year">
							<option value="2015" selected>2015</option>
							<option value="2016">2016</option>
							<option value="2017">2017</option>
							<option value="2018">2018</option>
							<option value="2019">2019</option>
						</select>
					</fieldset>
					<fieldset id="buttons">
						<legend>Submit Your Order</legend>
						<label>&nbsp;<label>
						<input type="submit" id="submit" value="Submit"> 
						<input type="reset" id="reset" value="Reset Fields">
						
						
					</fieldset>	
			</section>
		</main>

		<!-- footer starts -->
		<footer>
			<p>&copy; 2020 Brendan Knipfel</p>
		</footer>
	</body>
</html>
