<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="/css/style.css">
    <title>Survey Practice</title>
</head>

<body>
    <main>
        <section>
            <nav class="navbar">
                <ul>
                    <li>
                        <a>Survey Form</a>
                      
                    </li>
                </ul>
            </nav>
        </section>
        <section>
            <div class="main-content">
                <div class="color-container">
                    <div class="survey-container">
                        <h1 id="title">freeCodeCamp Survey Form</h1>
                        <p id="description">Thank you for taking the time to help us improve the platform </p>

                        <form id="survey-form" action="#" method="post">

                            <label for="name" id="name-label"> Name</label><br>
                            <input type="text" id="name" placeholder="Enter your name" required>

                            <br>
                            <label for="email" id="email-label">Email </label><br>
                            <input type="text" id="email" placeholder="Enter your email" required>
                            <br>
                            <label for="number" id="number-label">Number</label><br>
                            <input type="number" id="number" placeholder="Enter your number" min="1" max="9">
                            <br>
                            <label for="select" id="select-label">Select</label><br>

                            <select id="dropdown">
                                <option value=""></option>
                                <option value="1">1</option>
                                <option value="2">2</option>

                            </select>
                            <br>
                            <label for="select" id="select-label">Would you recommand my website to be visited?</label><br>
                            <label for="definitely">
                                <input type="radio" id="definitely" value="definitely" name="def-maybe-nsure">Definitely
                            </label>
                            <br>
                            <label for="maybe">
                                <input type="radio" id="maybe" name="def-maybe-nsure" value="maybe">Maybe

                            </label>
                            <br>
                            <label for="notSure">
                                <input type="radio" id="notSure" name="def-maybe-nsure" value="notSure">not Sure

                            </label>
                            <br>
                            <br>

                            <label>What would you like to improve (check all that apply)</label>
                            <br>
                            <label for="">
                                <input type="checkbox" id="" value="" name="">
                                HTML 
                            </label>
                            <br>
                            <label for="">
                                <input type="checkbox" id="" value="" name="">
                                CSS
                            </label>
                            <br>
                            <label for="">
                                <input type="checkbox" id="" value="" name="">
                                JS 
                            </label>
                            <br>
                            <br>

                            <textarea placeholder="Enter your comment here">

</textarea>
                            <br>
                            <button type="submit" id="submit" onclick="myFunction()">Submit</button>
                        </form>
                    </div>
                </div>

            </div>
        </section>
    </main>

    <script>
        function myFunction() {
            // Get the value of the input field with id="numb"
            let x = document.getElementById("number").value;
            // If x is Not a Number or less than one or greater than 10
            let text;
            if (isNaN(x) || x < 1 || x > 10) {
                text = "Input not valid";
            } else {
                text = "Input OK";
            }
            document.getElementById("number").innerHTML = text;
        }
    </script>
</body>

</html>
