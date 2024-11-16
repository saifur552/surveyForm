<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Survey Form</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f9;
            margin: 0;
            padding: 20px;
        }
        
        h1 {
            text-align: center;
            color: #4b3636;
        }

        p {
            text-align: center;
            color: #666;
        }

        form {
            max-width: 600px;
            margin: 0 auto;
            padding: 20px;
            border: 1px solid #ddd;
            border-radius: 8px;
            background-color: #fff;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }

        label {
            display: block;
            margin: 10px 0 5px;
            font-weight: bold;
            color: #333;
        }

        input, select, textarea, button {
            width: calc(100% - 20px);
            margin-bottom: 15px;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 4px;
            box-sizing: border-box;
        }

        input[type="number"] {
            max-width: 100%;
        }

        textarea {
            resize: vertical; 
            min-height: 100px;
        }

        button {
            background-color: #4CAF50;
            color: white;
            border: none;
            cursor: pointer;
            padding: 10px 20px;
            font-size: 16px;
        }

        button:hover {
            background-color: #45a049;
        }

        fieldset {
            border: 1px solid #ddd;
            border-radius: 4px;
            padding: 10px;
            margin-bottom: 15px;
            background-color: #f9f9f9;
        }

        legend {
            font-weight: bold;
            padding: 0 10px;
            color: #333;
        }

        .form-group {
            margin-bottom: 15px;
        }
    </style>
</head>

<body>
    <h1 id="title">Survey Form</h1>
    <p id="description">Fill out the survey form below.</p>
    
    <form id="survey-form">
        <!-- Name Input Field -->
        <label id="name-label" for="name">Name:</label>
        <input type="text" id="name" name="name" placeholder="Enter your name" required>
        
        <!-- Email Input Field -->
        <label id="email-label" for="email">Email:</label>
        <input id="email" type="email" name="email" placeholder="Enter your email" required>
        
        <!-- Number Input Field -->
        <label id="number-label" for="number">Number:</label>
        <input id="number" type="number" name="number" min="1" max="2" placeholder="Enter a valid number" required>
        
        <label for="dropdown">Select Your Faculty:</label>
        <select id="dropdown" name="dropdown">
            <option value="science">Science</option>
            <option value="commerce">Commerce</option>
            <option value="arts">Arts</option>
        </select>
  
        <fieldset>
            <legend>Choose Your Subject:</legend>
            <input type="radio" id="cse" name="subject" value="cse">
            <label for="cse">CSE</label>
            <input type="radio" id="marketing" name="subject" value="marketing">
            <label for="marketing">Marketing</label>
            <input type="radio" id="bangla" name="subject" value="bangla">
            <label for="bangla">Bangla</label>
        </fieldset>

     
        <fieldset>
            <legend>Check your answer:</legend>
            <label>
                <input type="checkbox" value="500tk" name="prize"> 500tk Prize Money
            </label>
            <label>
                <input type="checkbox" value="dinner" name="prize"> Buffet Dinner
            </label>
        </fieldset>
        
    
        <label for="comment">Additional Comments:</label>
        <textarea id="comment" name="comment" placeholder="Enter comment or feedback" rows="4" cols="50"></textarea>
        
      
        <button id="submit" type="submit">Submit</button>
    </form>
</body>

</html>
