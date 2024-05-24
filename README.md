<!DOCTYPE html>
<html>
<head>
    <title>Social Media Growth Service</title>
    <script>
        function calculateCost() {
            var instagramFollowersPrices = {
                500: 3000,
                1000: 5000,
                5000: 25000,
                10000: 50000
            };

            var instagramLikesPrices = {
                100: 2000,
                1000: 5000,
                5000: 12200,
                10000: 25200
            };

            var youtubeViewersPrices = {
                1000: 8500,
                5000: 35500,
                10000: 75000
            };

            var youtubeSubscribersPrices = {
                200: 10000,
                1000: 50000,
                10000: 100000
            };

            var tiktokFollowersPrices = {
                100: 2000,
                500: 5000,
                1000: 15000
            };

            var tiktokLikesPrices = {
                200: 2000,
                500: 3000,
                1000: 5000
            };

            var followers = parseInt(document.getElementById("followers").value);
            var likes = parseInt(document.getElementById("likes").value);
            var subscribers = parseInt(document.getElementById("subscribers").value);
            var comments = parseInt(document.getElementById("comments").value);

            var totalCost = (followers * instagramFollowersPrices[500]) + (likes * instagramLikesPrices[100]) + (subscribers * youtubeSubscribersPrices[200]) + (comments * tiktokLikesPrices[200]);

            document.getElementById("totalCost").innerHTML = "Total Cost: " + totalCost + " Tsh";

            // Send order details to email
            var email = "ibnyusuph418@gmail.com";
            var orderDetails = Instagram Followers: ${followers}, Instagram Likes: ${likes}, YouTube Subscribers: ${subscribers}, TikTok Likes & Viewers: ${comments};
            window.open(mailto:${email}?subject=Social Media Order&body=${orderDetails});
        }
    </script>
</head>
<body>

<h1>Welcome to our Social Media Growth Service!</h1>

<p>Choose the quantity of followers, likes, subscribers, and comments you want to buy:</p>

<form>
    <label for="followers">Number of Instagram Followers:</label>
    <input type="number" id="followers" name="followers"><br><br>
    
    <label for="likes">Number of Instagram Likes:</label>
    <input type="number" id="likes" name="likes"><br><br>

    <label for="subscribers">Number of YouTube Subscribers:</label>
    <input type="number" id="subscribers" name="subscribers"><br><br>

    <label for="comments">Number of TikTok Likes & Viewers:</label>
    <input type="number" id="comments" name="comments"><br><br>

    <input type="button" value="Calculate Cost" onclick="calculateCost()">
</form>

<div id="totalCost"></div>

<a href="https://wa.me/255733107308" target="_blank"><button>Contact via WhatsApp</button></a>
